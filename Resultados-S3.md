## 1. Indicadores de qualidade do processo

### 1.1. Burndown

[[imagens/burdown_3.png]]

### 1.2. Velocity

![Velocity](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/velocityt3.png)

### 1.3. Conhecimento

![Conhecimento](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/conhecimento3.png)

### 1.4. Retrospectiva

![Retrospectiva](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/RetrospectivaSprint3.jpg)

### 1.5. Frequência

![Retrospectiva](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/presencaS3.png)

### 1.6. Quadro de Humor

![HUmor](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sent2.jpg)

### 1.7. Considerações

A equipe conseguiu entregar todos os pontos planejados! Por um lado foi gratificante ter conseguido por um fim nas pendências, mas por outro foi bem estressante, pois passamos pela refatoração do download de dados, a história com maior valor de pontos, motivo pelo qual esta sprint foi mais longa. Notou-se uma melhora na integração da equipe em algumas reuniões que houveram, mas houveram problemas em relação aos Daily Meetings devido à semana universitária da UnB, pois os Daily Meetings eram feitos na Universidade. Para tal problema utilizou-se de Daily Meetings via hangout ou por mensagens no Telegram.

Outro ponto positivo foi que de fato a realização das reuniões no LabHacker minimizou os problemas de dependência com a API, pois os problemas eram facilmente comunicados para os desenvolvedores da API, por outro lado, como o LabHacker fica na Câmara dos Deputados, o local ficou complicado para alguns membros, o que gerou mais faltas.

Além da refatoração do download de dados, a equipe teve que refatorar, também, o design do aplicativo. Este fato foi pedido à equipe de desenvolvimento pelo Designer do LabHacker, que notou problemas de UX na sugestão de proposta e comentários feitos pelo usuário, pois tal tarefa não era muito intuitiva.

Um ponto percebido é que, na pressa para terminar as pendências, o grupo estava planejando muitos pontos para uma sprint de uma semana, visto que só foi possível concluir todos os pontos desta sprint pois a mesma foi mais longa, e anteriormente, era planejado um valor de pontos muito parecido com este para sprints de uma só semana, para as próximas sprints pretende-se então distribuir melhor as pendências, de forma que o planejado esteja mais de acordo com o velocity da equipe.

## 2. Indicadores de qualidade do produto

### 2.1. Cobertura

![cobertura](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint0-cobertura.png).

**OBS:** Não foi possível gerar a cobertura de testes nessa sprint, por este fato manteve-se a a cobertura de testes da sprint anterior. Não foi possível gerar a cobertura de testes porque havia testes para verificar o tipo de conexão do celular, como tais testes eram executados em máquinas virtuais do Android, elas não permitem que se use Wi-fi, pois possuem por padrão o 3G, portanto sempre um dos testes sempre falhava nestes dispositivos.

### 2.2. Métricas 50%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint3_mean.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_0.png)

### 2.3. Métricas 75%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint3_upper.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_75.png)

### 2.4. Métricas 95%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint3_ninety.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_95.png)

### 2.5. Considerações

Apesar de algumas métricas estarem acima do estabelecido como "bom", é preciso analisar as classes que causaram tal valor fora do padrão. Em relação ao ACCM, a principal classe que causa um valor ruim é a MainActivity.java localizada dentro do pacote view. Analisando tal classe percebe-se uma estrutura de switch-cases que para os desenvolvedores são importantes e não há como reduzir o valor do ACCM de tal classe para um valor menor que 3.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint3_metrics_justify.png)

Ainda sobre o ACCM, a equipe notou uma implementação de comparadores de projetos ou de segmentos, que influenciam também no valor da métrica de complexidade. Um exemplo desses códigos é dado abaixo, e notando que tal implementação é necessária ao projeto, manteve-se tais recursos sabendo que precisa-se analisar estas classes de forma individual para influenciar na nota de complexidade.

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint3_metrics_justify2.png)