#1. Introdução

Este documento tem como objetivo especificar como será feito o controle de qualidade do produto de Software e artefatos relacionados presentes no projeto Wikilegis mobile. Para que o monitoramento e controle aconteça é necessário adquirir dados que indiquem características relevantes, para que por sua vez os gerentes possam tomar decisões eficazes para que o projeto se mantenha dentro do tempo, custo e escopo planejados.

#2. Definições

##2.1. Métricas de software
Métricas são compostas por procedimentos de medição e escalas de medidas (ISO/IEC9126-1)[2].
Métricas de software lida com a medição do produto de software, isto é, código, documentação e o processo de desenvolvimento. Os dados obtidos desse processo de medição são então analisados e modelados, podendo então serem usados para estimar custo e prazos, bem como medir a produtividade e a qualidade de software. (1988, Mills) 

De acordo com Mills[1], boas métricas não devem apenas descrever o produto ou o processo de software, mas além disso, facilitar o desenvolvimento de modelos de predição do processo de desenvolvimento. Assim, o ideal é que as métricas possam ser:
* Simples e calculadas de forma precisa. Deve ser claro como a métrica é coletada.
* Objetiva, ou seja, deve atender um objetivo do projeto.
* apresentar uma boa relação custo-benefício.
* Valida, isto é, deve medir o que foi determinada a medir.
* Robusta - Relativamente insensível a mudanças insignificantes no produto ou processo.

##2.2. Por que medir?

Nos anos 90 a industria de software crescia a um ritmo assustador. Até então 50% de toda a industria empregadora já contava com a industria de software. Mas apesar do crescimento a industria de software ainda apresentava grandes problemas. Dentre eles estavam: Estimativa de custo e prazo absurdamente imprecisos; Baixa qualidade de software, com baixos níveis de confiabilidade e; a produtividade dos times não crescia tanto quanto a demanda de novos softwares. (1988, Mills) 

Para "resolver" a crise era necessário melhorar as estimativas de prazo e custo, melhorar a qualidade do software e aumentar a produtividade. Acontece que isso pode ser alcançado através de uma gerência de projetos mais eficaz, que por sua vez, pode ser alcançado por um melhor uso das métricas. (1988, Mills)

#3. Estratégias de controle de qualidade

A fim de assegurar a qualidade do produto de software e seu desenvolvimento foram adotadas as seguintes estratégias.

##3.1 Inspeção e validação dos artefatos

Os documentação produzida na fase de iniciação e elaboração do processo unificado te, grande foco na produção dos requisitos refletem o produto final, sendo assim, é necessário garantir que o artefatos estão de acordo com o esperado do ponto de vista de todos os steakholders. 

* Os gerentes(GPP) devem ler e fazer uma validação nos artefatos produzidos por eles e pela equipe de desenvolvimento(MDS).
* Os couches (Monitores) são responsáveis por ajudar a equipe com dúvidas na documentação. Essas dúvidas podem surgir na hora da produção ou da validação.
* O cliente (Desenvolvedores do wikilegis) - São marcadas reuniões para validar a corretude dos artefatos gerados de acordo com a expectativa deles. 

Pode-se ver estas reuniões no [cronograma.](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Cronograma).

##3.2 Métricas de código

