## 1. Tamanho da String
Escreva um programa que leia uma string do usuário e imprima o seu tamanho (número de caracteres) usando `strlen()`.  

**Saída esperada:**  
```
Digite uma string: Hello
Tamanho da string: 5
```

## 2. Concatenar Strings
Peça ao usuário para digitar duas strings e concatene-as em uma terceira string usando `strcat()`. Imprima o resultado. 

**Saída esperada:**  
```
Digite a primeira string: Bom
Digite a segunda string: dia
Strings concatenadas: Bomdia
```

## 3. Comparar Strings  
Leia duas strings do usuário e use `strcmp()` para verificar se são iguais. Imprima "São iguais" ou "São diferentes".  

**Saída esperada:**  
```
Digite a primeira string: teste
Digite a segunda string: teste
São iguais
```

## 4. Converter String para Inteiro 
Leia uma string que representa um número inteiro (ex: "123") e use `atoi()` para convertê-la em um `int`. Depois, multiplique esse número por 2 e imprima o resultado.  

**Saída esperada:**  
```
Digite um número inteiro: 42
Dobro: 84
```

## 5. Alocação Dinâmica
Use `malloc()` para alocar memória para um array de 5 inteiros. Preencha o array com números digitados pelo usuário e depois imprima-os.  

**Saída esperada:**  
```
Digite 5 números:
10 20 30 40 50
Números digitados:
10 20 30 40 50
```

## 6. Números Aleatórios
Gere um número aleatório entre 1 e 100 usando `rand()` e imprima-o.  

**Saída esperada (exemplo):**  
```
Número aleatório: 73
```

## 7. Potência  
Peça ao usuário dois números (base e expoente) e calcule a potência usando `pow()`. Imprima o resultado.  

**Saída esperada:**  
```
Digite a base e o expoente: 2 8
Resultado: 256.00
```

## 8. Raiz Quadrada  
Leia um número do usuário e calcule sua raiz quadrada usando `sqrt()`.  

**Saída esperada:**  
```
Digite um número: 25
Raiz quadrada: 5.00
```

## 9. Arredondamento
Leia um número decimal e arredonde-o para o inteiro mais próximo usando `round()`.  

**Saída esperada:**  
```
Digite um número decimal: 3.6
Arredondado: 4
```

## 10. Seno e Cosseno  
Peça um ângulo em graus, converta-o para radianos e calcule seu seno e cosseno. 

**Saída esperada:**  
```
Digite o ângulo em graus: 45
Seno: 0.71
Cosseno: 0.71
```

## BÔNUS: Troca de Valores com Ponteiros
Escreva um programa que:  
1. Declare duas variáveis inteiras (`a` e `b`) com valores iniciais.  
2. Use **ponteiros** para trocar os valores dessas variáveis.  
3. Imprima os valores antes e depois da troca.  

**Exemplo de Saída:**  
```
Valores originais: a = 5, b = 10
Valores trocados: a = 10, b = 5
```