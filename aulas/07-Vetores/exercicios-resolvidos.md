# EXERCÍCIOS

## 1 - Contagem de Pontos de Fase  
```c
#include <stdio.h>

int main() {
    int pontos[5];
    
    printf("Digite as pontuacoes das 5 fases:\n");
    for (int i = 0; i < 5; i++) {
        printf("Fase %d: ", i + 1);
        scanf("%d", &pontos[i]);
    }

    printf("\nPontuacoes do jogador:\n");
    for (int i = 0; i < 5; i++) {
        printf("Fase %d: %d pontos\n", i + 1, pontos[i]);
    }

    return 0;
}
```

## 2 - Média de FPS de um Jogo
```c
#include <stdio.h>

int main() {
    float fps[6], soma = 0, media;
    
    printf("Digite os FPS registrados em 6 momentos:\n");
    for (int i = 0; i < 6; i++) {
        printf("Momento %d: ", i + 1);
        scanf("%f", &fps[i]);
        soma += fps[i]; 
    }

    media = soma / 6;

    printf("\nMedia de FPS: %.2f\n", media);

    return 0;
}
```

## 3 - Encontrando o Maior Dano Causado
```c
#include <stdio.h>

int main() {
    int dano[4], maior;

    printf("Digite o dano de 4 ataques:\n");
    for (int i = 0; i < 4; i++) {
        printf("Ataque %d: ", i + 1);
        scanf("%d", &dano[i]);
    }

    maior = dano[0];
    for (int i = 1; i < 4; i++) {
        if (dano[i] > maior) {
            maior = dano[i];
        }
    }

    printf("\nMaior dano causado: %d\n", maior);

    return 0;
}
```

## 4 - Comparando Score com Recorde
```c
#include <stdio.h>

int main() {
    int scores[5], recorde = 5000;

    printf("Digite os 5 scores do jogador:\n");
    for (int i = 0; i < 5; i++) {
        printf("Score %d: ", i + 1);
        scanf("%d", &scores[i]);

        if (scores[i] > recorde) {
            printf("Parabens! Score %d superou o recorde!\n", scores[i]);
            recorde = scores[i];
        }
    }

    return 0;
}
```

## 5 - Ranking de Score (Ordenação)
```c
#include <stdio.h>

int main() {
    int jogadores[5], temp;

    printf("Digite os scores de 5 jogadores:\n");
    for (int i = 0; i < 5; i++) {
        printf("Jogador %d: ", i + 1);
        scanf("%d", &jogadores[i]);
    }

    // Bubble Sort
    for (int i = 0; i < 5; i++) {
        for (int j = 0; j < 5 - i; j++) {
            if (jogadores[j] < jogadores[j + 1]) {
                temp = jogadores[j];
                jogadores[j] = jogadores[j + 1];
                jogadores[j + 1] = temp;
            }
        }
    }

    printf("\nRanking de Scores:\n");
    for (int i = 0; i < 5; i++) {
        printf("%do lugar: %d pontos\n", i + 1, jogadores[i]);
    }

    return 0;
}
```