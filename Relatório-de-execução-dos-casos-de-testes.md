| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | :---: | :---: |
| 28/08/2016 | 1.0 | Abertura do documento | Rodrigo Oliveira |
| 28/08/2016 | 1.1 | Adição do teste do UC04 | Rodrigo Oliveira |
| 28/08/2016 | 1.2 | Adição do teste UC01, UC02, UC03 | Rodrigo Oliveira |
| 05/09/2016 | 1.3 | Arrumando a numeração dos TFUC | Marcelo Augusto |

#Índice

1. [TFUC01 - Cadastrar usuário](#tfuc01-cadastrar-usuário)
2. [TFUC02 - Visuaizar projeto de lei](#tfuc02-visualizar-projeto-de-lei)
3. [TFUC03 - Visualizar segmentos do projeto de lei](#tfuc03-visualizar-segmentos-do-projeto-de-lei)
4. [TFUC04 - Listar Projetos](#tfuc04-listar-projetos)

***

#TFUC01: Cadastrar usuário
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | :---: | :---: |
| CT001 | Nome | Nome com letras do alfabeto de até 30 caracteres. Caracteres de A-Z, a-z. | Números, espaços em branco ou sem preenchimento, nomes com mais de 30 caracteres. |
| CT001 | Segundo Nome | Nome com letras do alfabeto de até 30 caracteres. Caracteres de A-Z, a-z. | Números, espaços em branco ou sem preenchimento, nomes com mais de 30 caracteres. |
| CT001 | E-Mail | E-Mail com até 150 caracteres. Caracteres A-Z, a-z, 0-9. Além desses caracteres, é permitido usar: “ - ”, “ _ ” , ” . ” , “+”, “@” | Outros caracteres, espaços em branco ou sem preenchimento, e-mail com mais de 150 caracteres |
| CT001 | Senha | Senha que tenha, no mínimo 6 caracteres e no máximo 10, e seja igual a senha do campo de confirmação | Senha com menos de 6 ou mais de 10 caracteres, espaços em branco ou sem preenchimento, ou que não sejam iguais em ambos os campos (senha e confirmação de senha) |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | :---: | :---: | :---: |
| CT001_01 | Nome Válido | O nome do usuário é cadastrado com sucesso | Nome de usuário cadastrado com sucesso | Sucesso |
| CT001_02 | Nome Inválido | O sistema notifica que o nome do usuário é inválido e solicita uma nova entrada de dados | Apareceu uma mensagem de nome inválido | Sucesso |
| CT001_01 | Segundo nome Válido | O segundo nome do usuário é cadastrado com sucesso | Segundo nome cadastrado com sucesso | Sucesso |
| CT001_02 |Segundo nome Inválido | O sistema notifica que o segundo nome do usuário é inválido e solicita uma nova entrada de dados | Apareceu uma mensagem de segundo nome inválido | Sucesso |
| CT001_01 | E-Mail Válido | O e-mail digitado é cadastrado com sucesso | E-mail do usuário cadastrado com sucesso | Sucesso |
| CT001_02 | E-Mail Inválido | O sistema informa que o e-mail digitado é inválido e solicita uma nova entrada de dados | Apareceu uma mensagem de e-mail inválido | Sucesso |
| CT001_01 | Senha Válida | A senha do usuário é cadastrada com sucesso | Senha do usuário cadastrada com sucesso | Sucesso |
| CT001_02 | Senha Inválida | O sistema informa ao usuário que a senha digitada é inválida e solicita uma nova entrada de dados | Apareceu uma mensagem de senha inválido | Sucesso |

#TFUC02: Visualizar projeto de lei
###Classes de equivalência:
| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | :---: | :---: |
| CT002_01 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | :---: | :---: | :---: |
| CT002_01 | Toque do usuário em um projeto | Redirecionamento para uma página com o conteúdo do projeto de lei selecionado | | | 
| CT002_02 | id do projeto ,titulo,epigrafe,status, descrição, tema, segmentos do projeto, numero de propostas e data do projeto | sistema notifica se todos os dados vem null| O sistema exibe uma mensagem informando que o projeto de lei não pode ser carregado | Sucesso 
| CT002_03 |id do projeto ,titulo,epigrafe,status,descrição, tema,segmentos do projeto, numero de propostas e data do projeto| o sistema notifica se algum dos campos vem null| O sistema exibe uma mensagem informando que o projeto de lei não pode ser carregado | Sucesso |

#TFUC03: Visualizar segmentos do projeto de lei
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT003_00 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT003_01 | Toque do usuário em um segmento | Redirecionamento para uma página com o conteúdo do segmento, sugestões de proposta e avaliações do mesmo |
|CT003_02|id do segmento, ordem , identificado projeto ao qual o segmento pertence, se o segmento já sofreu alteração,se o projeto sofreu proposta de alteração , tipo , numero ,conteúdo da proposta de alteração, identificador ,id voto , id do comentário ,data de criação do segmento|O sistema informa ao usuário que parou a aplicação| Mensagem informando que o campo não pode ser nulo | Sucesso |
|CT003_03|id do segmento, ordem , identificado projeto ao qual o segmento pertence, se o segmento já sofreu alteração,se o projeto sofreu proposta de alteração , tipo , numero ,conteudo da proposta de alteração, identificador ,id voto , id do comentário ,data de criação do segmento|O sistema informa ao usuario que parou a aplicação| O usuário é informado que houve um erro na aplicação e que o campo não pode ser nulo | Sucesso |
#TFUC04: Listar projetos
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT004_01 | Toque do usuário | Toque do usuário | Não se aplica |
| CT004_02 | Toque do usuário | Toque do usuário | Não se aplica |
| CT004_03 | Toque do usuário | Toque do usuário | Não se aplica |
| CT004_04 | Toque do usuário | Toque do usuário | Não se aplica |
| CT004_05 | Toque do usuário | Toque do usuário | Não se aplica |
| CT004_06 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT004_01 | Toque do usuário em listar projetos por status fechado, sem a existência de projetos com tal status | O sistema exibir uma mensagem, informando que não existem projetos com este status |
| CT004_02 | Toque do usuário em listar projetos por status fechado, com a existência de projetos com  tal status | O sistema lista todos os projetos de lei com status fechado |
| CT004_03 | Toque do usuário em listar projetos por status aberto, com a existência de projetos com tal status | O sistema lista todos os projetos de lei com status aberto |
| CT004_04 | Toque do usuário em listar projetos por status aberto, sem a existência de projetos com tal status | O sistema exibe uma mensagem, informando que não existem projetos com este status |
| CT004_05 | Toque do usuário em listar projetos por relevância | O sistema lista todos os projetos de lei, ordenando do projeto com mais sugestões de proposta para o projeto com menos sugestões de proposta |
| CT004_06 | Toque do usuário em listar projetos por relevância, sem a existêcia de projetos | O sistema exibe uma mensagem, informando que não existem projetos |
