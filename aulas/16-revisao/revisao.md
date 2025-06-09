# **Aula de Revisão – Algoritmos e Lógica de Programação em C**

## **1 - Declaração de Variáveis**

- `int`: guarda números inteiros, como a **quantidade de alunos**.
- `float`: números com vírgula, como a **média final de um aluno**.
- `char`: um único caractere, como a **letra inicial de um nome**.

**Exemplo em código:**

```c
int idade = 20;
float media = 8.5;
char letra = 'A';

printf("Idade: %d\n", idade);
printf("Média: %.2f\n", media);
printf("Letra: %c\n", letra);
```

## **2 - Laços de Repetição (for, while, do while)**

### ✅ **`for` – Quando você já sabe quantas vezes repetir**

**Exemplo:**

```c
for (int i = 0; i < 5; i++) {
    printf("Aluno %d\n", i + 1);
}
```

### ✅ **`while` – Repete enquanto a condição for verdadeira**

```c
int i = 1;

while (i <= 5) {
    printf("While: %d\n", i);
    i++;
}
```

### ✅ **`do while` – Garante pelo menos uma execução**

```c
int j = 1;

do {
    printf("Do While: %d\n", j);
    j++;
} while (j <= 5);
```

## **3 - Arrays (Vetores) e Matrizes**

### ✅ **Array (vetor)**

```c
int notas[5] = {7, 8, 6, 9, 10};

for (int i = 0; i < 5; i++) {
    printf("Nota %d: %d\n", i, notas[i]);
}
```

> Analogia: array = **gaveta com vários compartimentos numerados**.

### ✅ **Array Multidimensional (Matriz)**

```c
int matriz[2][3] = {
    {1, 2, 3},
    {4, 5, 6}
};

for (int i = 0; i < 2; i++) {
    for (int j = 0; j < 3; j++) {
        printf("%d ", matriz[i][j]);
    }
    printf("\n");
}
```

## **4 - Loops Aninhados**

```c
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 2; j++) {
        printf("Sala %d, Aluno %d\n", i + 1, j + 1);
    }
}
```

## **5 - Condicionais (`if/else` e `switch`)**

### ✅ **`if/else`**

```c
int nota = 7;

if (nota >= 6) {
    printf("Aprovado\n");
} else {
    printf("Reprovado\n");
}
```

### ✅ **`switch case`**

```c
int opcao = 2;

switch (opcao) {
    case 1: printf("Início\n"); break;
    case 2: printf("Meio\n"); break;
    case 3: printf("Fim\n"); break;
    default: printf("Opção inválida\n");
}
```

> Analogia: `switch` é como **um menu de lanchonete**.

## **6 - Funções com Passagem de Parâmetros**

```c
void ola(char nome[]) {
    printf("Olá, %s!\n", nome);
}

int soma(int a, int b) {
    return a + b;
}

int main() {
    ola("João");

    int resultado = soma(3, 5);

    printf("Resultado: %d\n", resultado);
}
```

> Dica: função = **uma tarefa separada** que pode ser chamada várias vezes.
