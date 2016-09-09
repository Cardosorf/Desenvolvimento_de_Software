### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 17/08/2016 | 1 | Elaboração Inicial | Igor Duarte |
| 18/08/2016 | 1.1 | Adição da Equipe | Izabela Cardoso |

# 1. Introdução

<p align="justify">Este documento tem como objetivo a formalização do projeto Wikilegis Mobile. As informações contidas nos tópicos a seguir foram produzidos a fim de mostrar um grande resumo dos riscos, limites e recursos, bem como mostrar o estudo de viabilidade do projeto. (PMBOK quinta edição, cap.4.1.3.1, pag. 71)</p>

# 2. Descrição do Projeto

<p align="justify">O projeto trata-se de uma adaptação para Android de uma aplicação web, de código aberto, desenvolvida pelo Laboratório Hacker da Câmara dos Deputados. Seu objetivo é oferecer aos seus usuários a oportunidade de propor alterações e discussões relacionadas à redação de projetos de lei.</p>

# 3. Propósito e justificativa do Projeto

<p align="justify">O projeto tem como objetivo alcançar o cidadão que tem o direito democrático de contribuir com as legislações que regem seu pais. O Wikilegis procura fazer isso de forma interativa e atrativa, de forma a atrair o cidadão comum. Portanto se justifica a necessidade de uma adaptação mobile da plataforma web, tendo em vista que dos domicílios brasileiros que acessam a internet:</p>
* 80,4% o fizeram por celular (63.42% são android3)
* 76,6% via microcomputador
* 21,9% por tablet
* 4,9% por TV 
* 0,9% por outros equipamentos.

