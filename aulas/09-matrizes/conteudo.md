# **Matrizes em C**

## 📌 1. Introdução – Relembrando Vetores

> No conteúdo anterior vimos vetores: uma sequência de valores do mesmo tipo, acessados por um único índice.

```c
int notas[5] = {7, 8, 6, 9, 10};  // Um vetor com 5 notas
```

- Vetores são como uma **fila de caixas** com 1 linha só.

## 📌 2. O que é uma Matriz?

Uma matriz é como uma **tabela ou planilha do Excel**.

|        | Coluna 0 | Coluna 1 | Coluna 2 |
|--------|----------|----------|----------|
| Linha 0|   [0][0] |  [0][1]  |  [0][2]  |
| Linha 1|   [1][0] |  [1][1]  |  [1][2]  |
| Linha 2|   [2][0] |  [2][1]  |  [2][2]  |

> Cada elemento está em uma posição específica, identificada por **duas coordenadas**: linha e coluna.

### 📌 Sintaxe:

```c
int matriz[3][3];  // 3 linhas e 3 colunas
```

## 📌 3. Exemplo do dia a dia: Notas de alunos

**Contexto**: 3 alunos fizeram 2 provas. Queremos armazenar e mostrar as notas.

```c
#include <stdio.h>

int main() {
    int notas[3][2] = {
        {7, 8},
        {6, 9},
        {10, 7}
    };

    printf("Nota do aluno 1, prova 1: %d\n", notas[0][0]); // 7
    printf("Nota do aluno 2, prova 2: %d\n", notas[1][1]); // 9
    return 0;
}
```

> Usamos dois índices: `notas[aluno][prova]`

## 📌 4. Preenchendo a matriz com `for`

```c
#include <stdio.h>

int main() {
    int notas[3][2];

    // Entrada de dados
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 2; j++) {
            printf("Digite a nota do aluno %d, prova %d: ", i + 1, j + 1);
            scanf("%d", &notas[i][j]);
        }
    }

    // Saída de dados
    printf("\nNotas:\n");
    for (int i = 0; i < 3; i++) {
        printf("Aluno %d: ", i + 1);
        for (int j = 0; j < 2; j++) {
            printf("%d ", notas[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

## 📌 5. Exemplo: Temperatura em uma cidade

**Contexto**: Medir a temperatura em 7 dias, 4 horários diferentes por dia.

```c
float temperatura[7][4];  // 7 dias, 4 horários

// Cada linha é um dia, cada coluna é um horário
```

- Matrizem podem nos ajudar a organizar informações mais complexas.

## 📌 6. Dicas Importantes

- A indexação começa em `0`.
- Matrizes em C **têm tamanho fixo**.
- Para manipular dados de maneira organizada, **loop for aninhado** é essencial.
- Cada tipo de dado ocupa espaço na memória proporcional ao seu tipo.