# EXERCÍCIOS RESOLVIDOS

>⚠️ Tente resolver antes de olhar hein?? Tô de olho! 👀

## 1. Cadastro de Usuário 

```sh
algoritmo "CadastroUsuario"
var
   nome: caractere
   idade: inteiro
   cidade: caractere
inicio
   escreva("Digite seu nome: ")
   leia(nome)
   
   escreva("Digite sua idade: ")
   leia(idade)
   
   escreva("Digite sua cidade: ")
   leia(cidade)
   
   escreval("Olá ", nome, "! Você tem ", idade, " anos e mora em ", cidade, ".")
fimalgoritmo
```

## 2. Cálculo de Salário

```sh
algoritmo "CalculoSalario"
var
   salarioMensal, salarioAnual: real
inicio
   escreva("Digite seu salário mensal: ")
   leia(salarioMensal)
   
   salarioAnual <- salarioMensal * 12
   
   escreval("Seu salário anual é R$", salarioAnual, ".")
fimalgoritmo
```

## 3. Cálculo do IMC

```sh
algoritmo "CalculoIMC"
var
   peso, altura, imc: real
inicio
   escreva("Digite seu peso (kg): ")
   leia(peso)

   escreva("Digite sua altura (m): ")
   leia(altura)

   imc <- peso / (altura * altura)

   escreval("Seu IMC é", imc)

   se (imc < 18.5) entao
      escreval("Você está abaixo do peso.")
   senao
      se ((imc >= 18.5) e (imc <= 24.9)) entao
         escreval("Você está no peso ideal.")
      senao
         escreval("Você está acima do peso.")
      fimse
   fimse
fimalgoritmo
```

## 4. Validação de Senha 

```sh
algoritmo "ValidacaoSenha"
var
   senha: caracter
inicio
   escreva("Digite a senha: ")
   leia(senha)

   se (senha = "xablau") entao
      escreval("Acesso permitido!")
   senao
      escreval("Senha incorreta! Tente novamente.")
   fimse
fimalgoritmo
```

## 5. Loja de Descontos 

```sh
algoritmo "LojaDescontos"
var
   valorCompra, desconto, valorFinal: real
inicio
   escreva("Digite o valor total da compra: R$")
   leia(valorCompra)

   se (valorCompra <= 100) entao
      desconto <- 0
   senao
      se (valorCompra <= 200) entao
         desconto <- valorCompra * 0.10
      senao
         desconto <- valorCompra * 0.20
      fimse
   fimse

   valorFinal <- valorCompra - desconto

   escreval("Seu desconto foi de R$", desconto, ".")
   escreval("Valor final: R$", valorFinal, ".")
fimalgoritmo
```