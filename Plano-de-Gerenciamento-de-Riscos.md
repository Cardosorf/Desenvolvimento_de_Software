## Histórico de Versões

|Responsável|Descrição|Data|
|-----------|---------|----|
|Izabela Cardoso| Criação da introdução e identificação dos riscos |02/09/2016|
|Izabela Cardoso| Adicionando probabilidade |03/09/2016|
|Izabela Cardoso| Adicionando impacto e prioridade |04/09/2016|
|Izabela Cardoso| Adicionando planejamento das respotas |04/09/2016|

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
| R11        | Entregas antes do previsto | Tempo para desenvolver novas atividades ou evoluir as concluídas  | Alta produtividade da equipe ou erro no planejamento |
| R12        | Interesse do cliente em continuar o projeto | Apoio para o desenvolvimento de novas atividades e evolução das concluídas | Qualidade do projeto satisfatória para o cliente |

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
|Médio|Há impacto considerável porém de fácil recuperação |3|
|Alto|Há grande impacto no desenvolvimento do projeto|4|
|Muito Alto|O impacto inviabiliza o projeto|5|

### 3.3. Prioridade

<p align="justify">Para o auxílio das definições dos níveis de prioridade dos requisitos foi utilizada a matriz de probabilidade X impacto. Nessa matriz, os impactos e probabilidades são representados nas linhas e colunas, sendo cada uma das células o produto dos valores de representação do impacto de sua respectiva linha e da probabilidade de sua respectiva coluna.</p>

![Matriz Probabilidade / Impacto](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-WikiLegis/imagens/tabela.png)

A partir desta matriz foram obtidos os níveis de prioridade utilizados.

|Nível de Prioridade|Intervalo|
|-------------------|---------|
|Baixo|1 à 5|
|Médio|6 à 14|
|Alto|15 à 25|

## 4. Planejamento de respostas ao riscos

<p align="justify">De acordo com as definições de probabilidade, impacto e prioridade, foram definidas quais estratégias seriam tomadas em relação a cada risco, e qual ação é recomendada para atingir sucesso na execução da estratégia.</p>

### 4.1. Riscos negativos

| ID  | Descrição | Probabilidade | Impacto | Prioridade | Estratégia | Resposta Recomendada |
|-----|---------|-------------|-------|----------|----------|--------------------|
| R01 | Dificuldade com as tecnologias utilizadas | Alta (4) | Alto (4) | Alta (16) | Prevenir | Realização de treinamentos e transferência de conhecimentos entre os membros | 
| R02 | Produto não atender ao esperado pelo cliente | Baixa (2) | Alto (4) | Média (8) | Prevenir e Mitigar | Realização de validações com o cliente a cada iteração |
| R03 | Produto possuir desempenho ruim | Baixa (2) | Alto (4) | Média (8) | Prevenir e Mitigar | Realizar análises constantes do desempenho, transferir conhecimentos sobre características que influem no desempenho, Refatorar código buscando melhorar o desempenho |
| R04 | Mudança no calendário acadêmico | Baixa (1) | Alto (4) | Média (4) | Mitigar | Trabalhar de casa em caso de greve ou Renegociar com cliente cronograma de acordo com novo calendário |
| R05 | Redução do uso da plataforma escolhida |  Baixa (1) | Alto (4) | Média (4) | Mitigar | Reavaliar requisitos e ambiente do usuário |
| R06 | Atraso nas entregas das atividades | Alto (4) | Médio (3) | Média (3) | Mitigar | Replanejar o cronograma e realizar reuniões de acompanhamento |
| R07 | Mudanças no Escopo | Média (3) | Médio (3) | Média (9) | Prevenir e Mitigar | Validar escopo com o cliente e replanejar cronograma no caso de mudanças|
| R08 | Redução de Membros | Média (3) | Médio (3)  | Média (9) | Prevenir e Mitigar | Integrar e motivar a equipe, e em caso de redução de membros, realocar as atividades e refazer planejamento |
| R09 | Erros de Estimativa e Planejamento | Alta (4) | Médio (4) | Alto (16) | Prevenir e Mitigar | Pesquisar projetos anteriores e utilizar técnicas para embasar o planejamento, Replanejar conforme atividades anteriores | 
| R10 | Falhas de comunicação entre a equipe | Média (3) | Médio (3) | Médio (9) | Prevenir e Mitigar | Estabelecendo ferramentas de comunicação eficientes e reuniões fixas semanais, Agendando reuniões pontuais quando necessário para alinhar a equipe |

### 4.2. Riscos Positivos

| ID | Descrição | Probabilidade | Impacto | Prioridade | Estratégia | Resposta Recomendada |
|-----|---------|-------------|-------|----------|----------|----------|
| R11 | Entregas antes do previsto | Baixa (2) | Alto (4) | Médio (8) | Aceitar | Evoluir atividades concluída e executar novas atividades |
| R12 | Interesse do cliente em continuar o projeto | Alta (4) | Alto (4) | Alto (16) | Aceitar | Avaliar possíveis evoluções |