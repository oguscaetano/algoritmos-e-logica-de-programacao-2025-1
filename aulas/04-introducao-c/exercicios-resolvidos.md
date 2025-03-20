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

## 6 - Verificação de cartão vermelho

```c
#include <stdio.h>

int main() {
    int cartoes = 2; // Simulando que o jogador recebeu 2 amarelos

    if (cartoes == 2) {
        printf("O jogador foi expulso! Recebeu um cartao vermelho.\n");
    } else {
        printf("O jogador continua no jogo.\n");
    }

    return 0;
}
```

## 7 – Verificar se um Jogador Pode Jogar  

```c
#include <stdio.h>

int main() {
    int idade;

    // Entrada de dados
    printf("Digite a idade do jogador: ");
    scanf("%d", &idade);

    // Verificação
    if (idade <= 20) {
        printf("O jogador pode participar da categoria Sub-20.\n");
    } else {
        printf("O jogador deve jogar na categoria profissional.\n");
    }

    return 0;
}
```

## 8 – Avaliar o desempenho do jogador 

```c
#include <stdio.h>

int main() {
    int gols;

    printf("Digite a quantidade de gols marcados pelo jogador: ");
    scanf("%d", &gols);

    if (gols > 10) {
        printf("Excelente temporada!\n");
    } else if (gols >= 5) { // Aqui já sabemos que é no máximo 10
        printf("Boa temporada!\n");
    } else {
        printf("Temporada abaixo do esperado.\n");
    }

    return 0;
}
```

## 9 – Classificação do jogador baseada em idade e desempenho 

```c
#include <stdio.h>

int main() {
    int idade, gols;

    printf("Digite a idade do jogador: ");
    scanf("%d", &idade);

    printf("Digite a quantidade de gols marcados: ");
    scanf("%d", &gols);

    if (idade <= 20 && gols > 10) { 
        printf("Jovem talento promissor!\n");
        } else if (idade <= 20 && gols <= 10){
            printf("Jovem em desenvolvimento.\n");
        } else if (idade > 20 && gols > 15) {
            printf("Jogador experiente em grande fase!\n");
        } else if (idade > 20 && gols <= 15){
            printf("Estevão.\n");
        }

    return 0;
}
```

## 10 – Classificação do nível da partida com base na quantidade de torcedores

```c
#include <stdio.h>

int main() {
    int capacidade, torcedores;
    float ocupacao;

    printf("Digite a capacidade total do estadio: ");
    scanf("%d", &capacidade);

    printf("Digite a quantidade de torcedores presentes: ");
    scanf("%d", &torcedores);

    ocupacao = (float)torcedores / capacidade * 100;

    printf("\n=== RESULTADO ===\n");

    printf("Lotação: %.2f%% \n", ocupacao);

    if (ocupacao > 90) {
        printf("Lotado!\n");
    } else if (ocupacao >= 70) {
        printf("Otima presenca de publico!\n");
    } else if (ocupacao >= 50) {
        printf("Publico razoavel.\n");
    } else {
        printf("Morumbis.\n");
    }

    return 0;
}
```