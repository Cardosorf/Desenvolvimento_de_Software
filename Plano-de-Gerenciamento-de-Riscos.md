## Histórico de Versões

|Responsável|Descrição|Data|
|-----------|---------|----|
|Izabela Cardoso| Criação da introdução e identificação dos riscos |02/09/2016|
|Izabela Cardoso| Adicionando probabilidade |03/09/2016|
|Izabela Cardoso| Adicionando impacto e prioridade |04/09/2016|

## 1. Introdução

<p align="justify">Este documento tem por objetivo identificar os riscos do projeto, categorizá-los, realizar uma análise quantitativa dos mesmos e estabelecer estratégias de resposta aos riscos identificados, descrevendo o processo de gerenciamento dos riscos no projeto.</p>

## 2. Identificação dos riscos

### 2.1. SWOT

<p align="justify">A técnica utilizada para identificar os riscos inicialmente foi a análise de forças, fraquezas, oportunidades e ameaças (SWOT, sigla em inglês), a imagem a seguir ilustra a aplicação da técnica no projeto Wikilegis Mobile.</p>

![SWOT](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-WikiLegis/imagens/fofa.jpg)

### 2.2. Categorização dos Riscos - EAR

<p align="justify">A Estrutura Analítica de Riscos (EAR) permite a organização dos riscos em categorias que representam suas causas, logo, esta técnica foi utilizada para identificar as possíveis causas dos riscos levantados pela técnica SWOT, resultando em uma estrutura hierárquica de categorias e sub-categorias.</p>

[Colocar imagem da EAR]

### 2.3 Registro dos riscos identificados

|Identificador|O evento x pode ocorrer|Causando o impacto|Cuja causa principal é|
|-------------|-----------------------|------------------|----------------------|
| R01         | Dificuldade com as tecnologias utilizadas | Atraso nas entregas das atividades | Falta de experiência da equipe com as tecnologias utilizadas |
| R02         | Produto não atender ao esperado pelo cliente | A rejeição do projeto pelo cliente | Falhas nas especificações e validações dos requisitos |
| R03         | Produto possuir desempenho ruim | Pouca aceitação dos usuários | Falta de experiência da equipe com as tecnologias utilizadas |
| R04         | Mudança no calendário acadêmico | Alterações no cronograma do projeto | Greves na universidade e imprevistos externos relacionados à Academia |
| R05         | Redução do uso da plataforma escolhida | Pouca utilização do aplicativo no mercado | Fatores externos |
| R06         | Atraso nas entregas das atividades | Atraso no cronograma | Falta de experiência, comunicação e/ou motivação da equipe, planejamento incorreto |
| R07         | Mudanças no Escopo | Atualização de artefatos e replanejamento | Escopo mal especificado, solicitação dos envolvidos, adaptação do cronograma |
| R08        | Redução de Membros | Sobrecarga de trabalha aos demais membros | Desmotivação |
| R09        | Erros de Estimativa e Planejamento | Membros sub/sobrecarregados, custo muito alto ou muito baixo | Inexperiência nas atividades de estimativa e planejamento |
| R10        | Falhas de comunicação entre a equipe | Retrabalho, execução de tarefas incorretamente, sobrecarga em membros específicos | Falta de organização da equipe |

## 3. Análise quantitativa dos riscos

Para a análise dos riscos foram definidos os níveis de probabilidade, impacto e prioridade utilizados no projeto.

### 3.1. Probabilidade

|Probabilidade|Intervalo|Representação|
|-------------|---------|-------------|
|Muito Baixa|Menor que 20%|1|
|Baixa|De 21% a 40%|2|
|Média|De 41% a 60%|3|
|Alta|De 61% a 80%|4|
|Muito Alta|Acima de 80%|5|

### 3.2. Impacto 

|Impacto|Descrição|Representação|
|-------------|---------|-------------|
|Muito Baixo|Impacto inexpressivo no desenvolvimento do projeto|1|
|Baixo|Pouco impacto no desenvolvimento do projeto|2|
|Médio|Impacto que prejudica o projeto porém de fácil recuperação|3|
|Alto|Impacto traz grave prejuízo ao projeto|4|
|Muito Alto|O impacto inviabiliza o projeto|5|

### 3.3. Prioridade

Para o auxílio das definições dos níveis de prioridade dos requisitos foi utilizada a matriz de probabilidade X impacto. Nessa matriz, os impactos e probabilidades são representados nas linhas e colunas, sendo cada uma das células o produto dos valores de representação do impacto de sua respectiva linha e da probabilidade de sua respectiva coluna.

![Matriz Probabilidade / Impacto](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-WikiLegis/imagens/tabela.png)

A partir desta matriz foram obtidos os níveis de prioridade e estabelecidas as respostas para cada um deles.

|Nível de Prioridade|Intervalo|Ação de resposta|
|-------------------|---------|----------------|
|Baixo|1 à 5|Aceitação|
|Médio|6 à 14|Mitigação|
|Alto|15 à 25|Prevenção e Mitigação|

## 4. Planejamento de respostas ao riscos