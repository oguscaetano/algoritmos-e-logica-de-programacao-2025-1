# Fundamentos de Entrada, Operadores e Expressões em Algoritmos

## 1. Introdução a Entrada e Saída de Dados
Antes de realizarmos cálculos ou comparações, **precisamos interagir com o usuário**. Para isso, utilizamos os comandos de **entrada e saída de dados**.  

### 🖥️ Entrada de Dados (leia)
No VisualG/portugol, usamos o comando `leia()` para capturar informações digitadas pelo usuário.  

### 🖥️ Saída de Dados (escreva)
Utilizamos `escreva()` para exibir informações na tela.  

### Exemplo prático: Cadastro de usuário 
Imagine que você está criando um **sistema para um site de academia**. O usuário deve informar seu nome e idade para se cadastrar.  

```sh
algoritmo "cadastro_academia"
var
   nome: caractere
   idade: inteiro
inicio
   escreva("Digite seu nome: ")
   leia(nome)

   escreva("Digite sua idade: ")
   leia(idade)

   escreval("Cadastro realizado!")
   escreval("Olá ", nome, ", você tem", idade, " anos.")
fimalgoritmo
```

**📌 O que acontece aqui?**  
1. O programa solicita **entrada** do nome e da idade.  
2. Depois, **exibe na tela** os dados digitados.  

## 2. Operadores Matemáticos
Os **operadores matemáticos** permitem realizar cálculos dentro do programa.  

| Operador | Descrição | Exemplo |
|----------|----------|---------|
| `+` | Soma | `5 + 3 → 8` |
| `-` | Subtração | `10 - 4 → 6` |
| `*` | Multiplicação | `6 * 2 → 12` |
| `/` | Divisão real | `7 / 2 → 3.5` |
| `div` | Divisão inteira | `7 div 2 → 3` |
| `%` | Resto da divisão | `7 % 2 → 1` |

### Exemplo prático: Calculadora de desconto
Imagine um programa que calcula o **preço final de um produto após um desconto**.  

```sh
algoritmo "calculo_desconto"
var
   preco, desconto, preco_final: real
inicio
   escreva("Digite o preço do produto: R$")
   leia(preco)

   escreva("Digite o percentual de desconto: ")
   leia(desconto)

   preco_final <- preco - (preco * (desconto / 100))

   escreva("O preço com desconto é: R$", preco_final)
fimalgoritmo
```

**📌 O que acontece aqui?**  
1. O usuário digita o preço e o percentual de desconto.  
2. O programa **calcula o valor final** e exibe o resultado.  

## 3. Operadores Relacionais
Os **operadores relacionais** são usados para comparar valores.  

| Operador | Descrição | Exemplo |
|----------|----------|---------|
| `=` | Igualdade | `5 = 5` (Verdadeiro) :white_check_mark:|
| `<>` | Diferente | `3 <> 5` (Verdadeiro) :white_check_mark:|
| `>` | Maior que | `10 > 7` (Verdadeiro) :white_check_mark:|
| `<` | Menor que | `4 < 6` (Verdadeiro) :white_check_mark:|
| `>=` | Maior ou igual | `3 >= 5` (Falso) ❌|
| `<=` | Menor ou igual | `2 <= 3` (Verdadeiro) :white_check_mark:|

### Exemplo prático: Entrada de cinema
Um programa verifica se a pessoa tem idade suficiente para assistir a um filme proibido para menores de 18 anos.  

```sh
algoritmo "entrada_cinema"
var
   idade: inteiro
inicio
   escreva("Digite sua idade: ")
   leia(idade)
   
   se (idade >= 18) entao
      escreva("Você pode assistir ao filme.")
   senao
      escreva("Acesso negado! Apenas para maiores de 18 anos.")
   fimse
fimalgoritmo
```

**📌 O que acontece aqui?**  
- O programa **verifica se a idade é maior ou igual a 18**.  
- Se for **verdadeiro**, permite a entrada. Caso contrário, **nega o acesso**.  

## 4. Operadores Lógicos
Os operadores lógicos são usados para combinar condições em decisões.  

| Operador | Descrição | Exemplo |
|----------|----------|---------|
| `e` | Ambas as condições devem ser verdadeiras | `(idade >= 18) e (ingresso = verdadeiro)` |
| `ou` | Pelo menos uma condição deve ser verdadeira | `(tempo >= 25) ou (pressao >= 180)` |
| `não` | Inverte o resultado da condição (negação) | `não (chovendo = verdadeiro)` |

### Exemplo prático: Controle de acesso ao parque
O parque só permite a entrada de **pessoas com mais de 12 anos ou acompanhadas por um responsável**.  

```sh
algoritmo "entrada_parque"
var
   idade: inteiro
   acompanhado: logico
inicio
   escreva("Digite sua idade: ")
   leia(idade)

   escreva("Está acompanhado de um responsável? (VERDADEIRO ou FALSO): ")
   leia(acompanhado)

   se (idade >= 12) ou (acompanhado = verdadeiro) entao
      escreva("Entrada permitida! Divirta-se no parque.")
   senao
      escreva("Entrada negada!")
   fimse
fimalgoritmo
```

**📌 O que acontece aqui?**  
- A entrada é permitida **se a idade for maior ou igual a 12** `OU` **se estiver acompanhado**.  

## 5. Precedência de Operadores
Assim como na matemática, as expressões em algoritmos seguem uma ordem de precedência:  

1️⃣ **Parênteses** `( )`  
2️⃣ **Multiplicação e Divisão** `*`, `/`, `div`, `%`  
3️⃣ **Soma e Subtração** `+`, `-`  
4️⃣ **Operadores relacionais** `<`, `>`, `<=`, `>=`, `=`, `<>`  
5️⃣ **Operadores lógicos** `não`, `e`, `ou`  

### Exemplo prático: Cálculo de média ponderada
```sh
algoritmo "media_ponderada"
var
   nota1, nota2, peso1, peso2, media: real
inicio
   escreva("Digite a primeira nota: ")
   leia(nota1)
   
   escreva("Digite o peso da primeira nota: ")
   leia(peso1)
   
   escreva("Digite a segunda nota: ")
   leia(nota2)
   
   escreva("Digite o peso da segunda nota: ")
   leia(peso2)
   
   media <- (nota1 * peso1 + nota2 * peso2) / (peso1 + peso2)
   
   escreva("A média ponderada é: ", media)
fimalgoritmo
```

**📌 Importância dos parênteses**  
>Se **não usarmos parênteses**, o cálculo poderia ser **errado** devido à precedência.  