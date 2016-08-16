# Plano de Gerenciamento de configuração

## Sumário
1.  Introdução [Introdução](#2-ferramentas)
2.  Ferramentas
 1. Git e GitHub
 2. Utilização

* "1. Introdução":#1-introducao
* "2. Ferramentas":#2-ferramentas
** "2.1. Git e Github":#21-git-e-github
** "2.2. Utilização":#22-utilizacao

## 1. Introdução

Este documento descreve o Plano de Gerenciamento de Configuração para o projeto de desenvolvimento do sistema X, 
com o objetivo de apresentar as ferramentas utilizadas na configuração do projeto, o processo de utilização das 
mesmas e os padrões de organização e nomeclatura a serem utilizados.

## 2. Ferramentas

### 2.1. Git e GitHub

Será utilizado o Git como ferramenta de versionamento do código e o "GitHub":http://github.com/ como repositório para hospedagem do mesmo.

### 2.2. Utilização

### Política de Branches

Inicialmente, a equipe de gerenciamento será responsável pela criação de duas branches principais, a "master" e a "devel". Na "master" será hospedado o código revisado e aprovado pela equipe de gerenciamento, enquanto a "devel" armazenará o código que ainda precisa de revisão.

Dentro da branch "devel" deverão ser criadas branches para cada issue.

### Padrões de nomeclatura

```sh
git commit -m "Issue #X: commit message"
