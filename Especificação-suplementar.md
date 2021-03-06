### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 26/08/2016 | 1 | Abertura do projeto | Thiago Freire |
| 26/08/2016 | 1.1 | Adição da introdução| Thiago Freire |
| 26/08/2016 | 1.2 | Adição Usabilidade, Interfaces, Suportabilidade | Thiago Freire |
| 18/08/2016| 1.3 | Adição de: Confiabilidade, Suportabilidade, Restrição de design | Marcelo Augusto |
| 19/08/2016 | 1.4 | Adição de: Interfaces, Requisitos de licenciamento, padrões aplicáveis | Marcelo Augusto |
| 19/08/2016 | 1.5 | Adição de novas telas na Interface | Thiago Freire |
| 19/08/2016 | 1.6 | Edição do item 4.2 e adição do item 4.3 | Rodrigo Oliveira |

***

#Índice

1.  [Introdução](#1--introdução)
 1. [Finalidade](#11-finalidade)
 2. [Escopo](#12-escopo)
 3. [Definições, Acrônimos e Abreviações](#13-definições-acrônimos-e-abreviações)
 4. [Referências](#14-referências)
 5. [Visão Geral](#15-escopo)
2.  [Usabilidade](#2--usabilidade)
 1. [Facilidade de uso](#21-facilidade-de-uso)
 2. [Auto descrição](#22-auto-descrição)
 3. [Mensagens de erro](#23-mensagens-de-erro)
3.  [Confiabilidade](#3--confiabilidade)
 1. [Garantia do funcionamento em tempo integral](#31-garantia-do-funcionamento-em-tempo-integral)
 2. [Garantia de segurança dos dados informados](#32-garantia-de-segurança-dos-dados-informados)
 3. [Garantia de segurança dos dados dos clientes](#33-garantia-de-segurança-dos-dados-dos-clientes)
4. [Suportabilidade](#4--suportabilidade)
 1. [Suportabilidade para Android](#41-suportabilidade-para-android)
 2. [Suportabilidade para uso offline](#42-suportabilidade-para-uso-offline)
5. [Restrições de Design](#5--restrições-de-design)
 1. [Responsividade](#51-responsividade)
 2. [Lei de disposição das propostas de lei](#52-lei-de-disposição-das-propostas-de-lei)
6. [Interfaces](#6--interfaces)
 1. [Interfaces do usuário](#61-interfaces-do-usuário)
 2. [Interfaces de hardware](#62-interfaces-de-hardware)
 1. [Interfaces de software](#63-interfaces-de-software)
7. [Observações legais de direitos autorais etc](#8--observações-legais-de-direitos-autorais-etc)
8. [Padrões Aplicáveis](#9--padrões-aplicáveis)

***

#1.  Introdução

##1.1. Finalidade

<p align="justify">A finalidade deste documento é levantar os requisitos do sistema que não são especificados diretamente no documento de especificações de caso de uso. Neste documento os requisitos não funcionais são mais evidenciados. Portanto é possível ter uma visão mais ampla dos requisitos quando ocorre a junção destes dois documentos.</p>

##1.2. Escopo
<p align="justify">As especificações contidas neste documento estão associadas ao projeto ‘Wikilegis App’, que será desenvolvido por alunos da disciplinas Métodos de Desenvolvimento de Software e Gestão de Portifólio e Projeto da UnB Gama. O objetivo do projeto é aumentar a contribuição e interação de usuários com as propostas de leis dos parlamentares.</p>

##1.3. Definições, Acrônimos e Abreviações
<p align="justify">Click - Ação de selecionar algo.</p>

<p align="justify">Feedback - Retorno de informação dado ao usuário.</p>

##1.4. Referências
<p align="justify">Documento de Visão;</p>

<p align="justify">Especificação dos Casos de Uso.</p>

##1.5. Visão Geral
<p align="justify">O que objetiva este documento é levantar os requisitos suplementares do sistema, portanto os requisitos não funcionais como: confiabilidade, usabilidade, suportabilidade, etc.</p>

#2.  Usabilidade

##2.1. Facilidade de uso

<p align="justify">O usuário do aplicativo não necessitará de nenhum treinamento específico para conseguir utilizar o sistema.</p>

<p align="justify">O usuário deve realizar ações críticas com no máximo 5 clicks.</p>

<p align="justify">O sistema terá ícones intuitivos que direcionem o uso do aplicativo pelo usuário.</p>


##2.2. Auto descrição

<p align="justify">O aplicativo deverá dar um feedback para o usuário após cada passo do usuário, para que fique o mais compreensível possível.</p>

##2.3. Mensagens de erro

<p align="justify">Em caso de erro, o aplicativo deverá apresentar mensagens, para ajudar o usuário a identificar o problema.</p>


#3.  Confiabilidade

##3.1. Garantia do funcionamento em tempo integral

<p align="justify">O aplicativo deve funcionar 24 horas por dia, 7 dias na semana.</p>

##3.2. Garantia de segurança dos dados informados

<p align="justify">Não deve haver erro nas informações apresentadas sobre as leis.</p>

##3.3. Garantia de segurança dos dados dos clientes

<p align="justify">O sistema deve garantir que os dados dos clientes estarão de acordo com o registrado pelo cliente.</p>


#4.  Suportabilidade

##4.1. Suportabilidade para android

<p align="justify">O sistema deverá ser suportado pelo sistema operacional Android versão 4.4 (KitKat) ou superior.</p>

##4.2. Suportabilidade para uso offline

<p align="justify">O sistema também operará offline, dando a possibilidade  do usuário ler os projetos de leis e seus respectivos segmentos.</p>


#5.  Restrições de Design

##5.1. Responsividade

<p align="justify">A disposição do conteúdo na tela deve se adequar ao tamanho da tela</p>

##5.2. Lei de disposição das propostas de lei

<p align="justify">A exibição das propostas de leis no aplicativo, seguem o padrão de exposição de lei conforme a lei complementar número 95, de 26 de fevereiro de 1998.</p>

#6.  Interfaces

##6.1. Interfaces do usuário

* <p align="justify">Tela inicial</p>

* <p align="justify">Tela de cadastro</p>

* <p align="justify">Tela de resultado da pesquisa</p>

* <p align="justify">Tela de listagem e filtragem</p>

* <p align="justify">Tela de exibição do projeto de lei</p>

* <p align="justify">Tela de exibição dos segmentos</p>

* <p align="justify">Tela de informações adicionais do wikilegisApp</p>

##6.2. Interfaces de hardware

<p align="justify">Smartphone</p>

<p align="justify">Tablet</p>

##6.3. Interfaces de software

<p align="justify">Sistema Android 4.4(Kit-Kat) ou superior.</p>

<p align="justify">Android Studio</p>

#7.  Observações legais de direitos autorais etc

<p align="justify">Licença: GNU GENERAL PUBLIC LICENSE v3.0</p>

#8.  Padrões Aplicáveis

<p align="justify">Padrão arquitetural MVC (Model - View - Controller).</p>

<p align="justify">Lei complementar n° 95, de 26 de fevereiro de 1998.</p>