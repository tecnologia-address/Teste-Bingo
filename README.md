# Teste-Bingo #
Teste de conhecimento e capacidade logica para avaliação de candidatos a desenvolvedor

Este é um teste de avaliação de capacidade de solução de problemas e conhecimento sobre algoritmos.

O Bingo é um jogo de azar, isto é, a chance de ganhar não está a associado a nenhuma habilidade dos jogadores exceto saber reconhecer na[s] cartela[s] os numeros sorteados.

Há diversos modelos de Bingo. O mais comum deles é o que possui bolas numeradas de 1 a 75 e as cartelas são formadas por blocos contendo numeros aleatorios. Estes numeros estão organizados em ordem aleatoria em linhas e colunas e na junção da coluna central com a linha central há um bloco onde não há numero para ser marcado.

Supomos que queiramos desenvolver um jogo de BINGO com as seguintes premissas.

* Bolas numeradas de 1 a 65
* As cartelas terão 5 colunas e 3 linhas.
* Há 2 formas de premiação. Uma quando uma linha é completada e outra quando toda a cartela é preenchida. Ambos só podem ocorrer uma vez.
* O numero de cartelas é limitado a 100 por rodada.
* A distribuição dos numeros será feita através da fórmula  
 - ***f(n) = (m.n + k)*** 
 * Na formula **n** é o indice da coluna iniciando em 0 (zero).
* **k** representa o deslocamento aleatorio para cada número da cartela e faz parte do conjunto ***[1, m]*** 
* **m** é o maior deslocamento possível para uma coluna.
 
Com base nas premissas acima responda os questionamentos abaixo.

    NOTA: A intenção do teste nao é ter respostas certas, pois existem diferentes 
    formas de se responder corretamente. Antes de efetuar qualquer pesquisa tente 
    responder apenas com seus conhecimentos. Após terminar de responder, anote as 
    dificuldades que enfrentou para responder e os conhecimentos que porventura 
    tenha adquirido e coloque junto com suas respostas.

1.) Qual o valor de ***m***.

2.) Quantas posições cada cartela terá?

2.) Descreva um algoritmo para gerar as cartelas. Voce pode utilizar suas proprias palavras ou pseudo-código.

3.) Escreva uma funcao (em codigo de qualquer linguagem ou pseudo-codigo) que faz o sorteio de um numero (bolinha).

4.) Imaginando criar todo o sistema do jogo, que inclui a geração das cartelas, o sorteio das bolinhas a verificação da cartela que primeiro preencheu uma linha e a primeira cartela a ser totalmente preenchida faça um planejamento da criação deste sistema. Indique que tecnologias seriam utilizadas (Banco de Dados, métodos, linguagens).

5.) Que tipos de problemas você acredita que poderiam surgir na implementação desta solução?


    DICAS:
    - Para definir o deslocamento máximo aleatório devemos imaginar que cada coluna terá um grupo
    de números a serem sorteados. Se tivessemos bolas de 1 a 90 e quisessemos divir aleatoriamente 
    mas de forma uniforme os numeros em 5 linha de 5 numeros com o centro vazio (total de 24 posições), 
    a primeira coluna teria numeros de **1** a **m**, a segunda de **2.m + 1** a **2.m + k** e assim por 
    diante até que a ultima coluna teria numeros de **m.n + 1** a **90**.
    - **m** é definido usando a formula **m = x/n** onde **x** é a quantidade de bolinhas e **n** é o 
    numero de colunas, portanto para o atual exemplo **m = 18**.
    - A primeira coluna de uma cartela desse nosso BINGO terá numeros de **1** a **18**.
    - A ultima coluna (quinta) terá os numeros **f(4) = (18.4) + k**.
    - Para qualquer coluna do exemplo, o menor valor de **k** será **1** e o maior valor de **k** será igual a **m** (pois **k** pertence a **[1, m]**).   

