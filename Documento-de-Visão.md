### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 18/08/2016 | 1 | Abertura do projeto | Thiago Freire, Rodrigo Oliveira, Augusto Moreno, Josué Nascimento, Marcelo Augusto |
| 18/08/2016 | 1.1 | Adição da introdução: objetivo e visão geral da solução. | Thiago Freire, Rodrigo Oliveira, Augusto Moreno, Josué Nascimento, Marcelo Augusto |
| 18/08/2016 | 1.2 | Adição da descrição do usuário e principais necessidades. | Thiago Freire, Rodrigo Oliveira, Augusto Moreno, Josué Nascimento, Marcelo Augusto |
| 18/08/2016| 1.3 | Adição dos envolvidos, visão geral do produto, perspectiva do produto e declaração de posição do produto. | Thiago Freire, Rodrigo Oliveira, Augusto Moreno, Josué Nascimento, Marcelo Augusto |
| 19/08/2016 | 1.4 | Adição do ambiente do usuário. | Marcelo Augusto |
| 19/08/2016 | 1.5 | Adição de alternativas e competição | Marcelo Augusto e Thiago Freire |
| 19/08/2016 | 1.6 | Mudanças na introdução ,objetivos, tabela de visão geral. | Rodrigo Oliveira |
| 20/08/2016 | 1.7 | Desempenho, Revisão gramatical | Augusto Moreno |
| 20/08/2016 | 1.8 | Adição da visão geral da solução e referência | Rodrigo Oliveira |
| 20/08/2016 | 1.9 | Adição de recursos do programa | Marcelo Augusto e Augusto Moreno |
| 20/08/2016 | 2.0 | Requisitos não funcionais usabilidade e confiabilidade | Thiago Nogueira |
| 21/08/2016 | 2.1 | Adição de gráfico do ambiente do usuário | Marcelo Augusto |
| 21/08/2016 | 2.2 | Mudança da tabela de declaração da posição do produto | Rodrigo Oliveira |
| 22/08/2016 | 2.3 | Mudanças na visão geral da solução  |Josué Nascimento|
| 25/08/2016 | 2.4 | Adição de RNF | Marcelo Augusto |
| 26/08/2016 | 2.5 | Correção de requisitos não funcionais | Thiago Freire |
***

#Índice

