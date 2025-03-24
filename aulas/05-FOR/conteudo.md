# Estrutura de Repetição (for) em C  

## 1 - O que é uma Estrutura de Repetição? 
Antes de mergulharmos no código, precisamos entender o **problema que a repetição resolve**.  

**🔎 Situação do Mundo Real:**  
Imagine que um super-herói precisa realizar um **treinamento diário** por 10 dias. Se fôssemos escrever isso em código sem repetição, teríamos algo assim:  

```c
printf("Dia 1: Ta pago!\n");
printf("Dia 2: Ta pago!\n");
printf("Dia 3: Ta pago!\n");
// … até o dia 10
```

😱 **Isso é ineficiente e repetitivo!** Para resolver esse problema, usamos estruturas de repetição como o **`for`**.

## 2 - Sintaxe do `for` em C
O comando `for` é utilizado quando sabemos exatamente **quantas vezes** queremos repetir uma ação.  

### Estrutura Geral do `for`

```c
for (inicialização; condição; incremento) {
    // Bloco de código a ser repetido
}
```

💡 **Explicação dos Componentes:**  
1. **Inicialização** → Define uma variável de controle (`int index = 1;`)  
2. **Condição** → Diz até quando o laço deve continuar (`index <= 10;`)  
3. **Incremento** → Aumenta a variável de controle a cada iteração (`index++`)  

## 3 - Exemplo - Treinamento do Super-Herói 🦸‍♂️
Vamos usar o `for` para exibir 10 dias de treinamento de um herói.

```c
#include <stdio.h>

int main() {
    int dias;

    printf("Digite quantos dias de treinamento o heroi precisa fazer: ");
    scanf("%d", &dias);

    for (int index = 1; index <= dias; index++) {
        printf("Dia %d: Ta pago!\n", index);
    }

    printf("Treinamento concluido!\n");

    return 0;
}
```

## 4 - Exemplo - Contagem Regressiva para uma bomba explodir 💣
Nos filmes, muitas vezes existe um tempo para agir antes de uma bomba explodir! Vamos criar um código que faz uma contagem regressiva.

```c
#include <stdio.h>

int main() {
    printf("Contagem regressiva para a bomba explodir:\n");

    for (int index = 10; index >= 1; index--) {
        printf("%d...\n", index);
    }

    printf("🔥 BOOM!\n");

    return 0;
}
```