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

## 2.2 Chef

Ferramenta utilizada para automatizar ambientes de desenvolvimento. O [site oficial](https://www.chef.io/chef/)  apresenta mais informações sobre a mesma. Esta é implementada em [Ruby](https://www.ruby-lang.org/pt/), permitindo a execução de lógicas de programação no momento de configurar o ambiente, possibilitando a manipulação de arquivos, variáveis, pacotes, políticas de permissões, entre outros pontos. Iremos aplicar funcionalidades simples, que executam a instalação na própria máquina do usuário.

## 2.3. Utilização

### Política de Branches

Inicialmente, a equipe de gerenciamento será responsável pela criação de duas branches principais, a "master" e a "devel". Na "master" será hospedado o código revisado e aprovado pela equipe de gerenciamento, enquanto a "devel" armazenará o código que ainda precisa de revisão.

Dentro da branch "devel" deverão ser criadas branches para cada issue.

### Padrões de nomeclatura

```sh
git commit -m "Issue #X: commit message"

### Instalação do Ambiente (Chef)
Para a configuração do ambiente de desenvolvimento, foi utiliza a tecnologia C
