# EXERCÍCIOS

## 1 – Preenchendo uma matriz simples
Uma escola deseja registrar a quantidade de alunos presentes em 2 salas durante 3 turnos (manhã, tarde e noite). Escreva um programa que leia os dados dessa frequência e exiba a tabela completa de presença.

Exemplo de saída:
```
Tabela de presencas:
Sala 1: 12 10 20
Sala 2: 10 8 7
```

## 2 – Somando elementos de uma matriz
Um banco quer somar todos os valores de uma matriz 2x3 que representa o valor arrecadado por 2 agências em 3 dias. Imprima o total arrecadado.

Exemplo de saída:
```
Agencia 1, Dia 1: 1890
Agencia 1, Dia 2: 12000
Agencia 1, Dia 3: 7000
Agencia 2, Dia 1: 976
Agencia 2, Dia 2: 123
Agencia 2, Dia 3: 80

Total arrecadado: R$22069
```

## 3 – Média por linha
Registre as notas de 3 alunos em 4 provas. Depois, calcule e exiba a média de cada aluno.

Exemplo de saída:
```
Aluno 1, Prova 1: 10
Aluno 1, Prova 2: 9.5
Aluno 1, Prova 3: 7
Aluno 1, Prova 4: 5.5

Media do aluno 1: 8.00

Aluno 2, Prova 1: 9
Aluno 2, Prova 2: 7.5
Aluno 2, Prova 3: 8.5
Aluno 2, Prova 4: 9

Media do aluno 2: 8.50

Aluno 3, Prova 1: 10
Aluno 3, Prova 2: 7.5
Aluno 3, Prova 3: 3.5
Aluno 3, Prova 4: 2.5

Media do aluno 3: 5.88
```

## 4 – Encontrar o maior número
Leia uma matriz 3x3 de inteiros. Depois, exiba o maior número presente nela.

Exemplo de saída:
```
10
20
23
24
31
90
55
68
75
Maior valor: 90
```

## 5 – Verificar se a matriz é simétrica
Uma matriz quadrada é simétrica se `matriz[i][j] == matriz[j][i]`. Leia uma matriz 3x3 e diga se ela é simétrica.

Exemplo de saída:
```
1
2
3
2
4
5
3
5
6
A matriz e simetrica? SIM
```

## 6 – Soma da diagonal principal
Dada uma matriz 4x4, exiba a soma da diagonal principal.

Exemplo de saída:
```
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
Soma da diagonal principal: 34
```

## 7 – Substituir valores negativos
Dada uma matriz 3x3 com valores inteiros (positivos e negativos), substitua os valores negativos por 0 e exiba a matriz corrigida.

Exemplo de saída:
```
10
20
-8
4
5
-3
-9
90
-2

Matriz corrigida:

| 10  20   0 |
|  4   5   0 |
|  0  90   0 |
```

## 8 – Contar elementos maiores que X
Leia uma matriz 3x3 e um número inteiro X. Conte e exiba quantos valores da matriz são maiores que X.

Exemplo de saída:
```
Digite o valor de X: 10
12
11
1
2
3
4
5
60
34
Quantidade de valores maiores que X: 4
```

## 9 – Transposta de uma matriz
Dada uma matriz 3x2, imprima a sua transposta (2x3).

Exemplo de saída:
```
Digite os 6 valores da matriz 3x2 (linha por linha):
Elemento [0][0]: 10
Elemento [0][1]: 12
Elemento [1][0]: 8
Elemento [1][1]: 7
Elemento [2][0]: 19
Elemento [2][1]: 20

Matriz original:

|  10  12 |
|   8   7 |
|  19  20 |

Matriz transposta:

|  10   8  19 |
|  12   7  20 |
```

## 10 – Verificação de matriz identidade
Uma matriz identidade é uma matriz quadrada onde os elementos da diagonal principal são 1 e os demais são 0. Escreva um programa que leia uma matriz 4x4, diga se ela é uma matriz identidade e exiba a matriz formatada.

Exemplo de saída:
```
1
0
0
0
0
1
0
0
0
0
1
0
0
0
0
1

Matriz identidade? SIM

  1   0   0   0
  0   1   0   0
  0   0   1   0
  0   0   0   1
```