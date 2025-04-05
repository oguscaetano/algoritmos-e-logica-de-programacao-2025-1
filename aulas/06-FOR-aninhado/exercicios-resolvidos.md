## 1 - Tabuada 

```c
#include <stdio.h>

int main() {
    int i, j;

    for (i = 1; i <= 10; i++) {
        printf("Tabuada do %d \n", i);
        printf("---------------\n");
        for (j = 1; j <= 10; j++) {
            printf("%d x %d = %d\n", i, j, i * j);
        }
        printf("\n"); // Pula linha entre as tabuadas
    }

    return 0;
}
```

## 2 – Quadrado de Asteriscos  

```c
#include <stdio.h>

int main() {
    int numero, i, j;

    printf("Digite o tamanho do quadrado: ");
    scanf("%d", &numero);

    for (i = 0; i < numero; i++) {
        for (j = 0; j < numero; j++) {
            printf("* ");
        }
        printf("\n"); // Pula linha ao final de cada linha
    }

    return 0;
}
```

## 3 – Triângulo de Números 

```c
#include <stdio.h>

int main() {
    int numero, i, j;

    printf("Digite o numero de linhas do triangulo: ");
    scanf("%d", &numero);

    for (i = 1; i <= numero; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}
```

## 4 - Triângulo invertido de números 

```c
#include <stdio.h>

int main() {
    int numero;

    printf("Tamanho da piramide de hashtags: ");
    scanf("%d", &numero);

    for (int i = numero; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }
    return 0;
}
```

## 5 – Xadrez de Asteriscos  

```c
#include <stdio.h>

int main() {
    int tamanho, i, j;

    printf("Digite o tamanho do tabuleiro: ");
    scanf("%d", &tamanho);

    for (i = 0; i < tamanho; i++) {
        for (j = 0; j < tamanho; j++) {
            if ((i + j) % 2 == 0) {
                printf("# ");
            } else {
                printf("  "); // Dois espaços para manter o alinhamento
            }
        }
        printf("\n");
    }

    return 0;
}
```

## 6 – Pirâmide de Números Pares  

```c
#include <stdio.h>

int main() {
    int linhas, i, j, num = 2; 

    printf("Digite o numero de linhas da piramide: ");
    scanf("%d", &linhas);

    for (i = 1; i <= linhas; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d ", num);
            num += 2; // Incrementa para o próximo número par
        }
        printf("\n");
    }

    return 0;
}
```

## 7 - Controle de Estoque no Supermercado 

```c
#include <stdio.h>

int main() {
    int totalProdutos;

    printf("Digite a quantidade de produtos a serem cadastrados: ");
    scanf("%d", &totalProdutos);

    for (int i = 1; i <= totalProdutos; i++) {
        char nome[50];  // Nome do produto
        int estoque, minimo;  // Quantidade em estoque e estoque mínimo

        printf("\nProduto %d:\n", i);
        printf("Nome do produto: ");
        scanf("%s", nome);  // Captura o nome do produto

        printf("Quantidade em estoque: ");
        scanf("%d", &estoque);

        printf("Estoque mínimo recomendado: ");
        scanf("%d", &minimo);

        // Verifica se o produto precisa de reposição
        if (estoque < minimo) {
            printf("-> O produto '%s' precisa ser reposto! (Estoque: %d, Mínimo: %d)\n", nome, estoque, minimo);
        } else {
            printf("-> O produto '%s' tem estoque suficiente. (Estoque: %d, Mínimo: %d)\n", nome, estoque, minimo);
        }
    }

    return 0;
}
```

## 8 - Controle de Revisão de Carros  

```c
#include <stdio.h>

int main() {
    int quantidadeCarros;

    printf("Digite a quantidade de carros a serem registrados: ");
    scanf("%d", &quantidadeCarros);

    for (int i = 0; i < quantidadeCarros; i++) {
        char modelo[50];
        int ano;
        int carro_funcionando;

        printf("\nCarro %d:\n", i + 1);
        printf("Modelo do carro: ");
        scanf("%s", modelo);

        printf("Ano de fabricação: ");
        scanf("%d", &ano);

        printf("O carro está funcionando normalmente? (1 ou 0): ");
        scanf("%d", &carro_funcionando);

        // Verificação das condições do carro
        if (ano < 2005 && carro_funcionando == 0) {
            printf("O carro %s precisa de REPAROS URGENTES!\n", modelo);
        } else if (ano < 2005) {
            printf("O carro %s é antigo, recomenda-se uma revisão!\n", modelo);
        } else if (carro_funcionando == 0) {
            printf("O carro %s precisa de manutenção!\n", modelo);
        } else {
            printf("O carro %s está em boas condições!\n", modelo);
        }
    }

    return 0;
}
```

## 9 - Catálogo de Séries da Netflix 

```c
#include <stdio.h>

int main() {
    int num_series; 
    printf("Quantas series deseja cadastrar? ");
    scanf("%d", &num_series);

    for (int i = 0; i < num_series; i++) {
        char nome[50]; // Nome da série
        int num_avaliacoes;
        float soma_notas = 0, media;

        printf("\nDigite o nome da serie %d: ", i + 1);
        scanf(" %[^\n]", nome); // Lê o nome com espaços

        printf("Quantas avaliacoes essa serie recebeu? ");
        scanf("%d", &num_avaliacoes);

        for (int j = 0; j < num_avaliacoes; j++) {
            float nota;
            printf("Digite a nota %d (0 a 10): ", j + 1);
            scanf("%f", &nota);

            if (nota < 0 || nota > 10) {
                printf("Nota invalida! Digite um valor entre 0 e 10.\n");
                j--; // Para repetir a entrada da nota inválida
            } else {
                soma_notas += nota;
            }
        }

        media = soma_notas / num_avaliacoes;

        printf("\n--- Detalhes da Serie ---\n");
        printf("Nome: %s\n", nome);
        printf("Media das notas: %.2f\n", media);

        if (media >= 8.0) {
            printf("Classificacao: Super Recomendada 🔥\n");
        } else if (media >= 5.0) {
            printf("Classificacao: Boa 👍\n");
        } else {
            printf("Classificacao: Ruim 👎\n");
        }
        printf("--------------------------\n");
    }

    return 0;
}
```

## 10 - Triângulo de asteriscos
```c
#include <stdio.h>

int main() {
    int altura, i, j;

    printf("Digite a altura do triangulo: ");
    scanf("%d", &altura);

    for (i = 1; i <= altura; i++) {
        for (j = 1; j <= altura - i; j++) {
            printf(" ");
        }
        for (j = 1; j <= 2 * i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```