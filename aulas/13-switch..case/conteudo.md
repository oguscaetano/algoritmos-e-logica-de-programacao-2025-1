# 🧠 **`switch case` em C**

> *"Você já escreveu um monte de `if else` seguidos para tomar uma decisão com base em uma variável? E se existisse uma forma mais organizada e clara para isso? Pois bem, é aí que entra o `switch case`!"*

📌 Exemplo:

```c
if (opcao == 1) {
    printf("Novo jogo\n");
} else if (opcao == 2) {
    printf("Carregar jogo\n");
} else if (opcao == 3) {
    printf("Sair\n");
}
```

➡️ Pode ser substituído por um `switch case`.

## 🧠 **Estrutura do `switch case`**

```c
switch (variavel) {
    case valor1:
        // instruções
        break;
    case valor2:
        // instruções
        break;
    ...
    default:
        // instruções padrão
}
```

📌 **Explicação passo a passo:**

* `switch`: palavra-chave que abre a estrutura.
* `case`: cada caso testado contra o valor da variável.
* `break`: usado para sair do `switch` após encontrar o caso correspondente.
* `default`: o que acontece se nenhum `case` for igual ao valor da variável.

---

### 🎮 **Exemplo: Menu de Video Game**

```c
#include <stdio.h>

int main() {
    int opcao;
    printf("Menu:\n1 - Jogar\n2 - Carregar\n3 - Sair\nEscolha: ");
    scanf("%d", &opcao);

    switch (opcao) {
        case 1:
            printf("Iniciando novo jogo...\n");
            break;
        case 2:
            printf("Carregando jogo salvo...\n");
            break;
        case 3:
            printf("Saindo do jogo. Ate logo!\n");
            break;
        default:
            printf("Opcao invalida.\n");
    }

    return 0;
}
```

---

### 🛠️ **Exemplos**

**Exemplo 1 – Dia da semana**

```c
int dia;
printf("Digite um número de 1 a 7: ");
scanf("%d", &dia);

switch (dia) {
    case 1: printf("Domingo\n"); break;
    case 2: printf("Segunda-feira\n"); break;
    case 3: printf("Terça-feira\n"); break;
    case 4: printf("Quarta-feira\n"); break;
    case 5: printf("Quinta-feira\n"); break;
    case 6: printf("Sexta-feira\n"); break;
    case 7: printf("Sábado\n"); break;
    default: printf("Número inválido!\n");
}
```

**Exemplo 2 – Calculadora simples**

```c
char operador;
float a, b;

printf("Digite a operacao (+, -, *, /): ");
scanf(" %c", &operador);
printf("Digite dois numeros: ");
scanf("%f %f", &a, &b);

switch (operador) {
    case '+': printf("Resultado: %.2f\n", a + b); break;
    case '-': printf("Resultado: %.2f\n", a - b); break;
    case '*': printf("Resultado: %.2f\n", a * b); break;
    case '/': 
        if (b != 0)
            printf("Resultado: %.2f\n", a / b); 
        else 
            printf("Erro: divisao por zero!\n");
        break;
    default: printf("Operador invalido!\n");
}
```

---

## 🤔 **Diferenças entre `if/else` e `switch case`**

| Situação                                                                | Melhor usar |
| ----------------------------------------------------------------------- | ----------- |
| Comparações com operadores lógicos (`>`, `<`, `==`, `!=`)               | `if/else`   |
| Comparação de uma variável com vários valores fixos (ex: `1`, `2`, `3`) | `switch case`    |
