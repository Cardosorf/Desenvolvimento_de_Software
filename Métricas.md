A métricas serão coletadas e disponibilizadas aqui, junto com um breve relatório.
# Cobertura de teste
![cobertura](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/cobertura.png)
<p align="justify">Como foi dito no plano de qualidade a cobertura a meta para a primeira release é ter cobertua acima de 30%, e como evidenciado na imagem acima o objetivo foi alcançado.</p>
# Métricas de código fonte
## Terceira Interação
![metricas](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/metrics_v1.png)
### ACCM (Complexidade Ciclomática)
<p align="justify">Como descrito no plano de qualidade os valores aceitáveis para complexidade ciclomática é 0 - 3 Exelente e 3 - 5 Bom. O resultado obtido foi excelente dentro dos três percentis. Isso pode ser justificado pela baixa complexidade do projeto de software Wikilegis mobile.</p>
##ACC (Conexões aferentes)

<p align="justify">Como descrito no plano de qualidade os valores aceitáveis para conexões aferentes é 0 - 2, ou seja, bom. O resultado obtido para os percentis 0% e 75% foram "bom" e 95% foi "regular". Ao analisar os valores individuais de cada classe foi encontrada uma classe com o valor ACC absurdo de 31 ( Dao/DaoUtilities.java) e outras duas Bill(6) e Segment(4). O fato de serem poucas classes não influenciaram no resultado dos percentis baixos, o que evidencia a necessidade de rodar com vários percentis a fim de ter resultados relevantes.</p>

##LCOM4 (Falta de coesão entre métodos)
<p align="justify">Como descrito no plano de qualidade os valores aceitáveis para LCOM4 é 1 à 3. O resultado obtido foi excelente dentro dos três percentis. Isso pode ser justificado pela baixa complexidade do projeto de software Wikilegis mobile.</p>

# Análise
![legenda](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/legenda.png)

# Métricas de Estilo e Design

<p align="justify">Foram encontrados alguns erros de estilo e design no último dia de coleta de dados. Tais erros ocorreram principalmente por ajustes finais nas classes de requisição de dados, nas Daos, que foram modificadas até pouco antes do fechamento do Git. Outro erro encontrado, não se refere a design mas a boas práticas de programação, a exemplo, os números mágicos, em que, serão refatorados e explicado a equipe de desenvolvimento como evitar esse tipo de warning da ferramenta CheckStyle.</p>

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/iteracao3_checkstyle.png)
<p align="center">Tabela com os erros reportados pelo CheckStyle em sua devida classe</p>