"Métricas de código-fonte são aquelas obtidas através da análise do código-fonte."[3]. E código-fonte é “qualquer descrição completamente executável de um sistema de software”[4]. Métricas de código serão sempre importante, pois ele é a unica representação precisa do comportamento do sistema [4]. E não se engane, ele se tornará cada vez mais importante, pois cada vez mais o software se torna essencial na sociedade [4]. Mas não se precipite, nem tudo vale a pena ser medido. Deve-se escolher com cuidado o que vai ser medido e assim, garantir a qualidade desejada.[4]
Para escolher as métricas do contexto do Wikilegis mobile foi feito um plano [GQM](#Apêndice A), afim de definir os objetivos da medição e assim poder definir uma rastreabilidade, e no futuro poder identificar medições que se tornarem obsoletas.

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

O Mezuro é um ferramenta de análise de métricas de qualidade de código produzido pelo Centro de Competência em Software Livre (CCSL), da Universidade de São Paulo (USP). O Mezuro utiliza de duas outras ferramentas o Kalibro e o Analizo para calcular as métricas e análisá-las, para posteriomente mostrar as resultantes de código em seu portal.[3]

A tabela abaixo, lista algumas das métricas colhidas pelo Mezuro, e que são relevantes à equipe para garantir a qualidade de implementação do software.

| Métrica (PT-BR) | Métrica (EN-US) | Código | Escopo da Métrica |
| --- | --- | --- | --- |
| Conexões Aferentes | Afferents Connections | acc | Acoplamento |
| Média da Complexidade Ciclomática | Average Cyclomatic Complexity | accm | Complexidade |
| Média do Tamanho dos Métodos | Average Method Lines of Code | amloc | Tamanho |
| Complexidade Estrutural | Structural Complexity | sc | Coesão |


#5. Referências

[1] Mill, Everald E. **Software Métrics**. SEI - Carnegie Mellon University, 1988. [Link](http://www.sei.cmu.edu/reports/88cm012.pdf)

[2]ISO/IEC9126-1(2001) ISO/IEC9126-1. **Software engineering – product quality – part 1: Quality model.** International Organization for Standardization and International Electrotechnical Com-
mission. [Link.](http://luizcamargo.com.br/arquivos/NBR%20ISO_IEC%209126-1.pdf)

[3] Filho, Carlos Morais de Oliveira Filho **Kalibro: interpretação de métricas de código-fonte**, 2013, 89f, dissertação (Mestrado em Ciências), Instituto de Matemática e Estatística, USP. [Link.](http://www.teses.usp.br/teses/disponiveis/45/45134/tde-25092013-142158/publico/dissertacao.pdf)

[4] Harman(2010) Mark Harman. **Why source code analysis and manipulation will always be important**. Em 10th IEEE Working Conference on Source Code Analysis and Manipulation (SCAM). [Link.](http://www0.cs.ucl.ac.uk/staff/mharman/scam10.pdf)

[5] McCabe(1976) Thomas J. McCabe. **A complexity measure**. IEEE Transactions on Software Engineering. [Link.](http://www.literateprogramming.com/mccabe.pdf)

[6] Analizo: **an Extensible Multi-Language Source Code Analysis and Visualization Toolkit**, by Antonio Terceiro , Joenio Costa , João Miranda, Paulo Meirelles, Luiz Romário Rios, Lucianna Almeida, Christina Chavez, and Fabio Kon. Paper published in the Tools Session of the 1st Brazilian Conference on Software, September 2010. Describes analizo, its architecture and research work using analizo. [Link](http://www.analizo.org/publications/analizo-cbsoft2010-tools.pdf)

[7] Meirelles(2013) Paulo Roberto Miranda Meirelles. **Monitoramento de métricas de código-fonte em projetos de software livre**. Tese de Doutorado, Universidade de São Paulo. [Link.](https://social.stoa.usp.br/articles/0030/6046/tesePauloMeirelles.pdf)

#Apêndice A

#GQM (Goal, Question, Métric)

##OBJETIVOS ESTRATÉGICOS

O.1 - Qualidade do produto

|Analisar|código|
|:---:|:---:|
|Com o propósito de|melhorar|
|Com respeito a|Manutenibilidade do software|
|Sobre o ponto de vista do|desenvolvedor|
|No contexto do |projeto wikilegis mobile|

##QUESTÕES

|||
|---|---|
|**Foco na qualidade** <br/> **- Q.1.1** O produto apresenta uma boa manutenibilidade? <br/> **- Q.1.2** O produto apresenta uma boa usabilidade?|**Fatores de variação** <br/> - A produtividade não atender a expectativa; <br/> - Conhecimento da equipe limitado;|
|**Hipótese de baseline** <br/> - 30% de cobertura de teste até a primeira release; <br/> - 90% de cobertura de teste até a segunda release; <br/> - X de duplicação de código;<br/> - X de acoplamento;<br/> - X de coesão;<br/> - 0 discordâncias com a folha de estilo.|**Impacto das hipóteses de base line**<br/> - Baixa qualidade do produto de software;<br/> - Baixa manutenibilidade.|

##MÉTRICAS

|Métrica|M.1.1.1 - Cobertura de teste|
|---|---|
|**Objetivo da Medição**|Garantir que o software não contenha erros de lógica ou digitação, assim tendo uma garantia de qualidade.|
|**Descrição**||
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação.<br/>Ferramenta: Mezuro|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| Primeira release:<br/> “Dentro do esperado” dado por CoberturaTeste > 30%<br/>“fora do planejado” dado por CoberturaTeste < 30% <br/> Segunda release: <br/> “Dentro do esperado” dado por CoberturaTeste > 90%<br/>“fora do planejado” dado por CoberturaTeste < 90%|
|**Providências**| Caso a métrica esteja abaixo do esperado na primeira release, em qualquer uma das interações que envolvam desenvolvimento, a equipe de gerência deve ser alertada e o coach(Monitor) deve ser procurado em caso de dificuldades.<br/> Caso a métrica esteja abaixo do esperado na segunda release, na primeira semana a equipe de desenvolvimento deve ser alertada apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando do desenvolvimento de testes|

|Métrica|M.1.1.2 - Complexidade ciclomática|
|---|---|
|**Objetivo da Medição**||
|**Descrição**| <br/>Complexidade ciclomática equivale ao número de desvios (ou estruturas condicionais) mais 1. Como a coleta consiste em contar o número de condicionais, a métrica também é chamada de complexidade condicional. Ela indica o número de testes que o fragmento de software precisa ter para cobrir todos caminhos linearmente independentes de execução.[5]|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Mezuro|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| A definir|
|**Providências**|Caso a métrica esteja abaixo do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.3 - Complexidade estrutural (Coesão)|
|---|---|
|**Fórmula**|A definir|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Mezuro|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| A definir|
|**Providências**|Caso a métrica esteja abaixo do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.4 - Conexões Aferentes de uma classe (ACC)|
|---|---|
|**Objetivo da Medição**|Garantir a manutenibilidade do código, garantindo que o cliente será capaz de evoluir o código.|
|**Descrição**|Digamos q a classe Ca acessa a classe Cb. Podemos dizer que a classe Ca é cliente da classe fornecedora Cb e denotamos Ca => Cb. Considerando Ci != Cj e Ci => Cj, então cliente(Ci,Cj) = 1, se não cliente(Ci,Cj) = 0. Então ACC = Somatório, de 1 até n,cliente(Ci,C), onde n = ao numero total de classes do sistema e C a classe em que se está calculando. Essa métrica indica, se apresentar um grande valor, que o sistema é de difícil manutenção, pois, será qualquer mudança provavelmente afetará outras partes do sistema.[7]|
|**Fórmula**|![formula 1](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.png)<br/>![formula 2](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/imagens/formula_1.1.png)|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Mezuro|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit da interação para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar a evolução do software.|
|**Análise**| 0 - 2 Bom (Esperado)<br/> 2 - 20 Regular <br/> 20 - INF Ruim |
|**Providências**| Caso a métrica esteja abaixo do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.1.5 - Tamanho médio dos Métodos (Atomicidade)|
|---|---|
|**Fórmula**|A definir|
|**Escala da Medição**|Racional|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação. <br/>Ferramenta: Mezuro|
|**Procedimentos**| Será feito o uso da ferramenta no ultimo commit para obter os dados. Será mantido junto com as outras métricas numa tabela para acompanhar o software.|
|**Análise**| A definir|
|**Providências**|Caso a métrica esteja abaixo do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.|

|Métrica|M.1.2.1 - Usabilidade|
|---|---|
|**Fórmula**| A = amostra / U = usabilidade / M = Média <br/> U = M(A1)+M(A2)+M(A3)+M(A4)+M(A5)
|**Escala da Medição**|Ordinal|
|**Coleta**|Responsável: Equipe de gerência.<br/> Periodicidade ou Evento: A cada interação.|
|**Procedimentos**| Deverá ser feito um estudo de campo onde pessoas do contexto (Cidadãos) utilizam o software e a partir do uso da pessoa deverá ser avaliado o seguinte checklist.<br/>* O participante consegue descobrir as funcionalidades do sistema? <br/>* O participante conseguiu executar a funcionalidade pedida na primeira tentativa?<br/>* Como o participante julga a aparência do produto?<br/>* O participante julga a complexidade do sistema baixa?<br/>* O participante julga a relevância do sistema alta?<br/>Ao terminar uma amostragem de pelo menos 20 pessoas, as amostras devem ser armazenadas e concisas em uma média para cada ponto perguntado e ai então analisado. |
|**Análise**| Caso a média das amostras dê menor que 4 a usabilidade Caso a métrica esteja abaixo do esperado, na primeira semana a equipe de desenvolvimento deve ser alertada e apontada para possíveis materiais de ajuda. Se continuar por uma segunda semana, a equipe de gerência de interferir, participando da manutenção do código.erá dada como "não satisfatória" e acima de 4 como satisfatória.|
|**Providências**|Caso a métrica esteja abaixo do esperado deve ser avaliado qual amostra estava mais baixa e em cima dela deve-se tomar providências para melhorar a interface, para que na próxima pesquisa se consiga um resultado satisfatório.| 

##INDICADORES