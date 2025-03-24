# EXERCÍCIOS

## 1 – Contagem Simples  
```c
#include <stdio.h>

int main() {
    for (int index = 1; index <= 10; index++) {
        printf("%d\n", index);
    }
    return 0;
}
```

## 2 – Treino de Velocidade do Flash 🏃‍♂️

```c
#include <stdio.h>

int main() {
    int kilometros;
    
    printf("Quantos Km o Flash correu? ");
    scanf("%d", &kilometros);

    for (int index = 1; index <= kilometros; index++) {
        printf("O Flash correu %d km!\n", index);
    }
    
    printf("O Flash terminou seu treino!");

    return 0;
}
```

## 3 – Soma dos Números de `1 a n` 
```c
#include <stdio.h>

int main() {
    int n, soma = 0;

    printf("Digite um numero: ");
    scanf("%d", &n);

    for (int index = 1; index <= n; index++) {
        soma += index;
    }

    printf("A soma de 1 ate %d e: %d\n", n, soma);

    return 0;
}
```

## 4 – Sequência de Missões do Batman 🦇

```c
#include <stdio.h>

int main() {
    int numero;
    
    printf("Quantas missoes o batman vai fazer esse noite? ");
    scanf("%d", &numero);

    for (int index = 1; index <= numero; index++) {
        printf("Missão %d concluída! \n", index);
    }
    
    printf("Pode ir dormir, Batman. Seu trabalho ja foi concluido.");

    return 0;
}
```

## 5 – Tabuada

```c
#include <stdio.h>

int main() {
    int numero;
    
    printf("Qual número você quer saber a tabuada? ");
    scanf("%d", &numero);

    for (int index = 0; index <= 10; index++) {
        int multi;
        multi = index * numero;
        printf("%d x %d = %d\n", numero, index, multi);
    }

    return 0;
}
```

## 6 – Números Pares de `1 a n`
```c
#include <stdio.h>

int main() {
    int numero;

    printf("Digite um numero: ");
    scanf("%d", &numero);

    printf("Numeros pares de 1 ate %d:\n", n);

    for (int index = 1; index <= numero; index++) {
        if (index % 2 == 0) {
            printf("%d ", index);
        }
    }

    return 0;
}
```

## 7 – Contando Múltiplos de 3 e 5
```c
#include <stdio.h>

int main() {
    int numero, contador = 0;

    printf("Digite um numero: ");
    scanf("%d", &numero);

    for (int index = 1; index <= numero; index++) {
        if (index % 3 == 0 && index % 5 == 0) {
            printf("Numero: %d \n", index);
            contador++;
        }
    }

    if (contador == 1) {
        printf("Entre 1 e %d, existe %d numero multiplo de 3 e 5.\n", numero, contador);
    } else {
        printf("Entre 1 e %d, existem %d numeros multiplos de 3 e 5.\n", numero, contador);
    }

    return 0;
}
```

## 8 – Classificação de Idades
```c
#include <stdio.h>

int main() {
    int numero, idade;

    printf("Quantas pessoas voce quer classificar? ");
    scanf("%d", &numero);

    for (int index = 1; index <= numero; index++) {
        printf("Digite a idade %d: ", index);
        scanf("%d", &idade);

        if (idade < 12) {
            printf("Classificacao: Crianca\n");
        } else if (idade >= 12 && idade < 18) {
            printf("Classificacao: Adolescente\n");
        } else if (idade >= 18 && idade < 60) {
            printf("Classificacao: Adulto\n");
        } else {
            printf("Classificacao: Idoso\n");
        }
    }

    return 0;
}
```