### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 05/09 | 1.0 |Versão inicial | Izabela Cristina |
| 24/08 | 1.1 | Adição CT01 | Josué Nascimento |
| 24/08 | 1.2 | Edição CT01 | Marcelo Augusto |
| 25/08 | 1.3 | Adição CT02 | Marcelo Augusto |
| 25/08 | 1.4 | Adição CT03 | Rodrigo Oliveira |
| 26/08 | 1.5 | Edição CT01,CT02 e CT03 | Marcelo Augusto |
| 26/08 | 1.6 | Adição CT04 | Josué Nascimento |
| 27/08 | 1.7 | Adição CT05 | Marcelo Augusto |
| 27/08 | 1.8 | Edição CT03 | Josué Nascimento |
| 28/08 | 1.9 | Edição CT04 | Rodrigo Oliveira |
| 28/08 | 2.0 | Edição do CT01 e exclusão do CT05 | Josué Nascimento |
| 29/08 | 2.1 | Edição CT01 | Rodrigo Oliveira |
| 05/09 | 2.2 | Edição CT01 | Marcelo Augusto |
| 20/09 | 2.3 | Adição CT002_02, CT002_03, CT003_02, CT003_03 | Marcelo Augusto |
***

#Índice

1. [UC01 - Cadastrar usuário](#uc01-cadastrar-usuário)
 1. [CT001_01](#ct001_01-cadastrar-usuário-com-todos-os-campos-de-registro-válidos)
 2. [CT001_02](#ct001_02-cadastrar-usuário-com-pelo-menos-um-campo-preenchido-incorretamente)
2. [UC02 - Visuaizar projeto de lei](#uc02-visualizar-projeto-de-lei)
 1. [CT002_01](#ct002_01-clicar-para-visualizar-um-projeto-de-lei)
3. [UC03 - Visualizar segmento](#uc03-visualizar-segmento)
 1. [CT003_01](#ct003_01-clicar-para-visualizar-um-segmento)
4. [UC04 - Listar Projetos](#uc04-listar-projetos)
 1. [CT004_01](#ct004_01-listar-projetos-por-status-fechado-sem-a-existência-de-projetos-com-tal-status)
 2. [CT004_02](#ct004_02-listar-projetos-por-status-fechado-com-a-existência-de-tal)
 3. [CT004_03](#ct004_03-listar--projetos-por-status-aberto-com-a-existência-de-tal)
 4. [CT004_04](#ct004_04-listar-projetos-por-status-aberto-sem-a-existência-de-projetos-com-tal-status)
 5. [CT004_05](#ct004_05-listar-projetos-por-relevância)
 6. [CT004_06](#ct004_06-listar-projetos-por-relevância-sem-a-existência-de-projetos)
 7. [CT004_07](#ct004_07-listar-projetos-por-data)
 8. [CT004_08](#ct004_08-listar-projetos-por-data-sem-a-existência-de-projetos)


***


#UC01: Cadastrar Usuário

###<b>CT001_01:</b> Cadastrar Usuário com todos os campos de registro válidos 

<b>Descrição:</b> Esse caso de teste irá verificar se todos os campos do registro estão preenchidos corretamente.

<b>Pré condições:</b> Todos os campos de cadastro corretamente preenchidos e solicitar a efetuação do mesmo no sistema.

<b>Pós condições:</b> O Sistema apresenta uma mensagem de sucesso do cadastro , e os dados usuário são registrados no banco de dados.

<b>Dados requeridos:</b> Email, primeiro nome, segundo nome e senha.

###<b>CT001_02:</b> Cadastrar Usuário com pelo menos um campo preenchido incorretamente.

<b>Descrição:</b> Esse caso de teste irá verificar se existe algum campo preenchido de forma incorreta.

<b>Pré condições:</b> Solicitar registro no sistema com algum campo preenchido de forma incorreta.

<b>Pós condições:</b>  O sistema apresenta uma imagem de existência de campo inválido.

<b>Dados requeridos:</b> Email, primeiro nome, segundo nome e senha.

#UC02: Visualizar Projeto de Lei

###<b>CT002_01:</b> Clicar para visualizar um projeto de lei.

<b>Descrição:</b> Este caso de teste irá verificar se o usuário foi redirecionado ao projeto de lei selecionado pelo usuário.

<b>Pré condições:</b> Selecionar o projeto de lei.

<b>Pós condições:</b> O sistema exibe o projeto de lei requerido.

<b>Dados requeridos:</b> Não há.

###<b>CT002_02:</b> Verificar se todos os campos dos projetos de lei vem diferentes de nulos.

<b>Descrição:</b> Este caso de teste irá verificar se ao baixar as informações da api todos os dados são diferentes de null.

<b>Pré condições:</b> Não há

<b>Pós condições:</b> O sistema deve ter baixado para o banco local as informações do projeto de lei.

<b>Dados requeridos:</b> Não há.

###<b>CT002_03:</b> Verificar se algum dos campos dos projetos de lei vem nulos.

<b>Descrição:</b> Este caso de teste irá verificar se ao baixar as informações da api algum dos dados vem nulo.

<b>Pré condições:</b> Não há

<b>Pós condições:</b> Será mostrado para o usuário que houve um erro na aplicação.

<b>Dados requeridos:</b> Não há.

#UC03: Visualizar segmento

###<b>CT003_01:</b> Clicar para visualizar um segmento.

<b>Descrição:</b> Este caso de teste irá verificar se o usuário foi redirecionado ao segmento do projeto de lei selecionado.

<b>Pré condições:</b> Selecionar o segmento do projeto de lei.

<b>Pós condições:</b> O sistema exibe o segmento e as sugestões de propostas referentes a ele.

<b>Dados requeridos:</b> Não há.

###<b>CT003_02:</b> Verificar se todos os campos dos segmentos vem diferentes de nulos.

<b>Descrição:</b> Este caso de teste irá verificar se ao baixar as informações da api todos os dados são diferentes de null.

<b>Pré condições:</b> Não há

<b>Pós condições:</b> O sistema deve ter baixado para o banco local as todas informações dos segmentos.

<b>Dados requeridos:</b> Não há.

###<b>CT003_03:</b> Verificar se algum dos campos dos projetos de lei vem nulos.

<b>Descrição:</b> Este caso de teste irá verificar se ao baixar as informações da api algum dos dados vem nulo.

<b>Pré condições:</b> Não há

<b>Pós condições:</b> Será mostrado para o usuário que houve um erro na aplicação.

<b>Dados requeridos:</b> Não há.

#UC04: Listar projetos
###<b>CT004_01:</b> Listar Projetos por status fechado sem a existência de projetos com tal status.

 <b>Descrição:</b> Este caso de teste irá verificar se, ao listar projetos por status fechado sem a existência de projetos fechados, aparecerá uma mensagem informando ao usuário que não há projetos.

 <b>Pré condições:</b> Selecionar o filtro de listagem de projetos de lei fechado.

<b>Pós condições:</b> O sistema apresenta um aviso informando a inexistência de projetos com o filtro requerido.

<b>Dados requeridos:</b> Não há

###<b>CT004_02:</b> Listar Projetos por status fechado com a existência de tal.

<b>Descrição:</b> Este caso teste irá verificar se, ao filtrar projetos por status fechado com a existência de projetos fechados, serão listados todos os projetos de lei com o status de fechado.

<b>Pré-condições:</b> Selecionar o filtro de listagem  de projetos de lei fechado.

<b>Pós-condições:</b>  O sistema exibe os projetos de lei com o status de fechado.

<b>Dados requeridos:</b> Não há

###<b>CT004_03:</b> Listar  Projetos por status aberto com a existência de tal

 <b>Descrição:</b> Este caso teste irá verificar se, ao filtrar os projetos por status aberto com a existência de projetos abertos, serão listados todos os projetos de lei com o status de aberto.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos de lei aberto.

<b>Pós condições:</b>  O sistema exibe os projetos de lei com o status de aberto.

<b>Dados requeridos:</b> Não há

###<b>CT004_04:</b> Listar Projetos por status aberto sem a existência de projetos com tal status.

<b>Descrição:</b>  Este caso de teste irá verificar se, ao filtrar projetos por status aberto sem a existência de projetos abertos, aparecerá uma mensagem informando ao usuário que não há projetos.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos de lei aberto.

<b>Pós condições:</b> O sistema apresenta um aviso informando a inexistência de projetos com o filtro requerido.

<b>Dados requeridos:</b> Não há

###<b>CT004_05:</b> Listar projetos por relevância

<b>Descrição:</b> Este caso irá verificar se, ao filtrar os projetos de lei de acordo com o numero de propostas, o sistema organizou os projetos de acordo com a relevância, ou seja, do projeto com mais sugestões de propostas para o projeto que tem menos sugestões de propostas.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos por relevância.

<b>Pós condições:</b> O sistema irá apresentar os projetos em ordem crescente de acordo com a quantidade de propostas.

<b>Dados requeridos:</b> Não há

###<b>CT004_06:</b> Listar projetos por relevância sem a existência de projetos.

<b>Descrição:</b> Este caso irá verificar se ao listar projetos por relevância, sem a existência de projetos, aparecerá uma mensagem informando ao usuário que não existem projetos.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos por relevância.

<b>Pós condições:</b> O sistema apresenta um aviso informando a inexistência de projetos.

<b>Dados requeridos:</b> Não há

###<b>CT004_07:</b> Listar Projetos por data.

<b>Descrição:</b> Este caso irá verificar se, ao filtrar os Projetos de lei de acordo com a data de criação do projeto, o sistema organizou os projetos de acordo com a data de criação mais recente para a menos recente, nesta ordem de prioridade.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos de lei mais recentes.

<b>Pós condições:</b>  O sistema ordena os projetos por mais recentes.

<b>Dados requeridos:</b> Não há

###<b>CT004_08:</b> Listar Projetos por data sem a existência de projetos.

<b>Descrição:</b> Este caso irá verificar se, ao filtrar projetos de lei de acordo com a data de criação do projeto, sem a existência de projetos, aparecerá uma mensagem informando ao usuário que não existem projetos.

<b>Pré condições:</b> Selecionar o filtro de listagem de projetos de lei mais recentes.

<b>Pós condições:</b> O sistema apresenta um aviso informa a inexistência de projetos.

<b>Dados requeridos:</b> Não há
