# FUNÇÕES

>Imagine o Naruto usando o *Kage Bunshin no Jutsu* (Clone das Sombras) para várias tarefas. Cada clone faz uma tarefa diferente, mas todos têm o mesmo objetivo final: cumprir a missão.  
>Funções são como jutsus! São blocos de código que executam uma tarefa específica e podem ser reutilizados várias vezes.

Funções são usadas para reutilizar trechos de código.

## 1️⃣ Como escrever uma função

```c
tipo_retorno nome_funcao(parametros) {
    // bloco de código
    return valor; // se houver retorno
}
```

### EXEMPLO: Função que retorna a soma de dois números

```c
#include <stdio.h>

int somar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = somar(3, 5);
    printf("Resultado: %d\n", resultado);
    return 0;
}
```

## 2️⃣ Procedimentos (Funções que não retornam nada)

```c
void mostrarMensagem() {
    printf("O treino do Naruto está completo!\n");
}
```

>O tipo `void` é usado quando uma função não possui retorno. Ela é executada, porém não retorna nada.

Outro exemplo:

```c
#include <stdio.h>

// Função que mostra um menu (não retorna nada)
void exibirMenu() {
    printf("=== MENU DE OPÇÕES ===\n");
    printf("1 - Ver saldo\n");
    printf("2 - Fazer depósito\n");
    printf("3 - Fazer saque\n");
    printf("4 - Sair\n");
    printf("======================\n");
}

int main() {
    // Chamada da função
    exibirMenu();
    
    int opcao;
    printf("Escolha uma opção: ");
    scanf("%d", &opcao);

    printf("Você escolheu a opção %d.\n", opcao);
    return 0;
}
```

### EXEMPLO: Função que ordena um array usando o algoritmo `bubble sort`

```c
#include <stdio.h>

// Função que ordena o array em ordem crescente
void ordenar(int array[10]) {
    int temp;

    for (int i = 0; i < 10; i++) {
        for (int j = 0; j < 10 - i - 1; j++) {
            if (array[j] > array[j + 1]) {
                // troca os elementos
                temp = array[j];
                array[j] = array[j + 1];
                array[j + 1] = temp;
            }
        }
    }
}

int main() {
    int array[10] = {10, 7, 8, 3, 2, 4, 3, 2, 1, 0};

    ordenar(array); // ordena o array

    printf("Array ordenado:\n");
    for (int i = 0; i < 10; i++) {
        printf("%d ", array[i]);
    }

    return 0;
}
```