## 1. Histórias de Usuário
### US01 - Realizar Login

**Eu, como** cidadão visitante

**Desejo** realizar login no aplicativo

**Para** acessar as funcionalidades que exigem identificação

_Pontos:_ 8 pontos

_Epico:_ GERENCIAR USUARIO

### US02 - Editar Perfil
**Eu, como** cidadão registrado

**Desejo** editar o meu perfil

**Para** manter minhas informações atualizadas

_Pontos:_ 3 pontos

_Epico:_ GERENCIAR USUARIO

### US03 - Pesquisar Projetos
**Eu, como** cidadão 

**Desejo** pesquisar projetos 

**Para** acessar os projetos de meu interesse mais rapidamente

_Pontos:_ 5 pontos

_Epico:_ MELHORAR UX

### US04 - Sugerir proposta de alteração
**Eu, como** cidadão registrado

**Desejo** escrever uma proposta de alteração em um segmento

**Para** exercer minha cidadania

_Pontos:_ 8 pontos

_Epico:_ EXPRESSAR OPINIÃO

### US05 - Relatar Erro
**Eu, como** cidadão

**Desejo** relatar erros nos projetos de lei 

**Para** contribuir com a integridade dos projetos de lei

_Epico:_ COMUNICAÇÃO EXTERNA

_Pontos:_ 5 pontos

### US06 - Visualizar informações sobre o aplicativo
**Eu, como** cidadão

**Desejo** visualizar informações sobre o aplicativo

**Para** entender seu propósito e funcionamento

_Pontos:_ 1 ponto

_Epico:_ MELHORAR UX

### US07 - Avaliar segmento
**Eu, como** cidadão registrado

**Desejo** expressar minha opinião através de curtidas

**Para** dar feedback ao parlamentar sobre o segmento.

_Pontos:_ 5 pontos

_Epico:_ EXPRESSAR OPINIÃO

### US08 - Compartilhar projeto
**Eu, como** cidadão registrado

**Desejo** compartilhar um projeto de lei

**Para** que outras pessoas possam acessá-lo

_Pontos:_ 5 pontos

_Epico:_ COMUNICAÇÃO EXTERNA

### US09 - Comentar Segmento
**Eu, como** cidadão registrado

**Desejo** comentar projetos de lei e seus segmentos

**Para** expressar sua opinião em relação a ele

_Pontos:_  5 pontos

_Epico:_ EXPRESSAR OPINIÃO

### US10 - Compartilhar segmento
**Eu, como** cidadão registrado

**Desejo** compartilhar informações sobre os segmentos de um projeto de lei

**Para** que outras pessoas possam acessá-los

_Pontos:_  3 pontos

_Epico:_ COMUNICAÇÃO EXTERNA

### US11 - Ativar notificações de um projeto de lei
**Eu, como** cidadão registrado

**Desejo** ativar notificações de um projeto de lei

**Para** para acompanhar contribuições e alterações nele

_Pontos:_  8 pontos

_Epico:_ COMUNICAÇÃO EXTERNA

### US12 - Ativar notificações de um segmento
**Eu, como** cidadão registrado

**Desejo** ativar notificações de um segmento do projeto de lei

**Para** para acompanhar contribuições e alterações nele

_Pontos:_  5 pontos

_Epico:_ COMUNICAÇÃO EXTERNA

### US13 - Baixar dados
**Eu, como** cidadão

**Desejo** ter a opção de baixar todos os dados

**Para** utilizar a aplicação offline

_Pontos:_  5 pontos

_Epico:_ DISPONIBILIZAR DADOS OFFLINE

Critérios de aceitação:

* O usuário deve ter a opção de baixar ou não.
* O usuário deve ter a opção de baixar somente no wifi ou no wifi e nos dados móveis.


## 2. Histórias Técnicas

### TS01 - Testar View
**Eu, como** desenvolvedor

**Desejo** testar o pacote view

**Para** aumentar a cobertura de código

_Pontos:_  5 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS02 - Testar DAO
**Eu, como** desenvolvedor

**Desejo** testar o pacote DAO

**Para** aumentar a cobertura de código

_Pontos:_  8 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS03 - Testar Model
**Eu, como** desenvolvedor

**Desejo** testar o pacote Model

**Para**aumentar a cobertura de código

_Pontos:_  2 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS04 - Testar Controller
**Eu, como** desenvolvedor

**Desejo** testar o pacote Controller

**Para** aumentar a cobertura de código

_Pontos:_  5 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS05 - Aplicar folha de estilo
**Eu, como** desenvolvedor

**Desejo** refatorar o código

**Para** padronizá-lo segundo a folha de estilo

_Pontos:_  1 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS06 - Refatorar design de filtragem
**Eu, como** desenvolvedor

**Desejo** refatorar o design da filtragem de projetos

**Para** tornar a  interface mais intuitiva

_Pontos:_  8 pontos

_Epico:_ Melhorar UX

### TS07 - Restringir orientação da tela
**Eu, como** desenvolvedor

**Desejo** restringir o design da aplicação para funcionar apenas em retrato

**Para** evitar problemas de responsividade

_Pontos:_  1 pontos

_Epico:_ Melhorar UX

### TS08 - Refatorar lista de projetos
**Eu, como** desenvolvedor

**Desejo** que os títulos dos projetos de lei e segmentos não sejam clicáveis

**Para** melhorar a usabilidade da aplicação

_Pontos:_  3 pontos

_Epico:_ Melhorar UX

### TS09 - Melhorar desempenho da tela de cadastro
**Eu, como** desenvolvedor

**Desejo** otimizar a tela de cadastro

**Para** permitir que ela responda mais rápido

_Pontos:_  5 pontos

_Epico:_ Melhorar UX

### TS10 - Melhorar AMLOC
**Eu, como** desenvolvedor

**Desejo** refatorar o código

**Para**  melhorar a métrica de AMLOC (Média de Linhas por Método)

_Pontos:_  2 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS11 - Melhorar ACC
**Eu, como** desenvolvedor

**Desejo** refatorar o código

**Para** melhorar a métrica de ACC (Média de Conexões Aferentes)

_Pontos:_  5 pontos

_Epico:_ MELHORAR MÉTRICAS

### TS12 - Refatorar download de dados
**Eu, como** desenvolvedor

**Desejo** refatorar o download de dados

**Para** quando houver internet, baixar os dados através de requisições

_Pontos:_  13 pontos

_Epico:_ MELHORAR UX

Critérios de aceitação:

* Caso não tenha os dados, estes devem ser baixados em background.
* Baixar somente os dados que passaram a existir após o ultimo download.