### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 10/08/2016 | 1 | Elaboração Inicial | Izabela Cardoso |
| 13/08/2016 | 1.1 | Ferramentas(Git)  | Izabela Cardoso |
| 16/08/2016 | 1.2 | Ferramentas(Chef) | Tiago Assunção |
| 17/08/2016 | 1.3 | Modelo do Processo | Izabela Cardoso |
| 17/08/2016 | 1.4 | Atualizando utilização do Git | Izabela Cardoso |
| 17/08/2016 | 1.5 | Atualizando utilização do padrão de nome de branch | Izabela Cardoso |
| 01/09/2016 | 1.6 | Instalação e configuração do Checkstyle | Pedro Ivo |
| 04/09/2016 | 1.7 | Atualizando política de branches | Izabela Cardoso |

***

# Sumário
1.  [Introdução](#1-Introdução)
2.  [Ferramentas](#2-ferramentas)
   * [2.1 Git e GitHub](#21-git-e-github)
      * [2.1.1 Utilização](#211-utiliza%C3%A7%C3%A3o)
   * [2.2 Chef](#22-chef)
      * [2.2.1 Instalação do ambiente (Chef)](#221-instala%C3%A7%C3%A3o-do-ambiente-chef)
   * [2.3 Circle CI](#23-circle-ci)
   * [2.4 Checkstyle](#24-checkstyle)
      * [2.4.1 Instalação no Android Studio](#231-instala%C3%A7%C3%A3o-no-android-studio)
      * [2.4.2 Configuração do Checkstyle](#232-configura%C3%A7%C3%A3o-do-checkstyle)
   
# 1. Introdução

<p align="justify">Este documento descreve o Plano de Gerenciamento de Configuração para o projeto de desenvolvimento do sistema Wikilegis Mobile, 
com o objetivo de apresentar as ferramentas utilizadas na configuração do projeto, o processo de utilização das 
mesmas e os padrões de organização e nomeclatura a serem utilizados.</p>

![Processo de Configuração do Software](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/processo_gcs.png)

# 2. Ferramentas

## 2.1. Git e GitHub

Será utilizado o Git como ferramenta de versionamento do código e o [GitHub](http://github.com/) como repositório para hospedagem do mesmo.
### 2.1.1. Utilização

#### Política de Branches

<p align="justify">Inicialmente, a equipe de gerenciamento será responsável pela criação de duas branches principais, a "master" e a "devel". Na "master" será hospedado o código revisado e aprovado pela equipe de gerenciamento, enquanto a "devel" armazenará o código que ainda precisa de revisão.</p>

<p align="justify">A equipe de gerenciamento criará um fork para o time, dentro da branch "devel" do fork, deverão ser criadas branches para cada Caso de Uso, cujo nome deve estar no seguinte padrão: "ucX_nomeDoCasoDeUso", onde X é o número identificador do Caso de Uso a ser produzido naquela branch e "nomeDoCasoDeUso" será o nome do Caso de Uso em inglês, utilizando camelCase, por exemplo "uc01_registerUser".</p>

<p align="justify">Quando o Caso de Uso for implementado, a equipe de desenvolvimento é responsável por mesclar a branch com a "devel", e fazer um "Pull Request" da branch devel para a master do respositório original (upstream).</p>

<p align="justify">Ao fim de cada iteração, a equipe de gerenciamento é responsável por revisar o código, caso o mesmo seja aprovado a equipe deve mesclá-lo com a branch "master" do respositório original e deletar as branches do fork do time, caso o mesmo seja reprovado a equipe de gerenciamento deve comentar os problemas no Pull Request e a equipe desenvolvimento deve corrigí-los. </p>

#### Padrões de nomeclatura

As mensagens de commits deverão ser escritas em inglês, seguindo o padrão abaixo, com a primeira letra maiúscula. 

```sh
git commit -m "Commit message"
```

## 2.2 Chef

Ferramenta utilizada para automatizar ambientes de desenvolvimento. Esta é implementada em [Ruby](https://www.ruby-lang.org/pt/), permitindo a execução de lógicas de programação no momento de configurar o ambiente, possibilitando a manipulação de arquivos, variáveis, pacotes, políticas de permissões, entre outros pontos. O [site oficial](https://www.chef.io/chef/)  apresenta mais informações sobre a mesma. 

Iremos aplicar funcionalidades simples, que executam a instalação na própria máquina do usuário.

### 2.2.1. Instalação do Ambiente (Chef)
Para a configuração do ambiente de desenvolvimento, foi utiliza a tecnologia [Chef](#22-chef). Toda a receita foi desenvolvida em um [repositório](https://github.com/TiagoAssuncao/chef-android) aberto. Todo o processo foi dividido em três passos: 

1. Atualização e padronização do sistema
2. Instalação do ferramental
3. Configuração do ferramental

<p align="justify">No primeiro passo, basicamente foi feita a atualização do sistema e instalação de pacotes básicos do linux, necessários para o desenvolvimento, como: vim, unzip, wget, git.</p>

<p align="justify">Posteriormente, foram obtidos os arquivos fontes necessários para executar o ambiente: android-studio, sdk. Estes foram manipulados em seus diretórios corretos e instalados.</p>

<p align="justify">Para finalizar, utilizamos alguns parâmetros para instalação e configuração de pacotes advindos do sdk. Dessa maneira, os desenvolvedores tiveram a única necessidade de rodar o script para executar toda a instalação.</p>

## 2.3 Circle CI

O Circle CI foi a ferramenta utilizada para implementação da integração contínua do projeto, as builds para o fork do time podem ser vistas [neste link](https://circleci.com/gh/izacristina/2016.2-WikiLegis) e as builds para a upstream podem ser vistas [neste link](https://circleci.com/gh/fga-gpp-mds/2016.2-WikiLegis).

A configuração para funcionamento da integração contínua foi feita através do arquivo circle.yml, descrito a seguir:

```yml
    machine:
        environment:
            PATH: "~/$CIRCLE_PROJECT_REPONAME/gradle-2.9/bin:$PATH"
            TERM: "dumb"
            ADB_INSTALL_TIMEOUT: "10"
            GRADLE_OPTS: '-Dorg.gradle.jvmargs="-Xmx2048m -XX:+HeapDumpOnOutOfMemoryError"'

    dependencies:
        pre:
            - echo y | android update sdk --no-ui --all --filter "tools"
            - echo y | android update sdk --no-ui --all --filter "build-tools-24.0.0"

    test:
        override:
            # start the emulator
            - emulator -avd circleci-android22 -no-audio -no-window:
                background: true
                parallel: true
            # wait for it to have booted
            - circle-android wait-for-boot
            # unlock the emulator screen
            - sleep 30
            - adb shell input keyevent 82
            # run tests  against the emulator.
            - ./gradlew connectedAndroidTest -PdisablePreDex
            # copy the build outputs to artifacts
            - cp -r app/build/outputs $CIRCLE_ARTIFACTS
            # copy the test results to the test results directory.
            - cp -r app/build/outputs/androidTest-results/* $CIRCLE_TEST_REPORTS
```

## 2.4 Checkstyle

O Checkstyle, conforme descrito no [Plano de Qualidade](), é uma ferramenta de análise estática para análise de códigos fonte JAVA, produzido pela IDEA. Promove uma análise em tempo real e sob demanda de padrões de código que devem ser seguidos pelos desenvolvedores. Ela é totalmente configurável e possui documentação disponível para os usuários, para mais informações, acesse: [Checkstyle Documentation](http://checkstyle.sourceforge.net/)

### 2.4.1 Instalação no Android Studio

Na IDE do Android Studio selecione, **File > Settings...**, e depois clique em **Plugins**, e selecione o botão **Browse Repositories...** conforme a figura abaixo:

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_022.png|width=600px|height=400px]]

Na nova janela que se abriu clique no campo de busca e pesquise por "Checkstyle", selecione o **CheckStyle-IDEA** e clique em **Install**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_024.png|width=600px|height=400px]]

Aguarde o download e instalação do plugin e clique em **Restart Android Studio**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_025.png|width=600px|height=400px]]

### 2.4.2 Configuração do Checkstyle

Na IDE do Android Studio, selecione **File > Settings...**, selecione **Other Settings** e depois clique em Checkstyle. Na interface lateral, próximo ao campo **Configuration File** selecione o botão **+** para adicionar um arquivo de configuração.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_026.png|width=600px|height=400px]]

Adicione uma descrição para o arquivo de configuração, selecione o marcador **"Use a local Checkstyle file"**, e clique no botão **Browse**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_027.png|width=600px|height=400px]]

Na nova janela que se abriu, busque a pasta checkstyle, localizada na pasta do repositório do WikiLegis, e escolha o **wikilegis_check.xml** e clique em **OK**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_028.png|width=600px|height=400px]]

Na janela subsequente selecione o botão **Next**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_029.png|width=600px|height=400px]]

Clique no botão **Finish** na janela de confirmação de instalação.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_030.png|width=600px|height=400px]]

Selecione o arquivo adicionado ao Android Studio, ative-o e clique em **OK**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_031.png|width=600px|height=400px]]

Na IDE do Android Studio, na barra inferior, com um projeto aberto, selecione **Checkstyle**. Clique no drop-down list chamado **Rules**.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_032.png|width=1100px|height=300px]]

Selecione o arquivo de configuração adicionado.

[[https://github.com/fga-gpp-mds/2016.2-WikiLegis/blob/master/images_wiki/Selection_033.png|width=600px|height=400px]]

Pronto! Basta rodar o Checkstyle no arquivo ou módulo do sistema em implementação para realizar a verificação de sintaxe.