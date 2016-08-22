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
 1. [Usabilidade](#51-usabilidade)
 2. [Confiabilidade](#52-confiabilidade)
 3. [Desempenho](#53-desempenho)
 4. [Suportabilidade](#54-suportabilidade)
 5. [Outros](#55-outros)
     1. [Licença, Segurança e Instalação](#551-licença-segurança-e-instalação)

***

#1  Introdução

Este documento apresenta uma visão geral do projeto, definindo as necessidades, características e requisitos do sistema. 

##1.1 Objetivos

Os objetivos deste documento são auxiliar na obtenção de informações dos usuários a cerca do aplicativo WikilegisApp,  do projeto ajudar a equipe desenvolvedora a ter uma visão alinhada sobre o escopo, melhorar a avaliação do desenvolvimento do software e validar com o cliente a visão da equipe de desenvolvimento acerca do aplicativo.

##1.2 Visão geral da solução

Na tabela a seguir, é mostrado um resumo acerca do problema e da solução apresentada.

<table style="width:100%">
  <tr>
    <td><b>O problema da</b></td>
    <td>Difícil comunicação entre a população e seus representantes políticos,</td> 
  </tr>
  <tr>
    <td><b>Afeta</b></td>
    <td>A elaboração de leis que não correspondem às reais necessidades da população,</td> 
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

#2  Descrição do usuário

Como o aplicativo traz uma oportunidade de políticos apresentarem suas propostas de lei, criadas na plataforma web do Wikilegis, e dos cidadãos poderem analisar e contribuir com elas, os usuários serão em sua maioria, cidadãos e políticos brasileiros.

##2.1 Usuário

| Tipo | Descrição | Principais Responsabilidades |
| :---: | :---: | --- |
|Cidadão|Cidadãos brasileiros.|Fiscalizar e colaborar com as leis propostas por parlamentares.|
|Parlamentar|Representantes legais da população.|Acompanhar as sugestões para suas propostas de lei.|


##2.2 Principais necessidades do usuário

| Necessidade | Problema | Solução atual | Solução proposta |
| :---: | :---: | :---: | :---: |
|O usuário tem a necessidade de analisar e contribuir com os projetos de leis.|A dificuldade de alcançar os políticos para se fazer sugestões em projetos de lei de forma prática, acessível e que permita mobilidade.|Um sistema web que possibilita ao usuário analisar e contribuir com os projetos de leis propostos pelos deputados.|Um sistema mobile que possibilita ao usuário analisar e contribuir com os projetos de leis propostos pelos deputados.|
|O usuário tem a necessidade de acompanhar o debate da sociedade acerca de seus projetos de lei.|A dificuldade de alcançar os cidadãos de uma maneira prática para receber sugestões acerca de seus projetos de lei.|Um sistema web que possibilita ao usuário expor projetos de leis para debate com a sociedade.|Um sistema mobile que possibilita ao usuário expor projetos de leis para debate com a sociedade.|

##2.3 Ambiente do usuário

Para que o usuário possa usar o aplicativo com maior mobilidade e para que ele atinja uma gama maior de usuários, visto que 80,4% (IBGE) dos usuários de internet no Brasil em 2016 já utilizam smartphones para acesso e 91,8% (Kantar) destes usuários utilizavam o sistema operacional Android até 2015, o sistema será desenvolvido para o sistema operacional Android, esperando-se que o usuário possua um telefone celular com este sistema, e que o mesmo possua acesso à internet.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/imageVisao1.png)

##2.4 Alternativas e competição

Nesta seção serão descritos os principais produtos semelhantes encontrados encontrados.

###2.4.1 Plataforma web Wikilegis

O uso de celular para acessar a internet ultrapassou, de acordo com o IBGE em 2016, o do computador pela primeira vez no Brasil, com esta grande crescente de utilização de internet no celular está surgindo cada vez mais a necessidade de fazer plataformas mobiles de diversas aplicações. O versão mobile Wikilegis trás consigo a mudança de plataforma, entretanto tem exatamente as mesmas  funcionalidades da plataforma web Wikilegis.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/imageVisao2.png)

###2.4.2 SigaLei

Trata-se de um aplicativo informativo que tem como principal objetivo, mostrar as leis que estão em trâmite de aprovação no Congresso nacional e assembleias de Minas Gerais. Os usuários podem acompanhar as discussões a respeito das leis e ser informado das atualizações de projetos de leis do seu interesse.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao3.png)

###2.4.3 Monitora, Brasil!

Monitora, Brasil é um aplicativo para Android que possibilita a qualquer pessoa pesquisar e monitorar o que os Deputados Federais estão fazendo na Câmara dos Deputados. Com ele, é possível verificar a assiduidade, os projetos propostos, rankings, Twitter e outras informações.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao4.png)

###2.4.4 Infoleg

Aplicativo com informações das atividades legislativas da Câmara dos Deputados, com informações sobre deputados, projetos de lei e outras proposições, sessões no plenário, reuniões nas comissões e legislação.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/ImageVisao5.png)

#3  Envolvidos

#4  Visão geral do produto

O aplicativo tem por funcionalidade principal, a contribuição e interação de usuários com as propostas de leis dos parlamentares.

Usuários cadastrados podem curtir ou descurtir um artigo ou comentário de uma proposta de lei, sugerir uma alteração no artigo de uma proposta de lei, comentar em artigos de propostas de lei e escolher receber notificações via e-mail a respeito de alterações em um projeto. Já os usuários não cadastrados, poderão apenas visualizar as informações e comentários dos projetos de leis.

##4.1 Perspectiva do produto

Tem por expectativa que o aplicativo fomente o interesse do cidadão brasileiro em verificar quais as leis estão em trâmite para serem aprovados, podendo assim, contribuir com as mesmas.

##4.2 Declaração de posição do produto

Na tabela a seguir é possível ver a posição do produto:

##4.3 Recursos do produto

O aplicativo Wikilegis oferece as seguintes funcionalidades ao usuário:

* **Gerenciar usuário:** Essa funcionalidade permite o usuário cadastrar, editar e visualizar o seu perfil.

* **Filtrar projetos:** Essa funcionalidade permite ao usuário filtrar projetos por data, relevância ou por status (aberto ou encerrado).

* **Avaliar artigo:** Essa funcionalidade permite o usuário avaliar um artigo de um projeto de lei em gostei ou não gostei.

* **Comentar:** Essa funcionalidade permite ao usuário comentar em artigos de propostas de leis ou em propostas feitas no artigo.

* **Sugerir proposta:** Essa funcionalidade permite ao usuário sugerir uma proposta de mudança em um projeto de lei.

* **Pesquisar projetos de lei:** Essa funcionalidade permite ao usuário pesquisar um projeto de lei.

* **Seguir projeto:** Essa funcionalidade permite ao usuário escolher receber notificações de um projeto por e-mail semanalmente ou diariamente.


#5  Requisitos não funcionais

##5.1 Usabilidade

Em caso de erro, o aplicativo deverá apresentar mensagens de fácil entendimento, para ajudar o usuário a identificar o problema.

##5.2 Confiabilidade

O aplicativo deve funcionar 24 horas por dia , 7 dias na semana. Além disso, não deve haver erro nas informações apresentadas sobre as leis.

##5.3 Desempenho

##5.4 Suportabilidade

O sistema deverá ser suportado pelo sistema operacional Android versão 4.4 (KitKat) ou superior.

Para o funcionamento correto do aplicativo, é necessário que o dispositivo mobile possua acesso à internet para poder interagir com a plataforma do wikilegis, que é de onde provém as informações dinâmicas.

##5.5 Outros

###5.5.1 Licença, Segurança e Instalação

 O aplicativo deverá ser instalado através do aplicativo Google Play. Deve-se deixar claro ao usuário que o sistema será seguro, não causando danos ao celular do usuário, além disso, as informações pessoais do usuário devem ser confidenciais.