1.  [Introdução](#1--introdução)
 1. [Objetivos](#11-objetivos)
 2. [Visão geral da solução](#12-visão-geral-da-solução)
2.  [Descrição do usuário](#2--descrição-do-usuário)
 1. [Usuário](#21-usuário)
 2. [Principais necessidades do usuário](#22-principais-necessidades-do-usuário)
 3. [Ambiente do usuário](#23-ambiente-do-usuário)
 4. [Alternativas e competição](#24-alternativas-e-competição)
     1. [Plataforma web Wikilegis](#241-plataforma-web-wikilegis)
     2. [SigaLei](#242-sigalei)
     3. [Monitora, Brasil!](#243-monitora-brasil)
     4. [Infoleg](#244-infoleg)
3.  [Envolvidos](#3--envolvidos)
4.  [Visão geral do produto](#4--visão-geral-do-produto)
 1. [Perspectiva do produto](#41-perspectiva-do-produto)
 2. [Declaração de posição do produto](#42-declaração-de-posição-do-produto)
 3. [Recursos do produto](#43-recursos-do-produto)
5.  [Requisitos não funcionais](#5--requisitos-não-funcionais)
6.  [Referências](#6-referências)

***

#1.  Introdução

<p align="justify">Este documento apresenta uma visão geral do projeto, definindo as necessidades, características e requisitos do sistema.</p>

##1.1. Objetivos

<p align="justify">Os objetivos deste documento são auxiliar na obtenção de informações dos usuários a cerca do aplicativo WikilegisApp,  do projeto ajudar a equipe desenvolvedora a ter uma visão alinhada sobre o escopo, melhorar a avaliação do desenvolvimento do software e validar com o cliente a visão da equipe de desenvolvimento acerca do aplicativo.</p>

##1.2. Visão geral da solução
<p align="justify">"A dinâmica atual da democracia representativa em nosso país revela uma triste realidade, a parcela da população que se posiciona e questiona ativamente as irregularidades praticadas e a não representatividade dos partidos políticos e governantes do país é bastante reduzida" (FONSECA, 2009, p. 15).</p>

<p align="justify">Assim, o que ocorre em nosso sistema político é que grande parcela da população não tem acesso a meios para contribuir com a criação das leis ou não possuem interesse em entrar em um computador para acessar uma aplicação web e contribuir.</p>
<p align="justify">O sistema WikilegisApp é a transformação da plataforma Web em uma plataforma mobile e vem como uma forma de promover uma interação maior entre a população e seus representantes políticos, promovendo um ambiente onde qualquer cidadão com um smartphone possa analisar e contribuir com os projetos de leis.</p>

<p align="justify">Na tabela a seguir, é mostrado um resumo acerca do problema e da solução apresentada.</p>

<table style="width:100%">
  <tr>
    <td><b>O problema da</b></td>
    <td>Difícil comunicação entre a população e seus representantes políticos,</td> 
  </tr>
  <tr>
    <td><b>Afeta</b></td>
    <td>Toda a população brasileira,</td> 
  </tr>
  <tr>
    <td><b>cujo impacto é</b></td>
    <td>A elaboração de leis que não correspondem às reais necessidades da população,</td> 
  </tr>
   <tr>
    <td><b>e uma boa solução seria</b></td>
    <td>Um aplicativo que utiliza características de redes sociais para uma maior integração entre os cidadãos e seus representantes políticos.</td> 
  </tr>
</table>

#2.  Descrição do usuário

<p align="justify">Como o aplicativo traz uma oportunidade de políticos apresentarem suas propostas de lei, criadas na plataforma web do Wikilegis, e dos cidadãos poderem analisar e contribuir com elas, os usuários serão em sua maioria, cidadãos e políticos brasileiros.</p>

##2.1. Usuário

| Tipo | Descrição | Principais Responsabilidades |
| :---: | :---: | --- |
|Cidadão|Cidadãos brasileiros.|Fiscalizar e colaborar com as leis propostas por parlamentares.|
|Parlamentar|Representantes legais da população.|Acompanhar as sugestões para suas propostas de lei.|


##2.2. Principais necessidades do usuário

| Necessidade | Problema | Solução atual | Solução proposta |
| :---: | :---: | :---: | :---: |
|O usuário tem a necessidade de analisar e contribuir com os projetos de leis.|A dificuldade de alcançar os políticos para se fazer sugestões em projetos de lei de forma prática, acessível e que permita mobilidade.|Um sistema web que possibilita ao usuário analisar e contribuir com os projetos de leis propostos pelos deputados.|Um sistema mobile que possibilita ao usuário analisar e contribuir com os projetos de leis propostos pelos deputados.|
|O usuário tem a necessidade de acompanhar o debate da sociedade acerca de seus projetos de lei.|A dificuldade de alcançar os cidadãos de uma maneira prática e abrangente para receber sugestões acerca de seus projetos de lei.|Um sistema web que possibilita ao usuário expor projetos de leis para debate com a sociedade.|Um sistema mobile que possibilita ao usuário expor projetos de leis para debate com a sociedade.|

##2.3. Ambiente do usuário

<p align="justify">Para que o usuário possa usar o aplicativo com maior mobilidade e para que ele atinja uma gama maior de usuários, visto que 80,4% (<a href="http://agenciabrasil.ebc.com.br/economia/noticia/2016-04/celular-e-principal-meio-de-acesso-internet-na-maioria-dos-lares">IBGE</a>) dos usuários de internet no Brasil em 2016 já utilizam smartphones para acesso e 91,8% (<a href="https://macmagazine.com.br/2016/02/01/ios-fechou-2015-com-apenas-28-de-mercado-no-brasil-android-dominou-com-918/">Kantar Worldpanel</a>) dos usuários que utilizam smartphone utilizavam o sistema operacional Android até 2015, o sistema será desenvolvido para o sistema operacional Android, esperando-se que o usuário possua um telefone celular com este sistema, e que o mesmo possua acesso à internet.</p>

<figure>
    <img src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/imageVisao1.png" alt="Ambiente do usuário" align="middle">
    <br>
    <figcaption style="text-align: center">Figura 1 - Ambiente do usuário.</figcaption>
</figure>


##2.4. Alternativas e competição

<p align="justify">Nesta seção serão descritos os principais produtos semelhantes encontrados encontrados.</p>

###2.4.1. Plataforma web Wikilegis

<figure>
    <img src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/imageVisao2.png" alt="Plataforma web wikilegis" align="middle">
    <br>
    <figcaption style="text-align: center">Figura 2 - Plataforma web wikilegis.</figcaption>
</figure>
<br>
<p align="justify">O uso de celular para acessar a internet ultrapassou, de acordo com o IBGE em 2016, o do computador pela primeira vez no Brasil, com esta grande crescente de utilização de internet no celular está surgindo cada vez mais a necessidade de fazer plataformas mobiles de diversas aplicações. O versão mobile Wikilegis trás consigo a mudança de plataforma tornando assim a aplicação mais abrangente.</p>

###2.4.2. SigaLei

<figure>
    <img src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao3.png" align="middle">
    <br>
    <figcaption style="text-align: center">Figura 3 - Tela do aplicativo SigaLei.</figcaption>
</figure>
<br>
<p align="justify">Trata-se de um aplicativo informativo que tem como principal objetivo, mostrar as leis que estão em trâmite de aprovação no Congresso nacional e assembleias de Minas Gerais. Os usuários podem acompanhar as discussões a respeito das leis e ser informado das atualizações de projetos de leis do seu interesse.</p>

###2.4.3. Monitora, Brasil!

<figure>
    <img src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao4.png" align="middle">
    <br>
    <figcaption style="text-align: center">Figura 4 - Tela do aplicativo Monitora, Brasil!.</figcaption>
</figure>
<br>
<p align="justify">Monitora, Brasil é um aplicativo para Android que possibilita a qualquer pessoa pesquisar e monitorar o que os Deputados Federais estão fazendo na Câmara dos Deputados. Com ele, é possível verificar a assiduidade, os projetos propostos, rankings, Twitter e outras informações.</p>

###2.4.4. Infoleg

<figure>
    <img src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao5.png" align="middle">
    <br>
    <figcaption style="text-align: center">Figura 5 - Tela do aplicativo Infoleg.</figcaption>
</figure>
<br>
<p align="justify">Aplicativo com informações das atividades legislativas da Câmara dos Deputados, com informações sobre deputados, projetos de lei e outras proposições, sessões no plenário, reuniões nas comissões e legislação.</p>

#3.  Envolvidos

| Nome | Descrição | Principais Responsabilidades |
| :---: | :---: | --- |
|Carla Silva Rocha Aguiar|Orientadora e avaliadora do projeto e do produto|Acompanhar e avaliar o desenvolvimento do projeto e do produto.|
|Josué Nascimento da Silva|Membro da equipe de desenvolvimento.|Executar o projeto, desenvolvendo e mantendo a documentação e o software.|
|Marcelo Augusto Araújo dos Reis|Membro da equipe de desenvolvimento.|Executar o projeto, desenvolvendo e mantendo a documentação e o software.|
|Rodrigo Oliveira Campos|Membro da equipe de desenvolvimento.|Executar o projeto, desenvolvendo e mantendo a documentação e o software.|
|Thiago Nogueira Freire|Membro da equipe de desenvolvimento.|Executar o projeto, desenvolvendo e mantendo a documentação e o software.|
|Augusto Moreno Vilarins Cardoso da Silva|Membro da equipe de desenvolvimento.|Executar o projeto, desenvolvendo e mantendo a documentação e o software.|
|Izabela Cristina Nere Rodrigues Cardoso|Membro da equipe de gerenciamento.|Gerir o projeto, planejando e administrando o andamento a fim de garantir que o produto final seja conforme especificado.|
|Igor Ribeiro Barbosa Duarte|Membro da equipe de gerenciamento.|Gerir o projeto, planejando e administrando o andamento a fim de garantir que o produto final seja conforme especificado.|
|Pedro Ivo Andrade|Membro da equipe de gerenciamento.|Gerir o projeto, planejando e administrando o andamento a fim de garantir que o produto final seja conforme especificado.|
|Tiago Assunção|Membro da equipe de gerenciamento.|Gerir o projeto, planejando e administrando o andamento a fim de garantir que o produto final seja conforme especificado.|
|Lucas Brilhante|Membro da equipe de gerenciamento.|Gerir o projeto, planejando e administrando o andamento a fim de garantir que o produto final seja conforme especificado.|
|Victor Hugo|Coach da equipe de desenvolvimento|Auxiliar no desenvolvimento do projeto|
|Emilie Morais|Coach da equipe de gerenciamento.|Auxiliar a equipe no gerenciamento do projeto|



#4.  Visão geral do produto

<p align="justify">O aplicativo tem por funcionalidade principal, a contribuição e interação de usuários com as propostas de leis dos parlamentares.</p>

<p align="justify">Usuários cadastrados podem curtir ou descurtir um artigo ou comentário de uma proposta de lei, sugerir uma alteração no artigo de uma proposta de lei, comentar em artigos de propostas de lei e escolher receber notificações via e-mail a respeito de alterações em um projeto. Já os usuários não cadastrados, poderão apenas visualizar as informações e comentários dos projetos de leis.</p>

##4.1. Perspectiva do produto

<p align="justify">Tem por expectativa que o aplicativo fomente o interesse do cidadão brasileiro em verificar quais as leis estão em trâmite para serem aprovados, podendo assim, contribuir com as mesmas.</p>

##4.2. Declaração de posição do produto

<p align="justify">Na tabela a seguir é possível ver a posição do produto:</p>

<table style="width:100%">
  <tr>
    <td><b>Para</b></td>
    <td>Cidadãos e parlamentares do Brasil</td> 
  </tr>
  <tr>
    <td><b>Que</b></td>
    <td>Desejam ter mais praticidade e mobilidade no acesso a um sistema de análise e contribuição de projetos de leis</td> 
  </tr>
  <tr>
    <td><b>O</b></td>
    <td>WikilegisApp</td> 
  </tr>
   <tr>
    <td><b>Que</b></td>
    <td>Permite aos usuários debaterem entre si e proporem alterações nos projetos de leis</td> 
  </tr>
   <tr>
    <td><b>Ao contrário</b></td>
    <td>De outros meios de acompanhamento de projetos de leis</td> 
  </tr>
   <tr>
    <td><b>Nosso produto</b></td>
    <td>Permite que usuários, além de analisar os projetos, possam sugerir alterações nos artigos e debater com outros usuários.</td> 
  </tr>
</table>



##4.3. Recursos do produto

<p align="justify">O aplicativo Wikilegis oferece as seguintes funcionalidades ao usuário:</p>

* <p align="justify"><b>Gerenciar usuário:</b> Essa funcionalidade permite o usuário cadastrar, editar e visualizar o seu perfil.</p>

* <p align="justify"><b>Filtrar projetos:</b> Essa funcionalidade permite ao usuário filtrar projetos por data, relevância ou por status (aberto ou encerrado).</p>

* <p align="justify"><b>Avaliar artigo:</b> Essa funcionalidade permite o usuário avaliar um artigo de um projeto de lei em gostei ou não gostei.</p>

* <p align="justify"><b>Comentar:</b> Essa funcionalidade permite ao usuário comentar em artigos de propostas de leis ou em propostas feitas no artigo.</p>

* <p align="justify"><b>Sugerir proposta:</b> Essa funcionalidade permite ao usuário sugerir uma proposta de mudança em um projeto de lei.</p>

* <p align="justify"><b>Pesquisar projetos de lei:</b> Essa funcionalidade permite ao usuário pesquisar um projeto de lei.</p>

* <p align="justify"><b>Seguir projeto:</b> Essa funcionalidade permite ao usuário escolher receber notificações de um projeto por e-mail semanalmente ou diariamente.</p>


| Recurso| Benefícios|
| :---: | :---: |
| Gerenciar usuário| É possível que o usuário deixe o perfil com a suas características pessoais |
| Filtrar projetos| Tornar as leis de interesse do usuário mais fáceis de serem encontradas. |
| Avaliar artigo| O usuário faz valer seu direito de voz no aplicativo através de suas avaliações. |
| Sugerir proposta| O usuário poderá participar ativamente das discussões políticas do seu pais, podendo sugerir propostas. |
| Comentar proposta| Permite ao usuário se manter ativo em discussões, podendo expressar opinião quanto às elaborações dos projetos. |
| Seguir projeto| O usuário se mantém informado sobre a evolução de um projeto de lei , recebendo periodicamente notificação. |
| Pesquisar projeto| O usuário consegue encontrar o projeto de forma mais rápida e prática. |

#5.  Requisitos não funcionais

<p align="justify">Os requisitos não funcionais especificarão requisitos relacionados a: Usabilidade, Confiabilidade, Desempenho, Suportabilidade e Outros. Eles podem ser visualizados na <a href="https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Especifica%C3%A7%C3%A3o-suplementar">Especificação Suplementar</a>.
</p>

#6. Referências

<p align="justify">FONSECA, Jumária Fernandes Ribeiro. <strong>O Orçamento Participativo e a Gestão Democrática de Goiânia</strong>. Dissertação (Mestrado em Desenvolvimento e Planejamento Territorial). Programa de Pós-Graduação em Desenvolvimento e Planejamento Territorial da Universidade Católica de Goiás. Goiânia, 2009. Disponível em: http://www.portalconscienciapolitica.com.br/ciber-democracia/democracia-participativa/. Acesso em:  20 set. 2016.
</p>

<p align="justify">Agência Brasil, Celular é principal meio de acesso à internet no Brasil, mostra IBGE. Disponível em: http://agenciabrasil.ebc.com.br/economia/noticia/2016-04/celular-e-principal-meio-de-acesso-internet-na-maioria-dos-lares. Acesso em: 19 set. 2016
</p>

<p align="justify">Kantar Worldpanel, Smartphone OS sales market share. Disponível em: http://www.kantarworldpanel.com/global/smartphone-os-market-share/. Acesso em: 19 set. 2016
</p>