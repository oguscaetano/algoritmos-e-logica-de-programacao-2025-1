# Exercícios Resolvidos

### 1. Escreva um programa que declare variáveis para armazenar:
   - O nome de uma pessoa
   - Sua idade
   - Sua altura
   - Se ela está estudando programação (`verdadeiro` ou `falso`)  
   - Exibir as informações na tela.

```sh
algoritmo "dados_pessoa"
var
   nome: caractere
   idade: inteiro
   altura: real
   estudando_programacao: logico
inicio
   // Atribuindo valores
   nome <- "Carlos"
   idade <- 20
   altura <- 1.75
   estudando_programacao <- verdadeiro

   // Exibindo os valores
   escreval("Nome: ", nome)
   escreval("Idade: ", idade)
   escreval("Altura: ", altura)
   escreval("Está estudando programação? ", estudando_programacao)
fimalgoritmo
```

### 2. Crie um programa que calcule o dobro de um número. 

```sh
algoritmo "dobro_numero"
var
   numero, dobro: inteiro
inicio

   numero <- 5
   dobro <- numero * numero

   escreval("O dobro de", numero, " é", dobro, ".")
fimalgoritmo
```

### 3. Crie um programa que recebe dois números e exiba:
   - A soma
   - A subtração
   - A multiplicação
   - A divisão real
   - A divisão inteira
   - O resto da divisão

```sh
algoritmo "calculadora_simples"
var
   num1, num2: inteiro
   soma, subtracao, multiplicacao, divInt, resto: inteiro
   divisaoReal: real
inicio
   num1 <- 10
   num2 <- 2

   // Realizando os cálculos
   soma <- num1 + num2
   subtracao <- num1 - num2
   multiplicacao <- num1 * num2
   divisaoReal <- num1 / num2
   divInt <- num1 div num2
   resto <- num1 % num2

   // Exibindo os resultados
   escreval("Soma: ", soma)
   escreval("Subtração: ", subtracao)
   escreval("Multiplicação: ", multiplicacao)
   escreval("Divisão real: ", divisaoReal)
   escreval("Divisão inteira: ", divInt)
   escreval("Resto da divisão: ", resto)
fimalgoritmo
```
