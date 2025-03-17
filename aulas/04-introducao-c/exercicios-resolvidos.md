# EXERCÍCIOS

## 1 - Apresentação do Jogador 

```c
#include <stdio.h>

int main() {
    char nome[50];
    int idade, gols;

    printf("Digite o nome do jogador: ");
    scanf("%s", &nome);

    printf("Digite a idade do jogador: ");
    scanf("%d", &idade);

    printf("Digite a quantidade de gols do jogador: ");
    scanf("%d", &gols);

    printf("\n--- Informacoes do Jogador ---\n");
    printf("Nome: %s\n", nome);
    printf("Idade: %d anos\n", idade);
    printf("Gols marcados: %d\n", gols);

    return 0;
}
```

## 2 - Média de Gols por Partida  

```c
#include <stdio.h>

int main() {
    int gols, partidas;
    float media;

    printf("Digite o numero total de gols: ");
    scanf("%d", &gols);

    printf("Digite o numero de partidas jogadas: ");
    scanf("%d", &partidas);

    media = (float)gols / partidas;

    printf("Media de gols por partida: %.2f\n", media);

    return 0;
}
```

## 3 - Conversão de Minutos para Tempo de Jogo 

```c
#include <stdio.h>

int main() {
    int minutos, horas, min_restantes;

    printf("Digite o tempo jogado em minutos: ");
    scanf("%d", &minutos);

    horas = minutos / 60;
    min_restantes = minutos % 60;

    printf("Tempo de jogo: %d horas e %d minutos\n", horas, min_restantes);

    return 0;
}
```

## 4 - Calculando o Aproveitamento de um Time

```c
#include <stdio.h>

int main() {
    int vitorias, empates, derrotas, pontos;

    printf("Digite o numero de vitorias: ");
    scanf("%d", &vitorias);

    printf("Digite o numero de empates: ");
    scanf("%d", &empates);

    printf("Digite o numero de derrotas: ");
    scanf("%d", &derrotas);

    pontos = (vitorias * 3) + (empates * 1);

    printf("O time tem %d pontos na tabela.\n", pontos);

    return 0;
}
```

## 5 - Diferença de Salários entre Jogadores 

```c
#include <stdio.h>

int main() {
    float salario1, salario2, diferenca;

    printf("Digite o salario do primeiro jogador: ");
    scanf("%f", &salario1);

    printf("Digite o salario do segundo jogador: ");
    scanf("%f", &salario2);

    diferenca = salario1 - salario2;

    printf("A diferenca de salario entre os jogadores e: R$ %.2f\n", diferenca);

    return 0;
}
```

Se você quiser saber o valor absoluto da diferença, poderá adicionar as seguintes linhas:

```c
#include <math.h> // Biblioteca para usar fabs()

diferenca = fabs(salario1 - salario2);
```

**`fabs`** vem de **"floating-point absolute value"**, que significa **"valor absoluto de ponto flutuante"**.  

📌 **Quebrando o nome:**  
- **`f`** → Refere-se a **números de ponto flutuante** (`float` ou `double`).  
- **`abs`** → Vem de **"absolute"**, ou seja, **valor absoluto** (sem sinal negativo).  

💡 **Comparação com `abs()`**  
No C, existe também a função **`abs(x)`**, que faz a **mesma coisa, mas para números inteiros (`int`)**.  

🔹 `fabs(x)` → Para **`float` e `double`** (números decimais).  
🔹 `abs(x)` → Para **`int`** (números inteiros).  
