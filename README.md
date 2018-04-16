Teste-Bingo
Teste de conhecimento e capacidade logica para avaliação de candidatos a desenvolvedor

Este é um teste de avaliação de capacidade de solução de problemas e conhecimento sobre algoritmos.

O Bingo é um jogo de azar, isto é, a chance de ganhar não está a associado a nenhuma habilidade dos jogadores exceto saber reconhecer na[s] cartela[s] os numeros sorteados.

Há diversos modelos de Bingo. O mais comum deles é o que possui bolas numeradas de 1 a 75 e as cartelas são formadas por blocos contendo numeros aleatorios. Estes numeros estão organizados em ordem aleatoria em linhas e colunas e na junção da coluna central com a linha central há um bloco onde não há numero para ser marcado.

Supomos que queiramos desenvolver um jogo de BINGO com as seguintes premissas.

* Bolas numeradas de 1 a 65
* As cartelas terão 5 colunas e 3 linhas.
* Há 2 formas de premiação. Uma quando uma linha é completada e outra quando toda a cartela é preenchida. Ambos só podem ocorrer uma vez.
* O numero de cartelas é limitado a 100 por rodada.
* A distribuição dos numeros é feita através da fórmula ***f(n) = (10.n + k)*** onde **n** é o indice da coluna iniciando em 0 (zero), sendo que **n** faz parte do conjunto *[0, x]*, onde **x** é o número de colunas menos 1 (um) **k** representa o deslocamento aleatorio. **k** faz parte do conjunto *[0,m]* e *m* é o maior deslocamento possível para uma coluna.

Com base nas premissas acima responda os questionamentos abaixo.

1.) Qual o valor que você definiria para ***m***. Explique.

2.) Descreva um algoritmo para gerar as cartelas. Voce pode utilizar suas proprias palavras ou pseudo-código.

3.) Escreva uma funcao (em codigo de qualquer linguagem ou pseudo-codigo) que faz o sorteio de um numero (bolinha).

4.) Imaginando criar todo o sistema do jogo, que inclui a geração das cartelas, o sorteio das bolinhas a verificação da cartela que primeiro preencheu uma linha e a primeira cartela a ser totalmente preenchida faça um planejamento da criação deste sistema. Indique que tecnologias seriam utilizadas (Banco de Dados, métodos, linguagens).

5.) Que tipos de problemas você acredita que poderiam surgir na implementação desta solução?





