# Introdução a Linguagem C

## O que é a Linguagem C?
- Criada por **Dennis Ritchie** em **1972**.  
- Base para várias outras linguagens (C++, Java, Python).  
- **Linguagem de alto desempenho** e utilizada em sistemas operacionais, jogos e embarcados.  

> **Diferença principal entre C e Portugol:**  
>- **Portugol** → Linguagem educacional para aprendizado.  
>- **C** → Linguagem real usada em sistemas complexos.  

## Configuração do Ambiente
### `1 - Instalar o compilador`
O C não é interpretado como o Portugol. Ele precisa ser compilado. Vamos usar o **MinGW (GCC)**.  
O **GCC (GNU Compiler Collection)** é o compilador necessário para rodar programas em **C e C++**. Vamos instalar o **MinGW-w64**, que inclui o GCC, e configurar tudo corretamente no Windows.

>Siga todas as orientações deste site: [🔗 Usando GCC com MinGW](https://code.visualstudio.com/docs/cpp/config-mingw)  

### `2 - Instalar e configurar o VS Code (Visual Studio Code)`
Agora que temos o GCC instalado, vamos configurar o VS Code:

1. Baixe e instale o [VS Code](https://code.visualstudio.com/)
2. Abra o VS Code e vá até Extensões (Ctrl + Shift + X).
3. Pesquise por C/C++ e instale a extensão oficial da Microsoft.
4. Instale a extensão C/C++ Extension Pack da Microsoft.

## Escrevendo e Rodando um Programa em C
Agora, vamos testar se tudo está funcionando:

1. **Crie um novo arquivo no VS Code** e salve-o como `teste.c`.  
2. Escreva o seguinte código:

   ```c
   #include <stdio.h>

   int main() {
       printf("Ola, Mundo!\n");
       return 0;
   }
   ```

📌 **Explicação:**  
- `#include <stdio.h>` → Biblioteca para entrada e saída.  
- `int main()` → Função principal do programa.  
- `printf("Ola, Mundo!\n");` → Imprime texto na tela.  
- `return 0;` → Indica que o programa finalizou corretamente.  

3. **Compilar e executar** 

Aperte o botão de play ▶️ no canto superior direito do VS Code 

Se tudo estiver certo, aparecerá no terminal:  

```
Ola, Mundo!
```

## Comparação entre Portugol e C

| Conceito | Portugol | C |
|----------|---------|----|
| **Declaração de Variáveis** | `variavel: inteiro` | `int variavel;` |
| **Entrada de Dados** | `leia(variavel)` | `scanf("%d", &variavel);` |
| **Saída de Dados** | `escreva(variavel)` | `printf("%d", variavel);` |
| **Operadores Matemáticos** | `+`, `-`, `*`, `/` | `+`, `-`, `*`, `/` |
| **Operadores Relacionais** | `=`, `<>`, `<`, `>`, `<=`, `>=` | `==`, `!=`, `<`, `>`, `<=`, `>=` |
| **Operadores Lógicos** | `e`, `ou`, `nao` | `&&`, `\|\|`, `!` |

Aqui está uma **tabela completa** com os **principais tipos de dados** em C, incluindo suas descrições, tamanhos típicos (em sistemas de 32 e 64 bits) e exemplos de uso. 🚀  

### Tipos de Dados em C
| Tipo         | Tamanho (bytes) | Faixa de Valores (Aproximada) | Exemplo de Uso |
|-------------|----------------|---------------------------------|----------------|
| `char`      | 1 byte         | -128 a 127 (`signed char`)<br>0 a 255 (`unsigned char`) | `char letra = 'A';` |
| `int`       | 4 bytes        | -2.147.483.648 a 2.147.483.647 | `int idade = 25;` |
| `float`     | 4 bytes        | ~6 casas decimais de precisão | `float pi = 3.1415;` |
| `double`    | 8 bytes        | ~15 casas decimais de precisão | `double numero = 2.718281828;` |
| `_Bool`     | 1 byte         | 0 (falso) ou 1 (verdadeiro) | `_Bool ligado = 1;` |

### Entrada e Saída de Dados
📌 **Em Portugol (VisualG)**

```sh
Algoritmo "Entrada e saída de dados"

Var
   numero: inteiro

Inicio

   escreva("Digite um número: ")
   leia(numero)
   escreval("O número digitado foi: ", numero)

Fimalgoritmo
```

📌 **Em C**
```c
#include <stdio.h>

int main() {
    int numero;
    printf("Digite um numero: ");
    scanf("%d", &numero);
    printf("O numero digitado foi: %d\n", numero);
    return 0;
}
```

📌 **Explicação:**  
- Em **C**, usamos `scanf()` para ler valores, com `%d` indicando que é um número inteiro.  
- O `&` antes da variável indica que estamos passando o endereço dela para `scanf()`.  

### Operadores Matemáticos
📌 **Em Portugol (VisualG)**

```sh
soma <- 5 + 3
produto <- 5 * 3
```

📌 **C**

```c
int soma = 5 + 3;
int produto = 5 * 3;
```

### Operadores Relacionais e Lógicos
📌 **Em Portugol (VisualG)**
```sh
Algoritmo "Menor ou maior de idade"

Var
   idade: inteiro

Inicio

   escreva("Digite sua idade: ")
   leia(idade)

   se (idade >= 18) entao
      escreval("Maior de idade")
   senao
      escreval("Menor de idade")
   fimse

Fimalgoritmo
```

📌 **C**
```c
#include <stdio.h>

int main() {
    int idade;
    printf("Digite sua idade: ");
    scanf("%d", &idade);

    if (idade >= 18) {
        printf("Maior de idade\n");
    } else {
        printf("Menor de idade\n");
    }

    return 0;
}
```

📌 **Explicação:**  
- `se ... entao` vira `if () {}` em **C**.  
- `senao` vira `else {}`.  

## Conclusão
- **C é mais detalhado** que Portugol, exigindo **tipos de dados, uso de `scanf` e `printf`**.  
- **Os operadores são similares** em ambas as linguagens.  
- **O aprendizado em Portugol facilita a transição para C**, pois a lógica é a mesma.  
