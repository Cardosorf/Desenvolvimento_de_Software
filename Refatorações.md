# Introdução

Esta sessão da wiki tem como objetivo evidenciar, para os envolvidos com a matéria de GPP/MDS, segundo de 2016, as principais refatorações feitas no projeto Wikilegis mobile durante a segunda parte da disciplina, isto é, a relase 2, referente ao desenvolvimento ágil.

# Refatorações

### Melhoramento de métricas

* Ocorreu durante a Sprint 1 e 2;
* Foi criado um épico que suprisse esta necessidade: [Melhorar Métricas;](https://github.com/fga-gpp-mds/2016.2-WikiLegis/issues/12)
* Teve como objetivo melhorar as métricas de código referente a Release 1;
* Métricas a serem melhoradas: AMLOC e ACC;
    * [47a249c4991d43f3356b01a816ac273cf13883d6](https://github.com/fga-gpp-mds/2016.2-WikiLegis/commit/47a249c4991d43f3356b01a816ac273cf13883d6)
    * [146978d439e5df38bcace5ca1dbb843061f2d742](https://github.com/fga-gpp-mds/2016.2-WikiLegis/commit/146978d439e5df38bcace5ca1dbb843061f2d742)
    * [bd4344236b30282eb2502dd304103a2361624abd](https://github.com/fga-gpp-mds/2016.2-WikiLegis/commit/bd4344236b30282eb2502dd304103a2361624abd)

### Refatorações de View

* Ocorreu durante todas as sprints;
* Foi criado o épico para atender as essas refatorações: [Melhorar UX;](https://github.com/fga-gpp-mds/2016.2-WikiLegis/issues/15)
* Constantemente, durante a validação das funcionalidades com o cliente, o especialista em design do Wikilegis nos dava dicas de melhorar o design. Atendendo a vontade do cliente, durante a sprint seguinte a da reunião, nós colocamos refatorações de design;
    * [7e393fcfd099c516a0b0d08ef17645dfa1be46f6](https://github.com/izacristina/2016.2-WikiLegis/commit/7e393fcfd099c516a0b0d08ef17645dfa1be46f6)
    * [5f44a007910b1853b4ffdbc8e12ec396307e4629](https://github.com/izacristina/2016.2-WikiLegis/commit/5f44a007910b1853b4ffdbc8e12ec396307e4629)
    * [e6605ae14f1560377c89a5b598b4889f5babf991](https://github.com/izacristina/2016.2-WikiLegis/commit/e6605ae14f1560377c89a5b598b4889f5babf991)

### Refatorando testes

* Ocorreu durante a sprint 4, 5, 6
* Após algumas modificações no código, alguns testes de interface pararam de funcionar, necessitando de refatoração.
* Alguns exemplos são:
   * [28a25e06603a8148e17181c04f11815279edf7ad](https://github.com/izacristina/2016.2-WikiLegis/commit/28a25e06603a8148e17181c04f11815279edf7ad)
   * [ccc231e758bde194fa96295d2c4a4481ad3117dc](https://github.com/izacristina/2016.2-WikiLegis/commit/ccc231e758bde194fa96295d2c4a4481ad3117dc)
   * [6b10947c385f7cbe96d447abd6c79195ab0b5c1a](https://github.com/izacristina/2016.2-WikiLegis/commit/6b10947c385f7cbe96d447abd6c79195ab0b5c1a)

### Refatorando Requisições

* Durante a construção do backlog foi percebido, junto com o cliente, a necessidade de adicionar o comportamento ao sistema de, quando existir internet, utilizar somente internet, e quando não utilizar o banco;
* Foi realizada durante a sprint 4;
* Foi criada uma [história técnica](https://github.com/fga-gpp-mds/2016.2-WikiLegis/issues/44) de 13 para a realização dessa refatoração, tendo em vista que esta refatoração alteraria toda estrutura do código;
    * [0494036a44e545d3f2d883efd183d220987b87b5](https://github.com/izacristina/2016.2-WikiLegis/commit/0494036a44e545d3f2d883efd183d220987b87b5)
    * [9b675bf8c05042c713f3527a9dcd3e2fa82cd86f](https://github.com/izacristina/2016.2-WikiLegis/commit/9b675bf8c05042c713f3527a9dcd3e2fa82cd86f)
    * [a3d32fe3567e2934ba53d6e5e4b0907d181c4d12](https://github.com/izacristina/2016.2-WikiLegis/commit/a3d32fe3567e2934ba53d6e5e4b0907d181c4d12)

