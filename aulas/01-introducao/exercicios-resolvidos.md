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

### 4. Crie um algoritmo que calcule a área de um retângulo.

```sh
Algoritmo "AreaRetangulo"

Var
    base, altura, area : real

Inicio
    // Definição de valores
    base <- 10
    altura <- 5

    // Cálculo da área do retângulo
    area <- base * altura

    // Exibição do resultado
    escreval("Área do retângulo: ", area)
Fimalgoritmo
```

### 5. Crie um algoritmo que calcule a área de um círculo.

```sh
Algoritmo "AreaCirculo"

Var
    raio, area, numeroPi : real

Inicio
    // Definição de valores
    numeroPi <- 3.1415
    raio <- 7

    // Cálculo da área do círculo
    area <- numeroPi * (raio * raio)

    // Exibição do resultado
    escreval("Área do círculo: ", area)
Fimalgoritmo
```

### 6. Crie um algoritmo que calcule a área de um triângulo.

```sh
Algoritmo "AreaTriangulo"

Var
    base, altura, area : real

Inicio
    // Definição de valores
    base <- 8
    altura <- 6

    // Cálculo da área do triângulo
    area <- (base * altura) / 2

    // Exibição do resultado
    escreval("Área do triângulo: ", area)
Fimalgoritmo
```

### 7. Crie um algoritmo que calcule o IMC (Índice de Massa Corporal) de uma pessoa.

```sh
Algoritmo "CalculoIMC"

Var
    peso, altura, imc : real

Inicio
    // Definição de valores
    peso <- 112
    altura <- 1.85

    // Cálculo do IMC
    imc <- peso / (altura * altura)

    // Exibição do resultado
    escreval("O IMC calculado é: ", imc)
Fimalgoritmo
```