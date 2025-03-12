# Introdução a Programação e Primeiros Passos com VisualG

## 1. Introdução à Programação e Algoritmos
- O que é programação?
  - Programação é o processo de escrever instruções que um computador pode entender e executar.
  - Analogia: Assim como uma receita de bolo tem passos que devem ser seguidos na ordem correta, um programa de computador é um conjunto de instruções para realizar uma tarefa.

- O que são algoritmos?
  - Um algoritmo é uma sequência de passos bem definidos para resolver um problema.
  - Exemplo prático: Vamos criar um algoritmo para preparar uma caneca de chocolate quente. 
    - Passo 1: Pegar uma caneca
    - Passo 2: Pegar o leite
    - Passo 3: Esquentar o leite 
    - Passo 4: Colocar leite quente na caneca  
    - Passo 5: Adicionar o pó chocolate  
    - Passo 6: Misturar  
    - Passo 7: Beber  

- O que é Portugol e o VisualG?
  - Portugol é uma linguagem fictícia baseada no português usada para aprender lógica de programação.
  - VisualG é um software que nos permite escrever e testar códigos em Portugol.

## 2. Download do VisualG

🔗 Download: [VisualG](https://sourceforge.net/projects/visualg30/)

## 3. Estrutura Básica de um Programa no VisualG

```sh
algoritmo "primeiro_programa"
inicio
   escreva("Olá, mundo!")
fimalgoritmo
```

- Explicação:
  - `algoritmo "primeiro_programa"` → Define o início do programa.
  - `inicio` e `fimalgoritmo` → Delimitam o bloco principal do código.
  - `escreva("Olá, mundo!")` → Exibe texto na tela.

>**💡 Execute no VisualG para ver a saída**

## 4. Variáveis e Constantes
- O que são variáveis?
  - Uma variável é um espaço na memória do computador onde podemos armazenar um valor.
  - Analogia: Pense em uma variável como uma caixinha onde guardamos algo, como um número ou um nome.

- O que são constantes?
  - Uma constante é um valor que não muda durante a execução do programa.
  - Exemplo: O número de dias em uma semana é sempre 7.

- Tipos de dados no VisualG:
  | Tipo      | Descrição                  | Exemplo |
  |-----------|----------------------------|---------|
  | `inteiro` | Números inteiros            | 10, -5  |
  | `real`    | Números com casas decimais  | 3.14, -2.5 |
  | `caractere` | Textos                     | "João", "Corinthians" |
  | `logico`  | Valores `verdadeiro` ou `falso` | `verdadeiro`, `falso` |

## 5. Declarando e Utilizando Variáveis
**Exemplo de código:**
```sh
algoritmo "exemplo_variaveis"
var
   nome: caractere
   idade: inteiro
   altura: real
   maior_de_idade: logico
inicio
   nome <- "Yuri Alberto"
   idade <- 21
   altura <- 1.75
   maior_de_idade <- verdadeiro

   escreval("Nome: ", nome)
   escreval("Idade: ", idade)
   escreval("Altura: ", altura)
   escreval("Maior de idade? ", maior_de_idade)
fimalgoritmo
```

- **Explicação do código:**
  - `var` → Define as variáveis.
  - `nome <- "Carlos"` → Armazena um texto na variável `nome`.
  - `idade <- 20` → Armazena um número inteiro na variável `idade`.
  - `altura <- 1.75` → Armazena um número decimal na variável `altura`.
  - `maior_de_idade <- verdadeiro` → Define uma variável lógica.
  - `escreval(...)` → Exibe os valores na tela e pula uma linha.

>**💡 Execute no VisualG para ver a saída**

## 6. Operadores Matemáticos
Operadores matemáticos são símbolos usados para realizar operações como `soma`, `subtração`, `multiplicação` e `divisão`.

| Operador | Operação        | Exemplo       | Resultado |
|----------|----------------|--------------|-----------|
| `+`      | Adição         | `5 + 3`      | `8`       |
| `-`      | Subtração      | `10 - 4`     | `6`       |
| `*`      | Multiplicação  | `2 * 6`      | `12`      |
| `/`      | Divisão real   | `10 / 4`     | `2.5`     |
| `div`    | Divisão inteira | `10 div 4`   | `2`       |
| `%`      | Resto da divisão (módulo) | `10 % 4`  | `2`       |

>**💡 `div` retorna apenas a parte inteira da divisão, enquanto `/` retorna um valor com casas decimais.**

---

### Operações básicas
```sh
algoritmo "operadores_matematicos"
var
   a, b, soma, subtracao, multiplicacao: inteiro
   divisao: real
inicio
   a <- 10
   b <- 3

   soma <- a + b
   subtracao <- a - b
   multiplicacao <- a * b
   divisao <- a / b

   escreval("Soma: ", soma)
   escreval("Subtração: ", subtracao)
   escreval("Multiplicação: ", multiplicacao)
   escreval("Divisão: ", divisao)
fimalgoritmo
```

>**💡 Execute no VisualG para ver a saída**

### Divisão inteira e módulo
```sh
algoritmo "divisao_inteira_modulo"
var
   num1, num2, resultadoDiv, resto: inteiro
inicio
   num1 <- 10
   num2 <- 3

   resultadoDiv <- num1 div num2
   resto <- num1 % num2

   escreval("Divisão inteira: ", resultadoDiv)
   escreval("Resto da divisão: ", resto)
fimalgoritmo
```

### Precedência de Operadores
Assim como na matemática, as operações seguem uma ordem de precedência:

1. **Parênteses `()`** → Tem a maior prioridade.
2. **Multiplicação `*`, Divisão `/`, Divisão Inteira `div`, Módulo `%`** → Vêm antes da adição e subtração.
3. **Adição `+` e Subtração `-`** → São as últimas a serem resolvidas.

### Testando Precedência
```sh
algoritmo "precedencia_operadores"
var
   resultado1, resultado2, resultado3: inteiro
inicio
   resultado1 <- 10 + 2 * 5
   resultado2 <- (10 + 2) * 5
   resultado3 <- 10 + 2 * 5 - 3 div 2

   escreval("Resultado 1: ", resultado1) // 10 + (2 * 5) = 20
   escreval("Resultado 2: ", resultado2) // (10 + 2) * 5 = 60
   escreval("Resultado 3: ", resultado3) // 10 + (2 * 5) - (3 div 2) = 19
fimalgoritmo
```

>**💡 Execute no VisualG para ver a saída**
