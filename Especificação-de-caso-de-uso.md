### Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 24/08/2016 | 1.0 | Abertura do documento | Marcelo Augusto |
| 24/08/2016 | 1.1 | Adição do UC01 | Josué Nascimento |
| 24/08/2016 | 1.2 | Adição do UC02 | Thiago Freire |
| 24/08/2016| 1.3 | Edição do UC01, UC02 e UC03 | Marcelo Augusto |
| 25/08/2016 | 1.4 | Edição do UC03 | Rodrigo Oliveira |
| 26/08/2016 | 1.5 | Adição do UC04 | Marcelo Augusto e Augusto Moreno |
| 26/08/2016 | 1.6 | Edição do UC02 | Thiago Freire |
| 26/08/2016 | 1.7 | Edição do UC01 e adição do UC05 | Augusto Moreno |
| 28/08/2016 | 1.8 | Edição do UC03 | Rodrigo Oliveira |
| 29/08/2016 | 1.9 | Edição e junção dos UC01 e UC05 | Josué Nascimento |
| 29/08/2016 | 2.0 | Edição do UC01 | Marcelo Augusto |
| 05/09/2016 | 2.1 | Trocando numeração dos casos de uso | Marcelo Augusto |
***

#Índice

1. [UC01 - Listar Projetos](#uc01-listar-projetos)
2. [UC02 - Visuaizar projeto de lei](#uc02-visualizar-projeto-de-lei)
3. [UC03 - Visualizar segmentos do projeto de lei](#uc03-visualizar-segmentos-do-projeto-de-lei)
4. [UC04 - Cadastrar usuário](#uc04-cadastrar-usuário)

***


#UC01: Cadastrar Usuário

 <b>Descrição:</b> Este caso de uso permite ao usuário se cadastrar no aplicativo.

<b>Ator principal:</b> Usuário visitante.

<b>Pré condições:</b> O usuário deve estar desconectado de uma conta antes de iniciar o cadastro.

<b>Fluxo principal:</b> Este caso de uso é iniciado quando o usuário escolhe a opção de cadastrar um novo usuário.

    1. O sistema redireciona o usuário para da tela de cadastro. [FA01]
    2. O usuário preenche campos com as informações necessárias para realizar o cadastro. [FA01]
    3. O usuário confirma a realização do cadastro. [FA01]
    4. O sistema valida os dados informados pelo usuário [RN01], [RN02], [FE01], [FA01].
    5. O sistema exibe uma mensagem de cadastro efetuado com sucesso.
    6. O usuário é redirecionado para a tela de log in.
    7. O caso de uso é encerrado.

<b>Fluxo alternativo FA01:</b>

    1. O usuário escolhe a opção de cancelar cadastro.
    2. O sistema vai para o passo 7 do fluxo principal.
  
<b>Pós condições:</b> Ao final do caso de uso, o usuário possuirá um cadastro no sistema.

<b>Regras de Negócio:</b>
#####<b>[RN01] - Cadastro de usuário:</b>

| Campo | Formato | Obrigatoriedade | Valor | 
| :---: | :---: | :---: | :---: |
| E-mail | String de até 150 caracteres | Sim | Padrão: exemplo@email.com O email não pode ser igual a um email já registrado |
| Primeiro nome | String de até 30 caracteres | Sim | |
| Ultimo nome | String de até 30 caracteres | Sim | |
| Senha | String de até 10 caracteres | Sim | Deve ter no mínimo 6 e no máximo 10 caracteres |
| Confirmação de senha | String de até 10 caracteres | Sim | Deve ser igual a senha digitada anteriormente |

#####<b>[RN02] -</b> O sistema permitirá apenas um e-mail por usuário no cadastro.

<b>Fluxo de exceção FE01:</b>
#####<b>[FE01] - Dados inválidos:</b> 
No passo 4 do fluxo principal, se o sistema identifica alguma informação inválida, o sistema exibe uma mensagem de dado inválido e retornará ao passo 1 do fluxo principal.

#UC02: Visualizar Projeto de Lei

 <b>Descrição:</b> Este caso de uso permite ao usuário visualizar projetos de lei, tendo mais informações sobre o projeto.

<b>Ator principal:</b> Usuário cadastrado ou Usuário visitante.

<b>Pré condições:</b> Não há.

<b>Fluxo principal:</b> Este caso de uso se inicia quando o usuário seleciona algum projeto de lei.

    1. O usuário clica em qual projeto de lei deseja visualizar.
    2. O Sistema redireciona o usuário para a tela da lei que foi selecionada.
    3. O Sistema apresenta as informações do projeto lei selecionado [RN01].
    4. O caso de uso é encerrado.

<b>Pós condições:</b> Não há.

<b>Regras de Negócio:</b>
#####<b>[RN01] - Informações da lei:</b>

| Informação da lei | Valor | 
| :---: | :---: |
| Lei selecionada | Proposta de lei que o usuário selecionou |
| Número | Número que identifica qual lei está sendo apresentada |
| Autor | Nome do autor que está propondo a lei |
| Relator | Nome de quem redigiu a lei |
| Número de participantes | Número de pessoas que já opinaram sobre a lei proposta |
|Número de propostas | Quantidade de opiniões dada sobre a lei |
|Data da contribuição | Até quando é possível opinar sobre a lei |


#UC03: Visualizar segmentos do projeto de lei

 <b>Descrição:</b> Este caso de uso permite ao usuário visualizar segmentos de um projeto de lei tendo mais informações sobre o segmento selecionado.

<b>Ator principal:</b> Usuário cadastrado ou Usuário visitante.

<b>Pré condições:</b> Não há.

<b>Fluxo principal:</b> Este caso de uso se inicia quando o usuário seleciona um segmento de algum projeto de lei.

    1. O usuário clica no segmento que deseja visualizar.
    2. O sistema redireciona o usuário para a tela do segmento selecionado [RN01].
    3. O sistema apresenta as informações do segmento selecionado [RN02].
    4. O caso de uso é encerrado.

<b>Pós condições:</b> Não há.

<b>Regras de Negócio:</b>
#####<b>[RN01] -</b> Os segmentos podem ser: Artigos, parágrafos, incisos, alínea e citação.
#####<b>[RN02] - Informações de segmentos:</b>

| Informação de segmento | Valor | 
| :---: | :---: |
| Segmento selecionado | Texto do segmento selecionado |
| Avaliações do segmento | Curtidas e descurtidas feitas pelos usuários no Segmento |
| Sugestões | Sugestões de propostas dos usuários para o Segmento |
| Relator | Nome de quem redigiu a lei |
| Avaliações de sugestões | Curtidas e descurtidas feitas pelos usuários nas sugestões |

#UC04: Listar projetos

 <b>Descrição:</b> Este caso de uso permite ao usuário listar projetos de lei de acordo com a ordem desejada , podendo ser por relevância, data e  status (abertos).

<b>Ator principal:</b> Usuário cadastrado ou Usuário visitante.

<b>Pré condições:</b> Não há.

<b>Fluxo principal:</b> O fluxo principal é iniciado quando o usuário seleciona uma combinação de modos de filtragem.

    1. O Usuário seleciona uma combinação dos modos de filtragem [RN02] [FE01].
    2. O Sistema reorganiza os projetos e lista ao usuário de acordo com o modo de filtragem.
    3. O caso de uso é encerrado.



<b>Fluxo Alternativo FA01:</b> É iniciado quando o usuário faz o login ou entra como visitante na aplicação.

    1. O sistema exibe ao usuário uma lista dos projetos encontrados [RN01] [FE01].
    2. O sistema volta ao passo 3 do fluxo principal.

<b>Pós condições:</b> Não há.

<b>Regras de Negócio:</b>
#####<b>[RN01]- </b>A ordem de exibição default da tela inicial é por projetos mais relevantes e abertos.
#####<b>[RN02] - Modos de filtragem:</b>

| Opção de filtragem | Valor | 
| :---: | :---: |
| Relevantes | Proposta de lei com maior quantidade de sugestões de propostas |
| Recentes | Proposta de lei com a data de criação mais recente |
| Abertos | Proposta de lei em aberto |
| Fechados | Proposta de lei fechada |

<b>Fluxo de exceção FE01:</b>

    1. Caso não existam projetos referentes a ordem definida.
    2. O sistema informa ao usuário que não há projetos.
    3. O sistema vai para o passo 3 do fluxo principal.

