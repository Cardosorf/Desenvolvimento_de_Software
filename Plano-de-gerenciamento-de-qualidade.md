#1. Introdução

Este documento tem como objetivo especificar como será feito o controle de qualidade do produto de Software, documentação e produtividade dos membros presentes no projeto Wikilegis mobile. Para isso serão necessárias métricas que indiquem o _status_ do projeto, para que por sua vez os gerentes possam tomar decisões eficazes para que o projeto se mantenha dentro do tempo, custo e escopo planejados.

#2. Definições

Medir é atribuir valores à atributos de uma entidade, dessa forma podendo avaliar esta entidade de acordo com regras bem definidas, não dependendo diretamente de interpretações subjetivas. Sendo assim, medir, monitorar e controlar o projeto de software em sua fase de desenvolvimento é fundamental para garantir sua qualidade.[1] 

#3. Estratégias de controle de qualidade

A qualidade do projeto depende de muitas variáveis, por isso, várias estratégias diferentes devem ser tomadas a fim de assegurar a qualidade do produto.

##3.1. Treinamentos

A fim de garantir um certo nível de maturidade da equipe de desenvolvimento foram planejados treinamentos relacionados aos entregáveis do projeto.

##3.2 Inspeção e validação dos artefatos

Os documentação produzida na fase de iniciação e elaboração dos requisitos refletem o produto final, sendo assim, é necessário garantir que o artefatos estão de acordo com o esperado do ponto de vista dos steakholders. Estes são: Os gerentes(GPP) que fazem uma validação minuciosa e os couches (Monitores) que se espera uma assistência sobre duvidas que possam aparecer, já que são a referência de experiência de outros semestres na disciplinas.

Também serão feitas reuniões com o cliente para validar a corretude das informações levantadas nos requisitos. Essas reuniões podem ser vistas no [cronograma](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Cronograma).
(adicionar processo)

##3.3 Métricas de código

