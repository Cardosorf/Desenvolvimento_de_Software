### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 25/08/2016 | 1 | Elaboração Inicial | Lucas Brilhante |
| 28/08/2016 | 1.1 | Introdução e conceitos | Lucas Brilhante |
| 31/08/2016 | 1.2 | Elaboração do GQM | Lucas Brilhante |
| 01/09/2016 | 1.3 | Descrição das ferramentas | Lucas Brilhante |
| 04/09/2016 | 1.4 | Refinamento dos conceitos | Lucas Brilhante |
| 04/09/2016 | 1.4 | Descrição das ferramentas | Pedro Ivo |
| 05/09/2016 | 1.5 | Revisão bibliográfica | Lucas Brilhante |
| 05/09/2016 | 1.6 | Escolha de métricas | Lucas Brilhante |
| 05/09/2016 | 1.7 | Análise das métricas | Lucas Brilhante |
| 06/09/2016 | 1.8 | Atualizando métricas | Lucas Brilhante |
| 09/09/2016 | 1.9 | Atualizando Análise de métricas na tabela GQM | Pedro Ivo
| 15/09/2016 | 2.0 | Atualizando ferramentas | Lucas Brilhante |
| 15/09/2016 | 2.1 | Formatação e histórico de versão | Lucas Brilhante |
| 17/09/2016 | 2.2 | Adicionando referência de indicadores | Lucas Brilhante |
| 20/09/2016 | 2.3 | Correções apontadas pela monitora | Lucas Brilhante |

# Sumário

