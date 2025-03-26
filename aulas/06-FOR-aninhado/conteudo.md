# Loops `for` Aninhados em C

## 1 - O que são loops `for` aninhados? 
Um **loop aninhado** acontece quando um **`for` está dentro de outro `for`**. O **loop externo** controla quantas vezes o **loop interno** será executado.  

🔹 **Analogia:**  
Imagine que um **time de super-heróis** precisa patrulhar **diferentes cidades**.  

- O **loop externo** representa **cada cidade** (passamos por todas as cidades).  
- O **loop interno** representa **cada herói patrulhando aquela cidade**.  

>📌 **Regra de ouro:**  
>O **loop interno** sempre executa **completamente** para cada execução do **loop externo**.  

## 2 - Estrutura de um Loop `for` Aninhado
```c
for (inicialização; condição; incremento) { 
    for (inicialização; condição; incremento) { 
        // Comandos dentro do loop interno
    }
}
```
🔹 O loop **externo** controla o número de repetições do loop **interno**.  
🔹 O loop **interno** executa todas as suas iterações antes do loop **externo** avançar.  

## Exemplo 1 – Tabela de Multiplicação  
Vamos imprimir a **tabuada completa de 1 a 5**, usando dois loops `for`.

🔹 **Loop externo:** Representa os números da tabuada (1 a 5).  
🔹 **Loop interno:** Multiplica o número do loop externo por valores de 0 a 10.

```c
#include <stdio.h>

int main() {
    for (int i = 1; i <= 5; i++) { // Loop externo (tabuada de 1 a 5)
        printf("\nTabuada do %d:\n", i);
        for (int j = 0; j <= 10; j++) { // Loop interno (multiplicação de 1 a 10)
            printf("%d x %d = %d\n", i, j, i * j);
        }
    }
    return 0;
}
```

## Exemplo 2 – Criando um Retângulo de Asteriscos `*`
O programa pede ao usuário um número `n` e imprime um **retângulo de `n x n` asteriscos (`*`)**.

🔹 **Loop externo:** Controla as **linhas**.  
🔹 **Loop interno:** Controla os **asteriscos** de cada linha.

```c
#include <stdio.h>

int main() {
    int n;

    printf("Digite um numero para o tamanho do escudo: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) { // Loop externo (linhas)
        for (int j = 1; j <= n; j++) { // Loop interno (colunas)
            printf("* ");
        }
        printf("\n"); // Pula para a próxima linha
    }
    return 0;
}
```

## Exemplo 3 – Pirâmide de `#`  
Vamos imprimir uma **pirâmide de hashtags**, onde cada linha terá um número crescente de hashtags.  

🔹 **Loop externo:** Controla as **linhas**.  
🔹 **Loop interno:** Controla **quantas hashtags aparecem por linha**.

```c
#include <stdio.h>

int main() {
    int numero;

    printf("Tamanho da piramide de hashtags: ");
    scanf("%d", &numero);

    for (int i = 1; i <= numero; i++) { // Loop externo (linhas)
        for (int j = 1; j <= i; j++) { // Loop interno (imprime ###)
            printf("# ");
        }
        printf("\n");
    }
    return 0;
}
```