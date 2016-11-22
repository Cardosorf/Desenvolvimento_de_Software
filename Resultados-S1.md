## 1. Indicadores de qualidade do processo

## 1.1. Burndown

[[imagens/burndown_1.png]]

## 1.2. Velocity

[[imagens/velocity_1.png]]

## 1.3. Conhecimento

[[imagens/conhecimento_sprint_1.png]]

### 1.4. Retrospectiva

[[imagens/retro_1.jpg]]

### 1.5. Frequência

![Presenca](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/presenca2.png)

### 1.6. Considerações

Notando-se da falta de comprometimento de alguns membros da equipe, criou-se uma reunião para que a equipe pudesse conversar sobrea ausência desses membros e formas de poder ajudá-los no decorrer do projeto. Uma ação criada para tal fato foi a utilização do quadro de sentimentos, em sua versão inicial, para que todos pudessem escrever em post-its o que não gostava no projeto, na gerência e nas tecnologias. A versão inicial deste quadro é exibida abaixo (a foto foi tirada após a dinâmica, então faltam muitos post-its e tomadas de decisão que foram escritas no quadro):

![quadroSentimentos](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sent1.jpg)

## 2. Indicadores de qualidade do produto

### 2.1. Cobertura

![cobertura](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint0-cobertura.png)

### 2.2. Métricas 50%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint1_mean.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_0.png)

### 2.3. Métricas 75%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint1_upper.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_75.png)

### 2.4. Métricas 95%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint1_ninety.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_95.png)

### 2.5. Considerações

Conforme percebeu-se que a ACCM (complexidade ciclomática) e AMLOC (média de linhas por método) estavam um pouco acima dos parâmetros no percentil 75%, resolveu-se refatorar algumas classes com intuito de melhorar as métricas. As principais classes afetadas foram as DAOs, pois nelas se encontravam métodos com tipo de acesso protected e uma especialização de DAO que era extremamente desnecessária, estas ações diminuiram a métrica de ACCM. Para melhorar o AMLOC refatorou-se as classes de JSON e SegmentController, pois haviam métodos com muitas linhas.