### Histórico de Versão

| Data | Versão | Descrição | Autor(es) |
| :---: | :---: | --- | :---: |
| 21/09/2016 | 1.0 | Criação do Documento e descrição dos tópicos | Pedro Ivo |

### Sumário

1. [Introdução](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#1-introdu%C3%A7%C3%A3o)
2. [Objetivo](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#2-objetivo)
3. [Rastreabilidade](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#3-rastreabilidade)
   * [3.1 Rastreabilidade Vertical](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#31-rastreabilidade-vertical)
4. [Considerações](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#4-considera%C3%A7%C3%B5es)
5. [Referências](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Rastreabilidade-de-Requisitos#5-refer%C3%AAncias)


# 1. Introdução

<p align="justify"></p>

<p align="justify">Uma das principais tarefas da gerência de requisitos é possibilitar a rastreabilidade dos requisitos durante o processo de Engenharia de Requisitos. Se a rastreabilidade de requisitos é feita com sucesso, tem-se um impacto positivo e percebe-se uma melhoria significativa no projeto, sendo então, considerada parte valiosa da Engenharia de software, (HOKKANEN, 2001).</p>

<p align="justify">Um requisito é considerado rastreável se para qualquer parte do produto pode-se identificar o requisito que o ocasionou. Segundo Gotel e Finkelstein (1994, p. 1), a Rastreabilidade de Requisitos se refere a habilidade de escrever e seguir a vida de um requisito, tanto para "trás", quanto para "frente", isto é, de sua origem até sua implementação e especificação e vice-versa.</p>

# 2. Objetivo

<p align="justify">De acordo com o <i>Rational Unified Process</i>, a finalidade de estabelecer a rastreabilidade de requisitos é ajudar a: (1) compreender a origem dos requisitos, (2) gerenciar o escopo do projeto, (3) gerenciar mudanças nos requisitos, (4) avaliar o impacto no projeto da mudança em um requisito, (5) avaliar o impacto da falha de um teste nos requisitos, (6) verificar se todos os requisitos do sistema são desempenhados pela implementação e (7) verificar se o sistema faz apenas o que era esperado que ele fizesse.</p>

# 3. Rastreabilidade

<p align="justify">Há várias classificações para se caracterizar a rastreabilidade de requisitos. As duas classificações analisadas  foram a rastreabilidade vertical e horizontal de requisitos. Segundo, (GOTEL; FINKELSTEIN, 1994), a  rastreabilidade vertical de requisitos refere-se à rastreabilidade entre fases seguintes ou anteriores na vida de um requisito no processo de desenvolvimento, enquanto que a rastreabilidade horizontal refere-se à análise entre versões e variantes de um requisito numa fase particular da vida do requisito.</p>

## 3.1 Rastreabilidade Vertical

<p align="justify"></p>

<p align="justify">A imagem a seguir, representa todos as necessidades, caracterísiticas e os requisitos encontrados para a implementação do projeto. A partir dos itens elicitados, realiza-se a relação entre eles para gerar a rastreabilidade vertical.</p>
![Requisitos cadastrados](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_tree.PNG)
<p align="center"><b>Figura 1:</b> Todas necessidades, características e requisitos encontrados.</p>

***

<p align="justify">As imagens a seguir definem a rastreabilidade encontrada entre as necessidades, caracterísiticas e requisitos do produto.</p>

![Contribuir com Projetos de Lei](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_tree1.PNG)
<p align="center"><b>Figura 2:</b> Rastreabilidade da necessidade Contribuir com Projetos de Lei.</p>

![Acompanhar o debate da sociedade acerca dos Projetos de lei](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_tree2.PNG)
<p align="center"><b>Figura 3:</b> Rastreabilidade da necessidade Acompanhar o debate da sociedade acerca dos Projetos de Lei.</p>

![Disseminar informações sobre os Projetos de Lei](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_tree3.PNG)
<p align="center"><b>Figura 4:</b> Rastreabilidade da necessidade Disseminar informações sobre os Projetos de Lei.</p>


***

<p align="justify">Outra forma de representar a rastreabilidade dos requisitos é a partir da matriz de rastreabilidade, onde se encontram todos itens elicitados e as relações que possuem entre si. As figuras abaixo representam a Matriz de Rastreabilidade.</p>

![Matriz de Rastreabilidade parte 1](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_matrix1.png)
<p align="center"><b>Figura 5:</b> Matriz de Rastreabilidade de Requisitos, parte 1.</p>

![Matriz de Rastreabilidade parte 2](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/rast_matrix2.png)
<p align="center"><b>Figura 6:</b> Matriz de Rastreabilidade de Requisitos, parte 2.</p>

# 4. Considerações

<p align="justify">Para melhor entendimento da matriz de rastreabilidade, considere as seguintes informações: (1) Um item é "pai" de outro se a seta contínua parte dele para outro item. (2) Um item é "filho" de outro se a seta contínua chega a ele a partir de outro item. (3) As setas tracejadas representam implicações, por exemplo, "Contribuir com Projetos de Lei" implicam em "Alterar Itens do Projeto de Lei", "Comentar Itens de um Projeto de Lei", detre outros.</p>

# 5. Referências

[1]. RAMESH, B. et al. Lessons learned from Implementing Requirements Traceability. [S.l.:s.n.], 1995.

[2]. HOKKANEN, M. Requirements traceability. 2001.

[3]. GOTEL, O.; FINKELSTEIN, A. An analysis of the requirements traceability problem. Imperial College of Science, Technology and Medicine, p. 27, 1994.

[4]. RUP. Rational Unified Process. Best Practices for Software Development Teams. IBM. July, 2001.
