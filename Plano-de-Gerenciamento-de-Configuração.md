# Sumário
1.  [Introdução](#2-ferramentas)
2.  [Ferramentas](#2-ferramentas)
 1. [Git e GitHub](#21-git-e-github)
 2. [Utilização](#22-utiliza%C3%A7%C3%A3o)

# 1. Introdução

Este documento descreve o Plano de Gerenciamento de Configuração para o projeto de desenvolvimento do sistema X, 
com o objetivo de apresentar as ferramentas utilizadas na configuração do projeto, o processo de utilização das 
mesmas e os padrões de organização e nomeclatura a serem utilizados.

# 2. Ferramentas

## 2.1. Git e GitHub

Será utilizado o Git como ferramenta de versionamento do código e o [GitHub](http://github.com/) como repositório para hospedagem do mesmo.
### 2.1.1. Utilização

#### Política de Branches

Inicialmente, a equipe de gerenciamento será responsável pela criação de duas branches principais, a "master" e a "devel". Na "master" será hospedado o código revisado e aprovado pela equipe de gerenciamento, enquanto a "devel" armazenará o código que ainda precisa de revisão.

Dentro da branch "devel" deverão ser criadas branches para cada issue.

#### Padrões de nomeclatura

```sh
git commit -m "Issue #X: commit message"
```

## 2.2 Chef

Ferramenta utilizada para automatizar ambientes de desenvolvimento. Esta é implementada em [Ruby](https://www.ruby-lang.org/pt/), permitindo a execução de lógicas de programação no momento de configurar o ambiente, possibilitando a manipulação de arquivos, variáveis, pacotes, políticas de permissões, entre outros pontos. O [site oficial](https://www.chef.io/chef/)  apresenta mais informações sobre a mesma. 

Iremos aplicar funcionalidades simples, que executam a instalação na própria máquina do usuário.

### 2.2.1. Instalação do Ambiente (Chef)
Para a configuração do ambiente de desenvolvimento, foi utiliza a tecnologia [Chef](#22-chef). Toda a receita foi desenvolvida em um [repositório](https://github.com/TiagoAssuncao/chef-android) aberto. Todo o processo foi dividido em três passos: 

1. Atualização e padronização do sistema
2. Instalação do ferramental
3. Configuração do ferramental

No primeiro passo, basicamente foi feita a atualização do sistema e instalação de pacotes básicos do linux, necessários para o desenvolvimento, como: vim, unzip, wget, git.

Posteriormente, foram obtidos os arquivos fontes necessários para executar o ambiente: android-studio, sdk. Estes foram manipulados em seus diretórios corretos e instalados.

Para finalizar, utilizamos alguns parâmetros para instalação e configuração de pacotes advindos do sdk. Dessa maneira, os desenvolvedores tiveram a única necessidade de rodar o script para executar toda a instalação. 