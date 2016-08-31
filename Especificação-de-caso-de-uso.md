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
***

#Índice

1. [UC01 - Listar Projetos](#uc01-listar-projetos)
2. [UC02 - Visuaizar projeto de lei](#uc02-visualizar-projeto-de-lei)
3. [UC03 - Visualizar segmentos do projeto de lei](#uc03-visualizar-segmento)
4. [UC04 - Cadastrar usuário](#uc04-cadastrar-usuário)

***

#UC01: Listar projetos

 <b>Descrição:</b> Este caso de uso permite ao usuário listar projetos de lei de acordo com a ordem desejada , podendo ser por relevância, data e  status (abertos).

<b>Ator principal</b> Usuário cadastrado ou Usuário visitante.

<b>Pré condições:</b> Não há.

<b>Fluxo principal</b> O fluxo principal é iniciado quando o usuário seleciona uma combinação de modos de filtragem.
    <b>1</b>.O Usuário seleciona uma combinação dos modos de filtragem [RN02], [FE01].
    2.O Sistema reorganiza os projetos e lista ao usuário de acordo com o modo de filtragem.
    3.O caso de uso é encerrado.

<b>Pós condições:</b> Não há
