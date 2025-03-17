### Tipos de Dados em C
| Tipo         | Tamanho (bytes) | Faixa de Valores (Aproximada) | Exemplo de Uso |
|-------------|----------------|---------------------------------|----------------|
| `char`      | 1 byte         | -128 a 127 (`signed char`)<br>0 a 255 (`unsigned char`) | `char letra = 'A';` |
| `int`       | 4 bytes        | -2.147.483.648 a 2.147.483.647 | `int idade = 25;` |
| `float`     | 4 bytes        | ~6 casas decimais de precisão | `float pi = 3.1415;` |
| `double`    | 8 bytes        | ~15 casas decimais de precisão | `double numero = 2.718281828;` |
| `_Bool`     | 1 byte         | 0 (falso) ou 1 (verdadeiro) | `_Bool ligado = 1;` |

### Especificadores

| Especificador | Tipo de Dado | Exemplo de Uso |
|--------------|-------------|----------------|
| `%d` ou `%i` | Inteiro decimal (int) | `printf("%d", 100);` imprime `100` |
| `%f` | Ponto flutuante (float, double) | `printf("%f", 3.14);` imprime `3.140000` |
| `%.2f` | Ponto flutuante com 2 casas decimais | `printf("%.2f", 3.14);` imprime `3.14` |
| `%c` | Caracter único (char) | `printf("%c", 'A');` imprime `A` |
| `%s` | String (char[]) | `printf("%s", "Olá");` imprime `Olá` |
| `%x` | Inteiro em hexadecimal | `printf("%x", 255);` imprime `ff` |
| `%o` | Inteiro em octal | `printf("%o", 8);` imprime `10` |

