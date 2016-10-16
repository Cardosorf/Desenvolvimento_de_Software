As métricas utilizadas para aferir a qualidade do projeto wikilegis Mobile foram determinadas através do documento [Plano de qualidade](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade).

Após a primeira release viu-se a necessidade de histórias técnicas para melhorar as métricas que deram acima do esperado:

* [TS10](https://github.com/fga-gpp-mds/2016.2-WikiLegis/issues/18)
* [TS11](https://github.com/fga-gpp-mds/2016.2-WikiLegis/issues/22)

Mas após começar a realiza-las foi visto que alcançar os valores determinados no [Plano de qualidade](https://github.com/fga-gpp-mds/2016.2-WikiLegis/wiki/Plano-de-gerenciamento-de-qualidade) estava demandando muito esforço. Então foi visto que talvez os valores esperados não eram realísticos.

Tendo como base as métricas colhidas da própria API do android 4.3.1 no artigo:

[1] Pereira (2015) Marcos Ronaldo Pereira Junior. **Estudo de métricas do código fonte no sistema Android e seus aplicativos**. Trabalho de termino de curso, Universidade de Brasilia [Link](http://bdm.unb.br/bitstream/10483/11317/1/2015_MarcosRonaldoPereiraJunior.pdf)

E considerando que métricas de OO não dependem do tamanho do código.[1]

Temos então os novos intervalos:

Para todo o código 0%:

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_0.png)

Para o percentil de 75%:

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_75.png)

Para o percentil de 95%:

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/valores_95.png)