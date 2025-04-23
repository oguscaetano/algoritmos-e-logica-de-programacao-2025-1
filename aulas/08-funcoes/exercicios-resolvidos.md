# EXERCÍCIOS

## 1. Verificar se um número é par ou ímpar

```c
#include <stdio.h>

int parImpar(int numero) {
    if (numero % 2 == 0)
        return 1;
    else
        return 0;
}

int main() {
    int num;
    printf("Digite um numero: ");
    scanf("%d", &num);

    if (parImpar(num))
        printf("O numero e par.\n");
    else
        printf("O numero e impar.\n");

    return 0;
}
```

## 2. Calcular a média de dois números

```c
#include <stdio.h>

float media(float a, float b) {
    return (a + b) / 2;
}

int main() {
    float n1, n2;
    printf("Digite duas notas: \n");
    scanf("%f %f", &n1, &n2);

    printf("Media: %.2f\n", media(n1, n2));
    return 0;
}
```

## 3. Contar vogais em uma palavra

```c
#include <stdio.h>

int contarVogais(char palavra[]) {
    int contador = 0;
    for (int i = 0; palavra[i] != '\0'; i++) {
        if (palavra[i] == 'a' || palavra[i] == 'e' || palavra[i] == 'i' || palavra[i] == 'o' || palavra[i] == 'u')
            contador++;
    }
    return contador;
}

int main() {
    char texto[100];
    printf("Digite uma palavra: ");
    scanf("%s", texto);

    printf("Quantidade de vogais: %d\n", contarVogais(texto));
    return 0;
}
```

## 4. Encontrar o maior de três números

```c
#include <stdio.h>

int maior(int a, int b, int c) {
    if (a >= b && a >= c)
        return a;
    else if (b >= a && b >= c)
        return b;
    else
        return c;
}

int main() {
    int x, y, z;
    printf("Digite tres numeros: \n");
    scanf("%d %d %d", &x, &y, &z);

    printf("Maior numero: %d\n", maior(x, y, z));
    return 0;
}
```

## 5. Calcular a média de um array de inteiros

```c
#include <stdio.h>

float mediaArray(int vetor[], int tamanho) {
    int soma = 0;
    for (int i = 0; i < tamanho; i++)
        soma += vetor[i];
    return (float)soma / tamanho;
}

int main() {
    int numeros[5] = {10, 20, 30, 40, 50};
    printf("Media: %.2f\n", mediaArray(numeros, 5));
    return 0;
}
```

## 6. Imprimir uma tabela de multiplicação (tabuada)

```c
#include <stdio.h>

void tabuada(int n) {
    for (int i = 0; i <= 10; i++) {
        printf("%d x %d = %d\n", n, i, n * i);
    }
}

int main() {
    int num;
    printf("Digite um numero: ");
    scanf("%d", &num);

    tabuada(num);
    return 0;
}
```

## 7. Classificar notas de alunos

```c
#include <stdio.h>

void classificar(float nota) {
    if (nota >= 6)
        printf("Aprovado\n");
    else if (nota >= 4)
        printf("Recuperacao\n");
    else
        printf("Reprovado\n");
}

int main() {
    float nota;
    printf("Digite a nota do aluno: ");
    scanf("%f", &nota);

    classificar(nota);
    return 0;
}
```

## 8. Somar elementos pares de um vetor

```c
#include <stdio.h>

int somarPares(int vetor[], int tamanho) {
    int soma = 0;
    for (int i = 0; i < tamanho; i++) {
        if (vetor[i] % 2 == 0)
            soma += vetor[i];
    }
    return soma;
}

int main() {
    int vetor[6] = {1, 2, 3, 4, 5, 6};
    printf("Soma dos pares: %d\n", somarPares(vetor, 6));
    return 0;
}
```

## 9. Criar um padrão de asteriscos com for aninhado

```c
#include <stdio.h>

void quadrado(int n, char c) {
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++)
            printf("%c ", c);
        printf("\n");
    }
}

int main() {
    int lado;
    char caracter;
    printf("Digite o tamanho do lado do quadrado: ");
    scanf("%d", &lado);
    printf("Digite qual caracter quer usar: ");
    scanf(" %c", &caracter);

    quadrado(lado, caracter);
    return 0;
}
```

## 10. Avaliação de desempenho

```c
#include <stdio.h>

float calcularMedia(float n1, float n2, float n3) {
    return (n1 + n2 + n3) / 3;
}

void classificar(float media) {
    if (media >= 9)
        printf("Excelente\n");
    else if (media >= 7)
        printf("Bom\n");
    else if (media >= 5)
        printf("Regular\n");
    else
        printf("Ruim\n");
}

int main() {
    float n1, n2, n3, media;
    for (int i = 1; i <= 5; i++) {
        printf("Jogador %d:\n", i);
        printf("Digite as 3 notas: \n");
        scanf("%f %f %f", &n1, &n2, &n3);
        media = calcularMedia(n1, n2, n3);
        printf("Media: %.2f - ", media);
        classificar(media);
        printf("\n============== \n\n");
    }

    return 0;
}
```