### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 27/08/2016 | 1.0 | Abertura do documento | Thiago Freire |
| 27/08/2016 | 1.1 | Adição finalidade e Escopo. | Josué Nascimento da Silva |
| 28/08/2016 | 1.2 | Adição de visão geral , representação arquitetural, metas e restrições, visão casos de uso, atores diagramas de casos de uso,descrição dos casos de uso, diagrama de pacotes. | Josué Nascimento da Silva |
| 29/08/2016 | 1.3 | Adição visão lógica | Josué Nascimento da Silva |
| 29/08/2016 | 1.4 | Adição Visão de implementação | Marcelo Augusto |
| 29/08/2016 | 1.5 | Adição do diagrama de classes | Marcelo Augusto e Thiago Freire |
| 29/08/2016 | 1.6 | Adição do DE-R | Augusto Moreno e Marcelo Augusto |
| 29/08/2016 | 1.7 | Adição do ME-R | Augusto Moreno |
| 30/08/2016 | 1.8 | Edição representação arquitetural,Metas e restrições | Josué Nascimento da Silva e Rodrigo Oliveira |
| 31/08/2016 | 1.9 | Refinando representação arquitetural, Visão lógica e visão de implementação | Marcelo Augusto |
| 05/09/2016 | 2.0 | Arrumando numeração dos casos de uso | Marcelo Augusto |
| 05/09/2016 | 2.1 | Adicionando imagens | Marcelo Augusto |

***

#Índice

