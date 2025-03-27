# Exercícios

## 1 - Tabuada 
Escreva um programa que exiba a **tabuada de multiplicação** do 1 ao 10.

Exemplo de saída:

```
Tabuada do 1
--------------
1 x 0 = 0
1 x 1 = 1
1 x 2 = 2
1 x 3 = 3
...
1 x 10 = 10

Tabuada do 2
--------------
2 x 0 = 0
2 x 1 = 2
```

## 2 – Quadrado de Asteriscos  
Escreva um programa que peça ao usuário um número `N` e desenhe um **quadrado de asteriscos (`*`)** com tamanho `N x N`.  

Exemplo de `N` = 4:
```
* * * *
* * * *
* * * *
* * * *
```

## 3 – Triângulo de Números 
Escreva um programa que exiba um **triângulo numérico** com `N` linhas, onde cada linha tem os números de 1 até a posição atual (N).

Exemplo de `N` = 5:
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

## 4 - Triângulo invertido de números 
Crie um programa que **imprima um triângulo invertido de números**.  

🔹 O usuário entra com um número `N`.  
🔹 A saída esperada, para `N = 5`, seria:
```
1 2 3 4 5
1 2 3 4
1 2 3
1 2
1
```

## 5 – Xadrez de Asteriscos 
Escreva um programa que gere um **padrão de tabuleiro de xadrez** de tamanho `N x N`, alternando `#` e ` ` (espaços). 

Exemplo de `N` = 5:
```
# # # 
 # #   
# # # 
 # #   
# # # 
```

## 6 – Pirâmide de Números Pares  
Escreva um programa que exiba uma **pirâmide de números pares** com `N` linhas.  

Exemplo de saída se `N` for 10:
```
2
4 6
8 10 12
14 16 18 20
22 24 26 28 30
32 34 36 38 40 42
44 46 48 50 52 54 56
58 60 62 64 66 68 70 72
74 76 78 80 82 84 86 88 90
92 94 96 98 100 102 104 106 108 110
```

## 7 - Controle de Estoque no Supermercado 
O supermercado deseja controlar o estoque de seus produtos e verificar quais precisam ser repostos. O programa deve:  
1. Pedir ao usuário quantos produtos ele deseja cadastrar.  
2. Para cada produto, solicitar:  
   - Nome do produto  
   - Quantidade em estoque  
   - Estoque mínimo recomendado  
3. Exibir imediatamente se o produto precisa de reposição ou não.  

Exemplo:
```
Digite a quantidade de produtos a serem cadastrados: 3

Produto 1:
Nome do produto: Nescau
Quantidade em estoque: 10
Estoque mínimo recomendado: 20
-> O produto 'Nescau' precisa ser reposto! (Estoque: 10, Mínimo: 20)

Produto 2:
Nome do produto: Laranja
Quantidade em estoque: 7
Estoque mínimo recomendado: 4
-> O produto 'Laranja' tem estoque suficiente. (Estoque: 7, Mínimo: 4)

Produto 3:
Nome do produto: Abobrinha
Quantidade em estoque: 8
Estoque mínimo recomendado: 90
-> O produto 'Abobrinha' precisa ser reposto! (Estoque: 8, Mínimo: 90)
```

## 8 - Controle de Revisão de Carros  
Uma concessionária deseja criar um sistema para registrar os carros que entram para revisão e verificar quais precisam de reparos urgentes. O sistema deve:  

1. Pedir ao usuário quantos carros serão registrados.  
2. Para cada carro, solicitar:  
   - **Modelo**  
   - **Ano de fabricação**   
   - **Se está funcionando normalmente** (`1` ou `0`).  
3. Exibir uma mensagem indicando se o carro está em boas condições ou se precisa de reparos urgentes (se for muito antigo ou estiver com problemas).  

- Se o ano for menor que 2005 e o carro não estiver funcionando normalmente, então, retorne `"O carro X precisa de REPAROS URGENTES!"`.
- Se o ano for menor que 2005 e o carro estiver funcionando normalmente, então, retorne `"O carro X é antigo, recomenda-se uma revisão!"`.
- Se o ano for igual ou maior que 2005 e não estiver funcionando normalmente, então, retorne `"O carro X precisa de manutenção!"`.
- Se o ano for igual ou maior que 2005 e estiver funcionando normalmente, então, retorne `"O carro X está em boas condições!"`.

## 9 - Catálogo de Séries da Netflix 
A Netflix deseja criar um sistema para recomendar séries aos usuários com base na **nota média** que elas receberam. O sistema deve:  

1. **Pedir ao usuário** quantas séries ele deseja cadastrar.  
2. Para **cada série**, solicitar:  
   - **Nome da série** (até 50 caracteres)  
   - **Quantidade de avaliações**  
   - As **notas dadas pelos usuários** (valores entre 0 e 10).  
3. **Calcular a média das notas** para cada série e classificar:  
   - **Média ≥ 8.0** → "Super Recomendada 🔥"  
   - **Média ≥ 5.0 e < 8.0** → "Boa 👍"  
   - **Média < 5.0** → "Ruim 👎"  
4. **Exibir a lista de séries com sua classificação.**  

Exemplo de saída:
```
Quantas series deseja cadastrar? 2

Digite o nome da serie 1: Stranger Things
Quantas avaliacoes essa serie recebeu? 3
Digite a nota 1 (0 a 10): 9
Digite a nota 2 (0 a 10): 8
Digite a nota 3 (0 a 10): 7

--- Detalhes da Serie ---
Nome: Stranger Things
Media das notas: 8.00
Classificacao: Super Recomendada 🔥
--------------------------

Digite o nome da serie 2: The Witcher
Quantas avaliacoes essa serie recebeu? 2
Digite a nota 1 (0 a 10): 5
Digite a nota 2 (0 a 10): 6

--- Detalhes da Serie ---
Nome: The Witcher
Media das notas: 5.50
Classificacao: Boa 👍
--------------------------
```

## 10 - Triângulo de asteriscos ***
Faça um programa que leia um número `N` e imprima um triângulo de asteriscos com altura `N` e largura `2N-1`.

Exemplo de N = 4:
```
   *   
  ***  
 ***** 
*******
```