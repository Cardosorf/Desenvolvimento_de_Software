# 1. Objetivo do Plano de Gerenciamento dos Custos

<p align="justify">Este plano tem como objetivo explicar como será feita a gestão dos custos do projeto, deixando claras as técnicas utilizadas para medição e manutenção dos custos.</p>

# 2. Medição e avaliação dos Custos

# 2.1. Como Será Feita a Avaliação

<p align="justify">A avaliação dos custos do projeto será feita por meio da comparação entre 3 estimativas: Valor planejado, valor real e valor agregado. Como os custos de equipamentos e serviços não variam em nenhuma das 3 estimativas, não serão levados em consideração durante a comparação.</p>

# 2.2. Valor Planejado (VP)

<p align="justify">Para estimativa do valor planejado, é preciso estabelecer uma quantidade de horas a serem cumpridas semanalmente por cada membro das equipes de gerência e desenvolvimento. Para cada iteração, a quantidade de horas prevista por membro é multiplicada pela quantidade de membros da equipe. Ao fazer isso, obtém-se a quantidade total de horas trabalhadas pelas equipes no projeto. Por fim, para chegar ao valor planejado, basta multiplicar o total de horas trabalhadas no projeto pelo valor da hora trabalhada dos integrantes do grupo.</p>

# 2.3. Custo Real (CR)

<p align="justify">Para calcular o custo real do projeto, é necessário saber a quantidade de horas efetivamente trabalhadas pelas equipes de gerência e de desenvolvimento. Por isso, durante todo o projeto, cada integrante de ambas as equipes deverá registrar diariamente, em uma planilha compartilhada, a quantidade de horas que trabalhou no projeto. Dessa forma, com essa planilha devidamente preenchida, basta somar as horas trabalhadas por todos os membros do projeto em cada iteração e multiplicar pelo valor da hora trabalhada dos integrantes. O resultado será o custo real do projeto.</p>

# 2.4. Valor Agregado (VA)

<p align="justify">O valor agregado é calculado tendo como base o valor planejado. Durante cada iteração, é estimada uma porcentagem do quanto realmente foi feito em relação ao que havia sido planejado para aquela iteração. Com o cálculo da porcentagem terminado, basta pegar esse valor e multiplicar pelo valor planejado para aquela iteração. O resultado será o valor agregado do projeto.</p>

# 2.5. Resultado Esperado (RE)

<p align="justify">Ao fim dos cálculos, espera-se que o valor agregado e o valor real do projeto sejam os mesmos, sendo aceitável para o valor agregado uma margem de erro de até 7% acima ou abaixo do valor real. Alcançar esse resultado, é um indicativo de que o custo real do projeto condiz com o que foi prometido ao cliente. Além disso, espera-se também que o valor real do projeto não exceda em mais de 15% o valor planejado, o que poderia tornar o projeto insustentável.</p>

# 2.6. Variação dos custos (VC)

<p align="justify">A variação dos custos será calculada tirando-se a diferença entre o valor agregado e o custo real do projeto. Ela indica a relação entre o desempenho físico dos membros da equipe e os custos. O planejado é 
que a variação dos custos seja nula, sendo que uma variação negativa pode dificultar a recuperação do projeto.
<br>
Fórmula: VC = VA - CR.
</p>


# 2.7. Índice de desempenho dos custos (IDC)

<p align="justify">Possui como objetivo medir a eficiência de custos do trabalho executado. Ele é calculado tirando-se a razão entre o valor agregado e o custo real do projeto. Um valor de IDC menor que 1.0 indica um excesso de custo para o trabalho executado, enquanto um valor de IDC maior que 1.0 indica um desempenho de custo abaixo do limite até a data presente.
<br>
Fórmula: IDC = VA / CR
</p>