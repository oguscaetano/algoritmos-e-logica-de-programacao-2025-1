# 📚 **[SIMULADO - A2.2] Lógica de Programação e Algoritmos**

### Instruções:  
- Leia atentamente cada enunciado, interprete o que está sendo solicitado e desenvolva o algoritmo em linguagem C; 
- Lembre-se de declarar variáveis corretamente, usar entradas e saídas de dados e aplicar as estruturas de controle conforme pedido;
- Se o aluno for pego utilizando qualquer tipo de dispositivo com acesso a internet, sua nota será zerada;
- Se o aluno for pego colando de outro aluno, sua nota será zerada;
- Escreva os algoritmos com caneta, em letra de forma o mais legível possível (não será aceito lápis);

## Questão 1 – O Jogo dos Dados 🎲  (1 ponto)

No Reino dos Dados, existe um campeonato onde cada jogador precisa lançar dois dados. Dependendo da soma dos valores dos dados e de seu nome de jogador, ele pode ganhar uma pontuação bônus.  
Crie um programa que:

- Peça ao usuário:
  - O nome do jogador,
  - O valor do primeiro dado,
  - O valor do segundo dado,
  - O tempo de resposta do jogador em segundos.
- Calcule a soma dos valores dos dados.
- Se a soma for **maior ou igual a 10** e o tempo de resposta for **menor que 5 segundos**, exiba "Bônus concedido!".
- Caso contrário, exiba "Sem bônus dessa vez."

## Questão 2 – O Cofrinho da Aventura 💰 (1 ponto)

Na cidade de Códigolândia, o pequeno Alex decidiu juntar moedas para comprar um novo videogame. Cada dia, ele economiza uma quantidade diferente de moedas.  
Você precisa criar um programa que:

- Peça para o usuário informar quantos dias ele economizou moedas.
- Depois, peça para informar a quantidade de moedas economizadas em **cada dia**.
- **Use uma função** chamada `totalMoedas` que recebe a quantidade de dias e retorna o total de moedas economizadas.
- No final, imprima o valor total economizado.

## Questão 3 – Arena dos Campeões 🏟️ (3 pontos)

Em um grande torneio de luta em equipe, existem 4 times, cada um com 3 lutadores.  
Cada lutador recebe uma nota de avaliação entre 0 e 10. A equipe vencedora será aquela cuja **média dos lutadores** for a maior.  
Sua solução precisa ter uma função chamada `avaliarTime` para calcular a média de um time.
Exiba ao final a média de cada time e qual time é o grande campeão.

Formato da saída:
```
Notas do Time 1:
Digite a nota do Lutador 1: 9.5
Digite a nota do Lutador 2: 8
Digite a nota do Lutador 3: 7.5
Notas do Time 2:
Digite a nota do Lutador 1: 10
Digite a nota do Lutador 2: 2.5
Digite a nota do Lutador 3: 5.5
Notas do Time 3:
Digite a nota do Lutador 1: 7.5
Digite a nota do Lutador 2: 5.5
Digite a nota do Lutador 3: 6
Notas do Time 4:
Digite a nota do Lutador 1: 9.5
Digite a nota do Lutador 2: 8.5
Digite a nota do Lutador 3: 4.5
Media do Time 1: 8.00
Media do Time 2: 5.67
Media do Time 3: 6.00
Media do Time 4: 7.00

O grande campeao e o Time 1 com media 8.00!
```