fonte:[IBGE](http://saladeimprensa.ibge.gov.br/noticias?view=noticia&id=1&busca=1&idnoticia=3133), [statista](http://www.statista.com/statistics/262167/market-share-held-by-mobile-operating-systems-in-brazil/)

# 4. Restrições do Projeto

As restrições do projeto wikilegis mobile é:
* A aplicação está restrita a plataforma android.
* A aplicação está restrita a utilizar a API do próprio wikilegis para adquirir os dados das propostas e para autenticação dos usuários.
* O projeto está restrito ao tempo da disciplina de GPP/MDS (08/08/2015 - XX/12/2015).
* O projeto está restrito ao escopo de recursos de alunos da matéria de GPP/MDS.

# 5. Riscos do Projeto

<p align="justify">Os principais riscos do desenvolvimento do aplicativo Android do Wikilegis e suas respectivas medidas preventivas são:</p>

* Equipe de desenvolvimento não conseguir se adaptar às tecnologias propostas para o projeto.

**Plano de ação: Realização de treinamentos com o intuito de ensinar as tecnologias com as quais a equipe de desenvolvimento possui dificuldade ou não conhece.**

* Membro da equipe trancar ou abandonar a disciplina.

**Plano de ação: Distribuir as tarefas entre os integrantes remanescentes de forma que não sobrecarregue nenhum dos membros da equipe.**

* As ferramentas propostas não funcionarem corretamente nos computadores dos integrantes do grupo.

**Plano de ação: Configurar o ambiente através de uma receita de configuração de ambiente.**

# 6. Custos do Projeto

## 6.1. Recursos Humanos

De acordo com o [Relatório de Gestão da UnB do ano de 2015](http://www.dpo.unb.br/documentos/Relatorio_Gestao_2015.pdf), o custo anual de um aluno de Engenharia de Software é cerca de R$ 11.020,00. Dessa forma, levando em consideração que um aluno do mesmo curso pega em média 48 créditos por ano e estimando que cada crédito corresponda a 15 horas de aula, estima-se que o custo por hora de um aluno de Engenharia de Software da UnB seja:

11.020,00 / (48 * 15) ≃ R$ 15,30.

<p align="justify">Tendo em vista que até a terceira semana do projeto a equipe contava com 10 integrantes que trabalhavam 10 horas por semana cada e que a partir de então a equipe deverá possuir 9 integrantes trabalhando 12 horas por semana cada até o final das 16 semanas do projeto, o valor estimado para gasto com recursos humanos é de:</p>

Três primeiras semanas: 10 * 10 * 3 * 15,3 = R$ 4.590,00
<br>
Restante do projeto: 12 * 9 * 13 * 15,3 = R$ 21.481,20
<br>
Total: 4.590,00 + 21.481,20 = R$ 26.071,20

## 6.2. Equipamentos e Serviços

Os equipamentos e serviços levados em consideração e seus respectivas custos foram: 

* Aluguel de espaço no Gama (180 m²): R$ 1.200,00 / mês.
* Energia Elétrica: Levando-se em consideração a estimativa de 447,60 kWh para consumo mensal e utilizando uma média de preço de R$ 0,54 por kWh, calcula-se um total de 447,60 * 0,54 ≃ R$ 241,70 / mês.
* Notebooks: Utilizando uma média de preço de R$ 2.300,00 para cada notebook e tendo em vista que cada um dos 10 membros da equipe precisará do seu próprio notebook, calcula-se um total de 2.300,00 * 10 =  R$ 23.000,00.
* Internet (15 MB/s): R$ 75,90 / mês.
* Publicação (Google Play): R$ 80,10.

Sendo assim, o valor total gasto com equipamentos e serviços durante o período de desenvolvimento do projeto (aproximadamente 4 meses) é de:

1.200,00 * 4 + 241,70 * 4 + 23.000 + 75,90 * 4 + 80,10 = R$ 29.150,50.

## 6.3. Custo Total

Por fim, para se obter o custo total do projeto, basta somar os custos com recursos humanos e equipamentos e serviços:

26.071,20 + 29.150,50 = R$ 55.221,70.


# 7. Steakholders (Partes interessadas)

## 7.1. Equipe de Gerência

<p align="justify">Alunos da disciplina que tem a responsabilidade de planejar, monitorar e controlar o projeto, dessa forma garantindo um equilíbrio e assim o sucesso do projeto. Além disso, tem a responsabilidade de tomar decisões fundamentais dentro do projeto, sendo assim, responsabilizados por estas.</p>

| Nome                  | Disciplina | E-mail                     | Github              |
|-----------------------|:----------:|----------------------------|---------------------|
| Lucas Brilhante           | GPP        | lbrilhante82@gmail.com  | [@lucasBrilhante](https://github.com/lucasBrilhante)     |
| Izabela Cardoso         | GPP        | cizabelacristina@gmail.com   | [@izacristina](https://github.com/izacristina)     |
| Igor Ribeiro       | GPP        | igor.ribeiro.duarte@gmail.com | [@igorribeiroduarte](https://github.com/igorribeiroduarte) |
| Pedro Ivo        | GPP        | andradepedroivo@gmail.com | [@freemanpivo](https://github.com/freemanpivo)  |

## 7.1. Equipe de desenvolvimento

<p align="justify">Alunos da disciplina de MDS(Métodos de desenvolviemnto de software), que tem a responsabilidade de construir o produto e a documentação relacionada a metodologia seguida (RUP).</p>

| Nome                  | Disciplina | E-mail                     | Github              |
|-----------------------|:----------:|----------------------------|---------------------|
| Thiago Nogueira        | MDS        | thiagonf10@gmail.com | [@thiagonf](https://github.com/thiagonf)   |
| Marcelo Augusto  | MDS        | mekmay@gmail.com | [@maugustoo](https://github.com/maugustoo)                   |
| Augusto Vilarins | MDS        | augusto.vilarins@gmail.com | [@augustovilarins](https://github.com/augustovilarins)   |
| Josué Nascimento    | MDS      | josuetk63@gmail.com | [@josutk](https://github.com/josutk) | 
| Rodrigo Campos    | MDS      | rodrigo.redcode@gmail.com | [@rodrigocam](https://github.com/rodrigocam) | 

## 7.2. Monitores

<p align="justify">Ex-Aluno das disciplinas de MDS e GPP que tem a responsabilidade de acompanhar e ajudar a equipe de desenvolvimento e planejamento, garantindo que a avaliação do docente será terá uma fundamentação ótima. Além disso, devem tirar duvidas quanto as metodologias e as tecnologias das disciplinas.</p>

| Nome                  | Disciplina |
|-----------------------|:----------:|
| Victor Hugo       | MDS        |
| Gabriel Climaco | MDS        |
| Emilie Morais |GPP|

## 7.3. Docente

Professor das matérias de GPP e mds que tem a responsabilidade de avaliar os alunos responsáveis pelo projeto.

| Nome                  | Github     |
|-----------------------|:----------:|
| Carla Rocha          | [@rochaCarla](https://github.com/RochaCarla) |

## 7.4. Usuários

Os principais alvos do produto deste projeto são os cidadãos brasileiros.

# 8. Produto do Projeto

As entregas do produtos serão feitas em duas fases Release 1 (R1) e Release 2 (R2).

**R1:** Arquitetura pronta e incremento de software (Duas funcionalidades)

**R2:** Incremento de software e deploy (Todos casos de uso restantes)

## 8.1 Requisitos de alto nível

|ID|Requisito|Prioridade|
|:--:|:--:|:--:|
|R01|Gerenciamento dos usuários|Alta|
|R02|Gerenciamento dos projetos de lei|Alta|
|R03|Gerenciamento de sugestões de alterações em projetos de lei|Alta|