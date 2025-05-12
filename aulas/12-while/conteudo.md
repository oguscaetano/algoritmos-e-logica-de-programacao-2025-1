# O loop `while`

## 🧠 Como funciona?

O `while` **verifica a condição primeiro**. Se for verdadeira, executa o bloco. Ele pode **nem rodar nenhuma vez** se a condição começar falsa.

## 🧩 Sintaxe:

```c
while (condição) {
    // bloco de código
}
```

## 🧪 Exemplo:

```c
#include <stdio.h>

int main() {
    int contador = 1;

    while (contador <= 5) {
        printf("Contando: %d\n", contador);
        contador++; // incremento
    }

    return 0;
}
```

# O loop `do...while`

## 🧠 Como funciona?

O `do...while` **executa o bloco pelo menos uma vez**, depois **verifica a condição**.

## 🧩 Sintaxe:

```c
do {
    // bloco de código
} while (condição);
```

## 🧪 Exemplo:

```c
#include <stdio.h>

int main() {
    int senha;

    do {
        printf("Digite a senha correta (1234): ");
        scanf("%d", &senha);
    } while (senha != 1234);

    printf("Acesso liberado!\n");

    return 0;
}
```

## 🤔 Quando usar qual?

| Tipo de Loop | Quando Usar                                                                                                     |
| ------------ | --------------------------------------------------------------------------------------------------------------- |
| `for`        | Quando **você sabe o número de repetições**. Ex: contar de 1 até 10.                                            |
| `while`      | Quando **não sabe quantas vezes vai repetir**, e pode ser **zero vezes**. Ex: esperar o usuário digitar "sair". |
| `do...while` | Quando **precisa rodar ao menos uma vez**, independente da condição. Ex: pedir senha até acertar.               |

## ✅ Exemplo prático: Menu com `do...while`

```c
#include <stdio.h>

int main() {
    int opcao;

    do {
        printf("\n=== MENU ===\n");
        printf("1 - Jogar\n");
        printf("2 - Ver pontuação\n");
        printf("0 - Sair\n");
        printf("Escolha uma opção: ");
        scanf("%d", &opcao);

        if (opcao == 1)
            printf("Iniciando o jogo...\n");
        else if (opcao == 2)
            printf("Pontuação: 1200 pontos.\n");
        else if (opcao != 0)
            printf("Opção inválida!\n");

    } while (opcao != 0);

    printf("Saindo...\n");
    return 0;
}
```