1.  [Introdução](#1--introdução)
 1. [Finalidade](#11-finalidade)
 2. [Escopo](#12-escopo)
 3. [Visão geral](#13-visão-geral)
2.  [Representação Arquitetural](#2-representação-arquitetural)
3. [Metas e Restrições de Arquitetura](#3-metas-e-restrições-de-arquitetura)
4. [Visão de Casos de Uso](#4-visão-de-casos-de-uso)
 1. [Atores](#41-atores)
 2. [Diagrama de Casos de Uso](#42-diagrama-de-casos-de-uso)
 3. [Descrição dos Casos de Uso](#43-descrição-dos-casos-de-uso)
5. [Visão Lógica](#5-visão-lógica)
 1. [Visão Geral](#51-visão-geral)
     1. [Diagrama de pacotes](#512-diagrama-de-pacotes)
 2. [Visão de implementação](#52-visão-de-implementação)
     1. [Diagrama de classes](#521-diagrama-de-classe)
     2. [Banco de dados](#522-banco-de-dados)

***

#1.  Introdução

##1.1. Finalidade

<p align="justify">Neste documento serão apresentadas as principais características da arquitetura do app Wikilegis, afim de permitir esclarecer como será modelada a arquitetura do sistema. Cada tópico irá explicar e formalizar as decisões com base nos requisitos do sistema.</p>

##1.2. Escopo

<p align="justify">Este documento de arquitetura de software se destina ao app Wikilegis, sistema desenvolvido por alunos da disciplina de Métodos de Desenvolvimento de Software da Faculdade Gama.</p>

##1.3. Visão geral

<p align="justify">O documento é apresentado em uma serie de visão arquiteturais: Visão caso de uso, visão lógica e visão de implementação.</p>

#2. Representação Arquitetural

<p align="justify">A arquitetura será a MVC (Model-View-Controller) adaptada para Android, onde também terá uma camada DAO, uma API REST e um banco local. Utilizando essa arquitetura o projeto do software será padronizado.</p>

<p align="justify">No MVC adaptado para Android existem as seguintes camadas:</p>

* <p align="justify">Controller que é a camada responsável por interpretar as entradas fornecidas pelo usuário através da interface do sistema (View), mapeando-as em comandos que serão enviados para atualização e/ou busca de dados na camada DAO utilizando um objeto da camada Model, e estes comandos podem ser utilizados para visualização (View) e uma possível alteração necessária.</p>

* <p align="justify">View é a camada responsável por toda a interação com o usuário.</p>

* <p align="justify">Model que é a camada que gerencia os dados, responde as perguntas sobre seus estados e dados, e responde instruções para mudança de estado. A camada Model também é a responsável por modelar e gerenciar os dados referentes ao problema que se está tentando resolver.</p>

* <p align="justify">A camada DAO é utilizada para se fazer requisições para a API REST incitadas pela Controller a fim de atualizar as alterações da model na base de dados ou repassar informações da base de dados para alguma camada solicitante, e também é utilizada por gravar transmitir <i>querys</i> para atualização do banco de dados local.</p>

<p align="justify">As relações entre as camadas está descrita na figura 1.</p>

![Figura1](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/mvc.png)
<p align="justify"><b>Figura 1</b> - Funções das camadas Model-View-Controller-DAO</p>


#3. Metas e Restrições de Arquitetura

<p align="justify">O sistema será funcional em plataformas Android partir da versão 4.4(kitkat), o ambiente de desenvolvimento utilizado será o Android Studio, neste ambiente será utilizado a linguagem de programação JAVA e a linguagem de marcação XML. Como o aplicativo terá funcionalidades <i>offline</i> será implementado um banco de dados local utilizando o SQLite. Para as funcionalidades <i>online</i> será feito a comunicação com uma API REST que irá interagir através de requisições GET e POST para atualização/solicitação de dados da base de dados.</p>

<p align="justify">Com a utilização do padrão MVC existe uma maior organização no momento do desenvolvimento, por ser uma equipe formada por vários membros é importante que todos sigam um padrão de desenvolvimento, permitindo que todos possam ter conhecimento pleno do que está sendo elaborado e facilitando a manutenção do sistema por qualquer membro desenvolvedor.</p>

#4. Visão de Casos de Uso

##4.1. Atores

![atores](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/atores.jpg)

* **Cidadão brasileiro Cadastrado**: O cidadão pode visualizar, filtrar, pesquisar, comentar,  compartilhar,avaliar sugerir uma proposta de alteração em um projeto ou segmento de lei 

* **Cidadão brasileiro Visitante**: O cidadão  pode visualizar, filtrar e pesquisar um projeto de lei.

##4.2. Diagrama de Casos de Uso

![Diagrama de casos de uso](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/UseCaseDiagramm.png)

##4.3. Descrição dos Casos de Uso

<p align="justify">A seguir são apresentadas as descrições dos casos de uso do sistema , dos quais do UC01 ao UC04 serão apresentados na 1° release:</p>

* **UC01 - Realizar cadastro:** <p align="justify">Esse caso de uso permite ao cidadão visitante cadastrar-se no sistema.</p>

* **UC02 - Visualizar projeto de lei:** <p align="justify">Esse caso de uso permite que a ambos os cidadãos (cadastrados ou visitantes), visualizar os projetos de lei.</p>

* **UC03 - Visualizar segmento de projeto:** <p align="justify">Esse caso de uso permite aos cidadãos, visualizar os itens dos projetos de lei.</p>

* **UC04 - Listar projetos de lei:** <p align="justify">Este caso de uso permite ao cidadão listar projetos de lei de acordo com a forma de filtragem desejada, podendo ser por relevância, data e status (abertos).</p>

* **UC05 - Editar perfil:** <p align="justify">Esse caso de uso permite ao cidadão cadastrado editar seu perfil pessoal no sistema.</p>

* **UC06 - Pesquisar projeto:** <p align="justify">Esse caso de uso permite ao cidadão pesquisar por projetos que contenham uma determinada palavra chave em seu título ou em algum de seus itens.</p>

* **UC07 - Efetuar login:** <p align="justify">Esse caso permite ao cidadão cadastrado efetuar o login em sua conta no sistema.</p>

* **UC08 - Sugerir proposta:** <p align="justify">Permite exclusivamente ao cidadão cadastrado fazer uma sugestão ao projeto de lei de seu interesse.</p>

* **UC09 - Relatar erro:** <p align="justify">Esse caso permite aos cidadãos informar algum mal funcionamento no sistema.</p>

* **UC10 - compartilhar projeto:** <p align="justify">Permite ao cidadão cadastrado compartilhar um projeto de lei por completo em suas redes pessoais.</p>

* **UC11 - Ativar notificações:** <p align="justify">Permite ao cidadão cadastrado receber notificações sobre ao andamento de projetos de lei de seu interesse.</p>

* **UC12 - Visualizar segmento do projeto:** <p align="justify">Permite tanto ao cidadão cadastrado como ao não cadastrado visualizar parte mais internas do projeto de lei, tais como artigos, parágrafos e incisos que compõem aquele projeto de lei.</p>

* **UC13 - Avaliar segmento:** <p align="justify">Permite exclusivamente ao cidadão cadastrado “dar like” ou “dislike” nos artigos, parágrafos ou incisivos que compõem o projeto de lei.</p>

* **UC14 - Comentar segmento:** <p align="justify">Permite ao cidadão cadastrado comentar artigos, parágrafos ou incisos que compõem o projeto de lei.</p>

* **UC15 - Compartilhar segmento:** <p align="justify">Permite exclusivamente ao cidadão cadastrado compartilhar parágrafos, artigos ou incisivos que compõem o projeto de lei.</p>

#5. Visão lógica

<p align="justify">A visão lógica do aplicativo será distribuída em 4 pacotes principais sendo eles os pacotes Model, DAO, Controller e View.</p>

<p align="justify">Na Model estará a representação das entidades que compõem o sistema, como:</p>
* classes que irão representar o usuário;
* entidade projeto de lei; 
* entidade segmento;

<p align="justify">Na View estarão as classes responsáveis pelos formulários, que são as camadas responsáveis pela interação com os usuários, lá estarão as classes responsáveis pelas telas de registro, login, resultado da pesquisa, informação e filtragem.</p>

<p align="justify">Na Controller estão as classe responsáveis por estabelecer as comunicações entre a interface do aplicativo(View), o pacote Model e o pacote DAO gerenciando os registros, as filtragens, os comentários e as avaliações dos segmentos. </p>

<p align="justify">Na DAO estará as classes responsáveis por fazer a comunicação entre a aplicação e o banco de dados/API.</p>

<p align="justify">Então o usuário irá fazer solicitações ao aplicativo, as solicitações são recebidas pela View, processadas pela Controller que é o intermediário entre a View e a Model, a Model tenta a criação do objeto requirido, caso ele seja instanciado corretamente a Controller entra em contato com a DAO para efetivar as alterações da Model na base de dados do sistema.</p>

##5.1. Visão Geral

###5.1.2. Diagrama de pacotes

![Diagrama de pacotes](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/Package Diagram.jpg)

##5.2. Visão de implementação

<p align="justify">Representando a camada View, existe o pacote View. Esta é a camada de apresentação, nela irão ficar os arquivos referentes à parte visual do projeto, que são os arquivos XML, as classes Activities e as classes Fragments. Embora as classes Activities tenham características tanto de View quanto de Controller a trataremos como View pois as Activities cuidam de toda a interação da aplicação com o usuário, ou seja, como o XML será renderizado pela aplicação, como por exemplo: No caso de uma interação de um usuário clicar em um botão e acontecer uma ação na tela do usuário, toda a parte de ouvidores de botão e apresentação de dados na tela é controlada pela Activity.</p>

<p align="justify">Representando a camada Model, existe o pacote Model. Na Model é onde se faz a entrada, leitura e validação de dados do sistema.</p>

<p align="justify">A camada Controller deverá ficar dentro do pacote Controller. Ela é responsável por fazer a interação entre as Views, Model e DAO.</p>

<p align="justify">A camada DAO será responsável pela comunicação entre a API REST/Banco local e a controller. A API é responsável pela comunicação com o banco, através de uma requisição GET ou POST, solicitada por um dos componentes da DAO. O resultado desta solicitação é capturado por um componente da DAO e repassado para as camadas solicitantes.</p>

###5.2.1. Diagrama de classe

![Diagrama de classes](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/Class Diagram.jpg)

Para melhor visualização da imagem acesse : [Diagrama de classe](http://goo.gl/akOzAr)


###5.2.2. Banco de dados

* **DE-R**

![Diagrama entidade-relacionamento](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/derMDS2.jpg)

* **ME-R**

![Modelo entidade-relacionamento](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/merMDS3.jpg)