1.  [Introdução](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#1-introdu%C3%A7%C3%A3o)
   *  [Métricas de software](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#11-m%C3%A9tricas-de-software)
   *  [Métricas de software](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#12-por-que-medir)
2.  [Estratégias de controle de qualidade](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#2-estrat%C3%A9gias-de-controle-de-qualidade)
   *  [Inspeção e validação dos artefatos](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#21-inspe%C3%A7%C3%A3o-e-valida%C3%A7%C3%A3o-dos-artefatos)
   *  [Métricas de código](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#22-m%C3%A9tricas-de-c%C3%B3digo)
3.  [Ferramentas](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#3-ferramentas)
   * [3.1.  Checkstyle](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#31-checkstyle)
   * [3.2.  JaCoCo](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#32-jacoco)
   * [3.3.  Espresso](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#33-espresso)
   * [3.4.  Analizo](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#34-analizo)
4.  [Referências](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#4-refer%C3%AAncias)
5.  [GQM](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#gqm-goal-question-m%C3%A9tric)


#1. Introdução

<p align="justify">Este documento tem como objetivo especificar como será feito o controle de qualidade do produto de Software e artefatos relacionados presentes no projeto Wikilegis mobile. Para que o monitoramento e controle aconteça é necessário adquirir dados que indiquem características relevantes, para que por sua vez os gerentes possam tomar decisões eficazes para que o projeto se mantenha dentro do tempo, custo e escopo planejados.</p>

##1.1. Métricas de software
<p align="justify">Métricas são compostas por procedimentos de medição e escalas de medidas (ISO/IEC9126-1)[2].
Métricas de software lidam com a medição do produto de software, isto é, código, documentação e o processo de desenvolvimento. Os dados obtidos desse processo de medição são então analisados e modelados, podendo então serem usados para estimar custo e prazos, bem como medir a produtividade e a qualidade de software. (1988, Mills) </p>

<p align="justify"> De acordo com Mills[1], boas métricas não devem apenas descrever o produto ou o processo de software, mas além disso, facilitar o desenvolvimento de modelos de predição do processo de desenvolvimento. Assim, o ideal é que as métricas possam ser:</p>
* Simples e calculadas de forma precisa. Deve ser claro como a métrica é coletada.
* Objetiva, ou seja, deve atender um objetivo do projeto.
* apresentar uma boa relação custo-benefício.
* Válida, isto é, deve medir o que foi determinada a medir.
* Robusta - Relativamente insensível a mudanças insignificantes no produto ou processo.

##1.2. Por que medir?

<p align="justify">Nos anos 90 a indústria de software crescia a um ritmo assustador. Até então 50% de toda a industria empregadora já contava com a industria de software. Mas apesar do crescimento a dela, ainda apresentava grandes problemas. Dentre eles estavam: Estimativa de custo e prazo absurdamente imprecisos; Baixa qualidade de software, com baixos níveis de confiabilidade e; a produtividade dos times não crescia tanto quanto a demanda de novos softwares. (1988, Mills) 

Para "resolver" a crise era necessário melhorar as estimativas de prazo e custo, melhorar a qualidade do software e aumentar a produtividade. Acontece que isso pode ser alcançado através de uma gerência de projetos mais eficaz, que por sua vez, pode ser alcançado por um melhor uso das métricas. (1988, Mills)</p>

#2. Estratégias de controle de qualidade

<p align="justify">A fim de assegurar a qualidade do produto de software e seu desenvolvimento foram adotadas as seguintes estratégias.</p>

##2.1 Inspeção e validação dos artefatos

<p align="justify">As documentações produzidas na fase de iniciação e elaboração do processo unificado te, grande foco na produção dos requisitos refletem o produto final, sendo assim, é necessário garantir que o artefatos estão de acordo com o esperado do ponto de vista de todos os stakeholders. </p>

* Os gerentes(GPP) devem ler e fazer uma validação nos artefatos produzidos por eles e pela equipe de desenvolvimento(MDS).
* Os coaches (Monitores) são responsáveis por ajudar a equipe com dúvidas na documentação. Essas dúvidas podem surgir na hora da produção ou da validação.
* O cliente (Desenvolvedores do wikilegis) - São marcadas reuniões para validar a corretude dos artefatos gerados de acordo com a expectativa deles. 

Pode-se ver estas reuniões no [cronograma](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Cronograma).

##2.2 Métricas de código

<p align="justify">"Métricas de código-fonte são aquelas obtidas através da análise do código-fonte."[3]. E código-fonte é “qualquer descrição completamente executável de um sistema de software”[4]. Métricas de código serão sempre importante, pois ele é a unica representação precisa do comportamento do sistema [4]. E não se engane, ele se tornará cada vez mais importante, pois cada vez mais o software se torna essencial na sociedade [4]. Mas não se precipite, nem tudo vale a pena ser medido. Deve-se escolher com cuidado o que vai ser medido e assim, garantir a qualidade desejada.[4]
Para escolher as métricas do contexto do Wikilegis mobile foi feito um plano GQM, afim de definir os objetivos da medição e assim poder definir uma rastreabilidade, e no futuro poder identificar medições que se tornarem obsoletas.</p>
[Plano GQM](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade#gqm-goal-question-m%C3%A9tric)

#3. Ferramentas

##3.1 Checkstyle

<p align="justify">O Checkstyle é um plugin para a plataforma JetBrains IntelliJ IDEA, que promove ao usuário um feedback em tempo real para um determinado conjunto de regras de sintaxe de uma linguagem de programação. Este plugin verifica códigos escritos no formato java e gera warnings na IDE em que é instalado, caso alguma regra de sintaxe não venha a ser rigorosamente seguida pelo programador.

O uso dessa ferramenta permitirá que o sistema seja implementado de forma padrão por todos desenvolvedores. Tal fato é importante ao stakeholder, pois não trabalham oficialmente com a linguagem de implementação do aplicativo, e seria um facilitador para eles que irão manter o aplicativo após o fim do projeto.</p>

Mais informações podem ser encontradas nos links:

[CheckStyle Documentation](http://checkstyle.sourceforge.net/)

[Checkstyle Repository](https://github.com/jshiell/checkstyle-idea/blob/master/LICENCE)

[Checkstyle Addons](http://checkstyle-addons.thomasjensen.com/)

##3.2 JaCoCo

<p align="justify">JaCoCo é um plugin do framework Gradle, integrado ao Android Studio, utilizado para gerar cobertura de testes unitários e testes de interface, dois dos principais tipos de testes que podem ser codificados na IDE utilizada pela equipe.

Esta ferramenta permitirá que a equipe acompanhe como estão sendo realizadas as funcionalidades e a quantidade de testes realizados por cada classe implementada. O JaCoCo, permite ainda, visualizar quais métodos não foram testados, e a quantidade de testes realizados por cada método.</p>

##3.3 Espresso

<p align="justify">O Espresso é uma ferramenta para Testes de Interface de Usuário da plataforma Android. Com tal ferramenta a equipe garante não realizar somente testes unitários na aplicação, permite verificar de forma automatizada a interação que um usuário teria com a interface do aplicativo. Garante, também, um aumento na cobertura de testes do projeto, visto que o método onCreate das classes controladoras de interface não pode ser testado com testes unitários.</p>

##3.4 Analizo

<p align="justify">Analizo Metrics é uma ferramenta escrita em Perl que faz uso de extratores para analisar código-fonte.[3] 

A tabela abaixo, lista algumas das métricas colhidas pelo Analizo, e que são relevantes à equipe para garantir a qualidade de implementação do software.</p>

| Métrica (PT-BR) | Métrica (EN-US) | Código | Escopo da Métrica |
| --- | --- | --- | --- |
| Conexões Aferentes | Afferents Connections | acc | Acoplamento |
| Acoplamento entre objetos | Coupling between objects| cbo| Acoplamento|
| Média da Complexidade Ciclomática | Average Cyclomatic Complexity | accm | Complexidade |
| Média do Tamanho dos Métodos | Average Method Lines of Code | amloc | Tamanho |
| Falta de coesão entre entre dos métodos|Lack of coesion of methods| LCoM4|Coesão|

#4. Referências

[1] Mill, Everald E. **Software Métrics**. SEI - Carnegie Mellon University, 1988. [Link](http://www.sei.cmu.edu/reports/88cm012.pdf)

[2]ISO/IEC9126-1(2001) ISO/IEC9126-1. **Software engineering – product quality – part 1: Quality model.** International Organization for Standardization and International Electrotechnical Com-
mission. [Link.](http://luizcamargo.com.br/arquivos/NBR%20ISO_IEC%209126-1.pdf)

[3] Filho, Carlos Morais de Oliveira Filho **Kalibro: interpretação de métricas de código-fonte**, 2013, 89f, dissertação (Mestrado em Ciências), Instituto de Matemática e Estatística, USP. [Link.](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf)

[4] Harman(2010) Mark Harman. **Why source code analysis and manipulation will always be important**. Em 10th IEEE Working Conference on Source Code Analysis and Manipulation (SCAM). [Link.](http://www0.cs.ucl.ac.uk/staff/mharman/scam10.pdf)

[5] McCabe(1976) Thomas J. McCabe. **A complexity measure**. IEEE Transactions on Software Engineering. [Link.](http://www.literateprogramming.com/mccabe.pdf)

[6] Analizo: **an Extensible Multi-Language Source Code Analysis and Visualization Toolkit**, by Antonio Terceiro , Joenio Costa , João Miranda, Paulo Meirelles, Luiz Romário Rios, Lucianna Almeida, Christina Chavez, and Fabio Kon. Paper published in the Tools Session of the 1st Brazilian Conference on Software, September 2010. Describes analizo, its architecture and research work using analizo. [Link](http://www.analizo.org/publications/analizo-cbsoft2010-tools.pdf)

[7] Meirelles(2013) Paulo Roberto Miranda Meirelles. **Monitoramento de métricas de código-fonte em projetos de software livre**. Tese de Doutorado, Universidade de São Paulo. [Link.](https://social.stoa.usp.br/articles/0030/6046/tesePauloMeirelles.pdf)

[8] Pereira (2015) Marcos Ronaldo Pereira Junior. **Estudo de métricas do código fonte no sistema Android e seus aplicativos**. Trabalho de termino de curso, Universidade de Brasilia [Link](http://bdm.unb.br/bitstream/10483/11317/1/2015_MarcosRonaldoPereiraJunior.pdf)

#Apêndice A

#GQM (Goal, Question, Métric)

##OBJETIVOS ESTRATÉGICOS

O.1 - Qualidade do produto

<p align="justify">Visto que o software em produção será mantido pela equipe do Wikilegis da Câmera dos deputados, e que eles não possuem conhecimento da linguagem, temos que priorizar fazer um software com alta manutenibilidade, para que o cliente não tenha problemas em mantê-lo. Isto é, um produto de software documentado, altamente padronizado e com bons indicadores de orientação a objeto. Maior foco será na parte de padronização de código (Folha de estilo) e bons indicadores de orientação a objeto, que serão evidenciados nesse GQM. Dito isso, podemos concluir que o objetivo, nos padrões do GQM é:</p>

|Analisar|código|
|:---:|:---:|
|Com o propósito de|melhorar|
|Com respeito a|Manutenibilidade do software|
|Sobre o ponto de vista do|desenvolvedor|
|No contexto do |projeto wikilegis mobile|

##QUESTÕES

|||
|:---:|:---:|
|**Foco na qualidade** <br/> **- Q.1.1** O produto apresenta uma boa manutenibilidade? <br/> **- Q.1.2** O produto é confiável?|**Fatores de variação** <br/> - A produtividade não atender a expectativa; <br/> - Conhecimento da equipe limitado;|
|**Hipótese de baseline** <br/> - 30% de cobertura de teste até a primeira release; <br/> - 90% de cobertura de teste até a segunda release; <br/>Falta de coesão <br/> - 0 - 2 de acoplamento;|**Impacto das hipóteses de base line**<br/> - Baixa qualidade do produto de software;<br/> - Baixa manutenibilidade.|

##MÉTRICAS

<p align="justify">Para analise das métricas, fixando um indicador, será utilizado o conceito apresentado por Meirelles[7](2013), em que os dados serão comparados no percentil 75%, onde as curva normal começa a apresentar resultados relevantes, dado que muitos dados não atrapalham o calculo da métrica. Em alguns casos classes com métricas 0, não são desejáveis para a análise. Por isso será utilizado o valor "upper" das métricas da ferramenta analizo.
Outro ponto importante para a análise de métricas é o artigo apresentado por Pereira(2015), onde é analisado o código fonte da API de desenvolvimento de várias versões do android. Este valores serão considerados valores ideais para a análise do código fonte da aplicação Wikilegis mobile. </p>

|Métrica|M.1.1.1 - Cobertura de teste|
|---|---|
|**Objetivo da Medição**|Garantir que o software não contenha erros de lógica ou digitação, assim tendo uma garantia de qualidade.|
|**Descrição**|A cobertura de deste é dada pela proporção entre linhas testadas e a quantidade total de linhas de código. A cobertura de código é importante para acompanhar o andamento dos desenvolvimento dos testes. Testes estes que garantem a qualidade e um error mínimo de erros de desenvolvimento.|
|**Fórmula**|Cobertura = Linhas testadas / Linhas totais|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação.<br/>Ferramenta: JaCoCo|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| Primeira release:<br/> “Dentro do esperado” dado por CoberturaTeste > 30%<br/>“fora do planejado” dado por CoberturaTeste < 30% <br/> Segunda release: <br/> “Dentro do esperado” dado por CoberturaTeste > 90%<br/>“fora do planejado” dado por CoberturaTeste < 90%|
|**Providências**| Caso a métrica esteja abaixo do esperado na primeira release, em qualquer uma das interações que envolvam desenvolvimento, a equipe de gerência deve ser alertada e o coach(Monitor) deve ser procurado em caso de dificuldades.<br/> Caso a métrica esteja abaixo do esperado na segunda release, na primeira semana a equipe de desenvolvimento deve ser alertada apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando do desenvolvimento de testes|

|Métrica|M.1.1.2 - Complexidade ciclomática média (ACCM)|
|---|---|
|**Objetivo da Medição**|Garantir a manutenibilidade do código, garantindo que o cliente será capaz de evoluir o código.|
|**Descrição**|Complexidade ciclomática é o número de caminhos independentes dentro do grafo de nós dentro do sistema. Cada nó é um bloco de código sequencial do sistema.<br/>De forma resumida e sucinta, complexidade ciclomática equivale ao número de desvios (ou estruturas condicionais) mais 1. Como a coleta consiste em contar o número de condicionais, a métrica também é chamada de complexidade condicional. Ela indica o número de testes que o fragmento de software precisa ter para cobrir todos caminhos linearmente independentes de execução.[5]|
|**Fórmula**|V(G) = e - n + p<br/>Onde V(G) é a complexidade ciclomática, n = vertice, e = aresta, p = componentes conectados<br/> A média estão é feita, M(V(G)), dando a complexidade ciclomática média por metodo.|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Analizo|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| De acordo com a ferramenta [Mezuro](http://mezuro.org/pt/kalibro_configurations/1/metric_configurations/2), baseado em conhecimentos empiricos:<br/> 0 - 3 Exelente <br/> 3 - 5 Bom (Esperado)<br/> 5 - 7 Regular <br/> 7 - INF Preocupante <br/>|
|**Providências**|Caso a métrica esteja acima do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.3 - Conexões Aferentes por classe média(ACC)|
|---|---|
|**Objetivo da Medição**|Garantir a manutenibilidade do código, garantindo que o cliente será capaz de evoluir o código (Acoplamento).|
|**Descrição**|Digamos q a classe Ca acessa a classe Cb. Podemos dizer que a classe Ca é cliente da classe fornecedora Cb e denotamos Ca => Cb. Considerando Ci != Cj e Ci => Cj, então cliente(Ci,Cj) = 1, se não cliente(Ci,Cj) = 0. Então ACC = Somatório, de 1 até n,cliente(Ci,C), onde n = ao numero total de classes do sistema e C a classe em que se está calculando. Essa métrica indica, se apresentar um grande valor, que o sistema é de difícil manutenção, pois, será qualquer mudança provavelmente afetará outras partes do sistema.(Meirelles, 2013)[7].Quanto menor o acoplamento melhor.|
|**Fórmula**|![formula 1](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.png)<br/>![formula 2](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.1.png)|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Analizo|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit da interação para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar a evolução do software.|
|**Análise dos indicadores**| 0 - 2 Bom (Esperado)<br/> 2 - 20 Regular <br/> 20 - INF Ruim [7] <br/> Segundo [FILHO](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf), caso a métrica atinja valores muito altos [5,7] a classe possui muitas dependências, sendo necessário seguir o princípio da depêndencia única e reduzir o número de interfaces utilizadas.|
|**Providências**| Caso a métrica esteja acima do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.3 - Conexões Aferentes por classe média(ACC)|
|---|---|
|**Objetivo da Medição**| Garantir que não há dependências demais entre classes, diminuindo o esforço de manutenção (Acoplamento).|
|**Descrição**|Digamos q a classe Ca acessa a classe Cb. Podemos dizer que a classe Ca é cliente da classe fornecedora Cb e denotamos Ca => Cb. Considerando Ci != Cj e Ci => Cj, então cliente(Ci,Cj) = 1, se não cliente(Ci,Cj) = 0. Então ACC = Somatório, de 1 até n,cliente(Ci,C), onde n = ao numero total de classes do sistema e C a classe em que se está calculando. Essa métrica indica, se apresentar um grande valor, que o sistema é de difícil manutenção, pois, será qualquer mudança provavelmente afetará outras partes do sistema.(Meirelles, 2013)[7].Quanto menor o acoplamento melhor.|
|**Fórmula**|![formula 1](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.png)<br/>![formula 2](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.1.png)|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Analizo|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit da interação para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar a evolução do software.|
|**Análise dos indicadores**| 0 - 2 Bom (Esperado)<br/> 2 - 20 Regular <br/> 20 - INF Ruim [7] <br/> Segundo [FILHO](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf), caso a métrica atinja valores muito altos [5,7] a classe possui muitas dependências, sendo necessário seguir o princípio da depêndencia única e reduzir o número de interfaces utilizadas.|
|**Providências**| Caso a métrica esteja acima do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.4 - Fator de acoplamento (cof)|
|---|---|
|**Objetivo da Medição**| Garantir que não há dependências demais entre classes, diminuindo o esforço de manutenção (Acoplamento).|
|**Descrição**| Esta métrica utiliza a acc para realizar o calculo do indicador. A cof indica o quanto o software está acoplado, levando em consideração também o numero de |
|**Fórmula**|Não se aplica|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Analizo|
|**Procedimentos**| Será feito o uso da ferramenta no último commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**|De acordo com Pereira[8], O valor ideal é 1. Mas valores além disso não são estranhos. Considerando o escopo do projeto, valores aceitáveis serão:<br/>1-3 Aceitável<br/>4-INF Ruim|
|**Providências**|Caso a métrica esteja acima do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|
|Métrica|M.1.1.6 - Tamanho médio dos Métodos (AMLOC)|
|---|---|
|**Objetivo da Medição**|Garantir que a atomicidade dos métodos, isto é, executam somente uma tarefa, facilitando o desenvolvimento de testes.|
|**Descrição**|"Essa medida indica se o código está bem distribuido entre os métodos."(Meirelles)[7] É melhor métodos que são pequenos e bem definidos no que fazem. Essa métrica é obtida através da contagem simples do número de linhas com operações (Não brancas) e em seguida é feita a média entre as classes.|
|**Fórmula**|Não se aplica|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Analizo|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise e indicadores**| De acordo com Meirelles[7]:<br/>AMLOC <= 10 - Bom (Esperado) <br/>10 > AMLOC <= 13 Regular AMLOC >13 Ruim <br/> Segundo [FILHO](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf), caso a métrica atinja valores elevados [5,7] faz se necessário "quebrar" métodos grandes em métodos menores, e também, códigos muito aninhados são fortes candidatos a um novo método.|
|**Providências**|Caso a métrica esteja acima do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|


