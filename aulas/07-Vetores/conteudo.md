# Introdução ao Conceito de Vetores 
Imagine que um professor tem **5 alunos** e deseja armazenar suas notas. Sem vetores, precisaríamos de **5 variáveis separadas**:  
```c
int nota1, nota2, nota3, nota4, nota5;
```
Isso funcionaria, mas **e se forem 100 alunos?** Criar 100 variáveis seria muito ruim de gerenciar. Aí é que entram os vetores!

## O que é um vetor?
Um **vetor (array)** é uma estrutura de dados que permite armazenar **múltiplos valores do mesmo tipo** em uma única variável, organizados **em posições numeradas (índices).**  

**Exemplo de um vetor de 5 posições:**  

| Índice  | 0  | 1  | 2  | 3  | 4  |
|---------|----|----|----|----|----|
| Valor   | 8  | 6  | 7  | 9  | 10 |

## Declarando e Usando Vetores 

### Como declarar um vetor em C? 
```c
int notas[5]; // Vetor para armazenar 5 notas
```
- `int` → Tipo dos valores (números inteiros).  
- `notas` → Nome do vetor.  
- `[5]` → Número total de elementos que cabem no vetor.  

💡 **Exemplo prático: Supermercado**  
Um carrinho de compras pode ter vários produtos, cada um com um preço. Podemos armazenar **os preços em um vetor**:  
```c
float precos[3] = {10.50, 5.99, 20.30};
```
Aqui, `precos[0] = 10.50`, `precos[1] = 5.99`, etc.

## Acessando e Modificando Elementos do Vetor

📌 **Cada posição do vetor pode ser acessada pelo índice:**  
```c
notas[0] = 8;   // Armazena o valor 8 na posição 0
notas[1] = 6;   // Armazena 6 na posição 1
printf("Primeira nota: %d\n", notas[0]); // Exibe a primeira nota
```

🔹 **Importante!** Em C, os **índices começam do 0!**  
- O **primeiro elemento** está em `vetor[0]`.  
- O **último elemento** está em `vetor[tamanho - 1]`.  

💡 **Exemplo: Liga da Justiça**  
Imagine que um vetor armazena os **nomes dos super-heróis** que vão lutar contra um vilão:  
```c
char herois[3][20] = {"Superman", "Batman", "Mulher-Maravilha"};
printf("Heroi escolhido: %s\n", herois[1]); // Batman
```

## Usando Laços de Repetição com Vetores

💡 **Exemplo: Notas de alunos**  
Em vez de inserir valores um por um, usamos um **loop `for`** para preencher e exibir um vetor:  
```c
int notas[5];

for (int i = 0; i < 5; i++) {
    printf("Digite a nota do aluno %d: ", i + 1);
    scanf("%d", &notas[i]);
}

printf("\nNotas digitadas:\n");

for (int i = 0; i < 5; i++) {
    printf("Aluno %d: %d\n", i + 1, notas[i]);
}
```
📌 **Explicação:**  
1. O **primeiro `for`** preenche o vetor.  
2. O **segundo `for`** exibe os valores armazenados.  

💡 **Exemplo: Pontuação de um Jogo**  
Imagine um jogo onde **5 jogadores** ganham pontos. Podemos armazenar os pontos e calcular a **média de pontuação**:  
```c
int pontos[5], soma = 0;

for (int i = 0; i < 5; i++) {
    printf("Digite os pontos do jogador %d: ", i + 1);
    scanf("%d", &pontos[i]);
    soma += pontos[i]; // Soma os pontos
}

printf("Média de pontos: %d\n", soma / 5);
```

💡 **[DESAFIO] Exemplo: Mega-sena**  

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
	int megasena[6];
	int fezinha[6] = {3, 12, 23, 55, 10, 42};
	int contador = 0;
	
	srand(time(NULL));
	
	printf("=== Numeros da Megasena! ===\n");
	for (int i = 0; i < 6; i++) {
		megasena[i] = rand() % 60 + 1;
		printf("%d ", megasena[i]);
	}
	
	printf("\n\n=== Fezinha ===\n");
	for (int i = 0; i < 6; i++) {
		printf("%d ", fezinha[i]);
	}
	
	printf("\n\nNumeros iguais: ");
	for (int i = 0; i < 6; i++){
		for (int j = 0; j < 6; j++){
			if (megasena[i] == fezinha[j]) {
				printf("%d ", fezinha[j]);
				contador++;
			}
		}
	}
	
	if (contador == 0) {
		printf("0");
	}
	
	printf("\nAcertos: %d", contador);
    return 0;
}
```

## 🎯 Conclusão
✅ Vetores **armazenam múltiplos valores** em uma única variável.  
✅ Cada valor é acessado por um **índice numérico**.  
✅ É muito **mais eficiente** do que criar várias variáveis separadas.  
✅ Loops como `for` **facilitam a manipulação dos valores** de um vetor.  