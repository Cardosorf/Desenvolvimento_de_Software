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

##AMLOC (Tamanho médio dos métodos por classe)
<p align="justify">Como descrito no plano de qualidade os valores aceitáveis para AMLOC é 10, Bom . O resultado obtido foi excelente dentro do percenti 0%, mas ruim nos outros dois. Isso quer dizer que há uma quantidade considerável de classes com grandes número de linhas por método. Isso ocorre pela linguagem, java, que normalmente usa muitas linhas, mas também que a equipe não se preocupou tanto com isso durante o desenvolvimento. Para a próxima interação deve ser chamada a atenção afim de melhorar esse aspecto do código.</p>

##COF (Fator de acoplamento)
<p align="justify"> Esse indicador indica que o que já era esperado olhando para a métrica de ACC no percentil 95%, que deve se ter atenção, principalmente com a classe citada.

# Análise

![legenda](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/legenda.png)

# Métricas de Estilo e Design

<p align="justify">Foram encontrados alguns erros de estilo e design no último dia de coleta de dados. Tais erros ocorreram principalmente por ajustes finais nas classes de requisição de dados, nas Daos, que foram modificadas até pouco antes do fechamento do Git. Outro erro encontrado, não se refere a design mas a boas práticas de programação, a exemplo, os números mágicos, em que, serão refatorados e explicado a equipe de desenvolvimento como evitar esse tipo de warning da ferramenta CheckStyle.</p>

![](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time01-WikiLegis/imagens/iteracao3_checkstyle.png)
<p align="center">Tabela com os erros reportados pelo CheckStyle em sua devida classe</p>