Métricas de código-fonte são importantes para garantir que o produto está sendo desenvolvido dentro dos padrões de qualidade pré-definidos. Todos os conceitos relacionados a métricas de código estão no [apêndice A](#Apêndice A) deste documento, atrás do plano de medição GQM (Goal, Question, Métric). Porque utilizar-se deste modelo de medição? Para garantir que a medição está dentro dos objetivos estratégicos do projeto. Isso ocorro através da arvores de rastreabilidade, que sempre mapeia a métrica com um objetivo. Isto torna mais fácil identificar métricas que não atendem mais as necessidades do projeto.

#4. Ferramentas

##4.1 Checkstyle

O Checkstyle é um plugin para a plataforma JetBrains IntelliJ IDEA, que promove ao usuário um feedback em tempo real para um determinado conjunto de regras de sintaxe de uma linguagem de programação. Este plugin verifica códigos escritos no formato _.java_ e gera _warnings_ na IDE em que é instalado, caso alguma regra de sintaxe não venha a ser rigorosamente seguida pelo programador.

O uso dessa ferramenta permitirá que o sistema seja implementado de forma padrão por todos desenvolvedores. Tal fato é importante ao stakeholder, pois não trabalham oficialmente com a linguagem de implementação do aplicativo, e seria um facilitador para eles que irão manter o aplicativo após o fim do projeto.

Mais informações podem ser encontradas nos links:

[CheckStyle Documentation](http://checkstyle.sourceforge.net/)

[Checkstyle Repository](https://github.com/jshiell/checkstyle-idea/blob/master/LICENCE)

[Checkstyle Addons](http://checkstyle-addons.thomasjensen.com/)

##4.2 JaCoCo

JaCoCo é um plugin do framework Gradle, integrado ao Android Studio, utilizado para gerar cobertura de testes unitários e testes de interface, dois dos principais tipos de testes que podem ser codificados na IDE utilizada pela equipe.

Esta ferramenta permitirá que a equipe acompanhe como estão sendo realizadas as funcionalidades e a quantidade de testes realizados por cada classe implementada. O JaCoCo, permite ainda, visualizar quais métodos não foram testados, e a quantidade de testes realizados por cada método.

##4.3 Espresso

O Espresso é uma ferramenta para Testes de Interface de Usuário da plataforma Android. Com tal ferramenta a equipe garante não realizar somente testes unitários na aplicação, permite verificar de forma automatizada a interação que um usuário teria com a interface do aplicativo. Garante, também, um aumento na cobertura de testes do projeto, visto que o método _**onCreate**_ das classes controladoras de interface não pode ser testado com testes unitários.

##4.4 Mezuro

O Mezuro é um ferramenta de análise de métricas de qualidade de código produzido pelo Centro de Competência em Software Livre (CCSL), da Universidade de São Paulo (USP). O Mezuro utiliza de duas outras ferramentas o Kalibro e o Analizo para calcular as métricas e análisá-las, para posteriomente mostrar as resultantes de código em seu portal.

A tabela abaixo, lista algumas das métricas colhidas pelo Mezuro, e que são relevantes à equipe para garantir a qualidade de implementação do software.

| Métrica (PT-BR) | Métrica (EN-US) | Código | Escopo da Métrica |
| --- | --- | --- | --- |
| Conexões Aferentes | Afferents Connections | acc | Acoplamento |
| Média da Complexidade Ciclomática | Average Cyclomatic Complexity | accm | Complexidade |
| Média do Tamanho dos Métodos | Average Method Lines of Code | amloc | Tamanho |
| Complexidade Estrutural | Structural Complexity | sc | Coesão |

### 4.4.1 Uma Breve Descrição das Métricas

#### 4.4.1.1 Conexões Aferentes:

#### 4.4.1.2 Complexidade Ciclomática:

#### 4.4.1.3 Tamanho dos Métodos:

#### 4.4.1.4 Complexidade Estrutural:


#X. Referências

[1] Carlos Morais de Oliveira Filho. **Kalibro: interpretação de métricas de código-fonte**, 2013, 89f, dissertação (Mestrado em Ciências), Instituto de Matemática e Estatística, Universidade de São Paulo.[URL.](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf)

#Apêndice A

#GQM (Goal, Question, Métric)

OBJETIVOS ESTRATÉGICOS

O.1 - Boas entregas

|Analisar| código|
|:---:|:---:|
|Com o propósito de|melhorar|
|Com respeito a|qualidade interna do software|
|Sobre o ponto de vista do|desenvolvedor|
|No contexto do |projeto wikilegis mobile|


O.2 - Dedicação constante

|Analisar|os desenvolvedores e os gerentes|
|:---:|:---:|
|Com o propósito de|monitorar|
|Com respeito ao|comprometimento da equipe|
|Sobre o ponto de vista do|docente|
|No contexto do| projeto de desenho wikilegis mobile|

QUESTÕES

|||
|---|---|
|**Foco na qualidade** <br/> **- Q.1.1** O produto apresenta uma boa manutenibilidade? <br/> **- Q.1.2** O produto apresenta uma boa usabilidade?|**Fatores de variação** <br/> - A produtividade não atender a expectativa; <br/> - Conhecimento da equipe limitado;|
|**Hipótese de baseline** <br/> - 30% de cobertura de teste até a primeira release; <br/> - 90% de cobertura de teste até a segunda release; <br/> - X de duplicação de código;<br/> - X de acoplamento;<br/> - X de coesão;<br/> - 0 discordâncias com a folha de estilo.|**Impacto das hipóteses de base line**<br/> - Baixa qualidade do produto de software;<br/> - Baixa manutenibilidade.|

MÉTRICAS

|Métrica|M.1.1.1|
|---|---|
|**Objetivo da Medição**|Garantir que o software tenha menor quantidade de defeitos possível dentro dos padrões escolhidos.|
|**Fórmula**| CoberturaTeste =nº de itens executados/total de itens do código <br/>item = instruções de código, ramificações de código, caminhos de código.|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada commit.|
|**Procedimentos**| Análise com auxílio de software com análise estática de código. A ferramenta Utiliza dois dados extraidos do código para realizar esta medição: Número de linhas testadas e número de linhas do projeto. Além disse também será mantido junto com as outras métricas numa tabela para acompanhar melhora da métrica.|
|**Análise**| Primeira release:<br/> “Dentro do esperado” dado por CoberturaTeste > 30%<br/>“fora do planejado” dado por CoberturaTeste < 30% <br/> Segunda release: <br/> “Dentro do esperado” dado por CoberturaTeste > 90%<br/>“fora do planejado” dado por CoberturaTeste < 90%|
|**Providências**| Caso a métrica esteja abaixo do esperado na primeira release, em qualquer uma das interações que envolvam desenvolvimento, a equipe de gerência deve ser alertada e o coach(Monitor) deve ser procurado em caso de dificuldades.<br/> Caso a métrica esteja abaixo do esperado na segunda release, na primeira semana a equipe de desenvolvimento deve ser alertada. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando do desenvolvimento de testes|
