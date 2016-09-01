| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 28/08/2016 | 1.0 | Abertura do documento | Rodrigo Oliveira |
| 28/08/2016 | 1.1 | Adição do teste do UC04 | Rodrigo Oliveira |
| 28/08/2016 | 1.2 | Adição do teste UC01, UC02, UC03 | Rodrigo Oliveira |

#Índice

1. [TFUC01 - Listar Projetos](#tfuc01-listar-projetos)
2. [TFUC02 - Visuaizar projeto de lei](#tfuc02-visualizar-projeto-de-lei)
3. [TFUC03 - Visualizar segmentos do projeto de lei](#tfuc03-visualizar-segmentos-do-projeto-de-lei)
4. [TFUC04 - Cadastrar usuário](#tfuc04-cadastrar-usuário)

***

#TFUC01: Listar projetos
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT001_01 | Toque do usuário | Toque do usuário | Não se aplica |
| CT001_02 | Toque do usuário | Toque do usuário | Não se aplica |
| CT001_03 | Toque do usuário | Toque do usuário | Não se aplica |
| CT001_04 | Toque do usuário | Toque do usuário | Não se aplica |
| CT001_05 | Toque do usuário | Toque do usuário | Não se aplica |
| CT001_06 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT001_01 | Toque do usuário em listar projetos por status fechado, sem a existência de projetos com tal status | O sistema exibir uma mensagem, informando que não existem projetos com este status |
| CT001_02 | Toque do usuário em listar projetos por status fechado, com a existência de projetos com  tal status | O sistema lista todos os projetos de lei com status fechado |
| CT001_03 | Toque do usuário em listar projetos por status aberto, com a existência de projetos com tal status | O sistema lista todos os projetos de lei com status aberto |
| CT001_04 | Toque do usuário em listar projetos por status aberto, sem a existência de projetos com tal status | O sistema exibe uma mensagem, informando que não existem projetos com este status |
| CT001_05 | Toque do usuário em listar projetos por relevância | O sistema lista todos os projetos de lei, ordenando do projeto com mais sugestões de proposta para o projeto com menos sugestões de proposta |
| CT001_06 | Toque do usuário em listar projetos por relevância, sem a existêcia de projetos | O sistema exibe uma mensagem, informando que não existem projetos |

#TFUC02: Visualizar projeto de lei
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT002_00 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT002_00 | Toque do usuário em um projeto | Redirecionamento para uma página com o conteúdo do projeto de lei selecionado |

#TFUC03: Visualizar segmentos do projeto de lei
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT003_00 | Toque do usuário | Toque do usuário | Não se aplica |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT002_00 | Toque do usuário em um segmento | Redirecionamento para uma página com o conteúdo do segmento, sugestões de proposta e avaliações do mesmo |

#TFUC04: Cadastrar usuário
###Classes de equivalência:

| Casos de teste | Entrada | Classes de Equivalência Válidas | Classes de equivalência inválidas |
| :---: | :---: | --- | :---: |
| CT004 | Nome | Nome com letras do alfabeto de até 30 caracteres, caracteres especiais usados na composição de nomes | Números, espaços em branco ou sem preenchimento, nomes com mais de 30 caracteres |
| CT004 | Segundo Nome | Nome com letras do alfabeto de até 30, caracteres especiais usados na composição de nomes | Números, espaços em branco ou sem preenchimento, nomes com mais de 30 caracteres |
| CT004 | E-Mail | E-Mail com até 150 caracteres.
Caracteres A-Z, a-z, 0-9. Além desses caracteres, é permitido usar: “ - ”, “ _ ” , ” . ” , “+”, “@” | Outros caracteres, espaços em branco ou sem preenchimento, e-mail com mais de 150 caracteres |
| CT004 | Senha | Senha que tenha, no mínimo 6 caracteres e no máximo 10,  e seja igual a senha do campo de confirmação | Senha com menos de 6 ou mais de 10 caracteres, espaços em branco ou sem preenchimento, ou que não sejam iguais em ambos os campos (senha e confirmação de senha) |

###Análise de resultados:

| Casos de teste | Entrada | Resultado esperado | Resultado obtido | Status |
| :---: | :---: | --- | :---: | :---: |
| CT001_01 | Toque do usuário em listar projetos por status fechado, sem a existência de projetos com tal status | O sistema exibir uma mensagem, informando que não existem projetos com este status |
| CT001_02 | Toque do usuário em listar projetos por status fechado, com a existência de projetos com  tal status | O sistema lista todos os projetos de lei com status fechado |
| CT001_03 | Toque do usuário em listar projetos por status aberto, com a existência de projetos com tal status | O sistema lista todos os projetos de lei com status aberto |
| CT001_04 | Toque do usuário em listar projetos por status aberto, sem a existência de projetos com tal status | O sistema exibe uma mensagem, informando que não existem projetos com este status |
| CT001_05 | Toque do usuário em listar projetos por relevância | O sistema lista todos os projetos de lei, ordenando do projeto com mais sugestões de proposta para o projeto com menos sugestões de proposta |
| CT001_06 | Toque do usuário em listar projetos por relevância, sem a existêcia de projetos | O sistema exibe uma mensagem, informando que não existem projetos |
