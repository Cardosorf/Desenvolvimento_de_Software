## 1. Indicadores de qualidade do processo

### 1.1. Burndown

![Burndown](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/burndownsprint2.png)

### 1.2. Velocity

![Velocity](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/velocity2.png)

### 1.3. Conhecimento

![Conhecimento](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/conhecimento2.png)

### 1.4. Retrospectiva

![Retrospectiva](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/RetrospectivaSprint2.jpg)

### 1.5. Frequência

![Frequencia](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/presenca3.png)

### 1.6. Considerações

Nessa sprint houve um grande problema de dependência com a API do cliente. A utilização da API é um requisito, entretanto, a mesma ainda está em desenvolvimento, dessa forma, alguns problemas inesperados podem acontecer eventualmente, que foi o ocorrido na sprint, na qual somente ao desenvolver as histórias percebeu-se a necessidade de uma alteração na API para que as mesmas fossem concluídas.

Para a resolução deste problema esta sprint foi mais curta justamente para ajustar o dia da reunião de restrospectiva, review e planejamento das sprints para um dia em que fosse possível o cliente participar, sendo este, nas sexta-feiras.

Notando-se da falta de comprometimento de alguns membros da equipe, criou-se uma reunião para que a equipe pudesse conversar sobre a ausência desses membros e formas de poder ajudá-los no decorrer do projeto. Uma ação criada para tal fato, foi a utilização do quadro de sentimentos, em sua versão inicial, para que todos pudessem escrever em post-its o que gostava/não gostava no projeto, na gerência e nas tecnologias. A versão inicial deste quadro é exibida abaixo (a foto foi tirada após a dinâmica, então faltam muitos post-its e tomadas de decisão que foram escritas no quadro):

![quadroSentimentos](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sent1.jpg)


## 2. Indicadores de qualidade do código

### 2.1. Cobertura

![cobertura](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint0-cobertura.png)

### 2.2. Métricas 50%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint2_mean.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_0.png)

### 2.3. Métricas 75%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint2_upper.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_75.png)

### 2.4. Métricas 95%

**Resultados obtidos**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/sprint2_ninety.png)

**Valores chave**

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_95.png)

### 2.5. Considerações

Notou-se que o AMLOC (média de linhas por método) voltou a crescer, isso aconteceu pois na única história entregue, havia a criação de uma tela, com muitas operações ocorrendo dentro do método onCreate(). Na próxima sprint 3 espera-se resolver tal problema.