## ✅ Exercício 1 – Calculadora do Racha
Você e seus amigos foram ao cinema e dividiram a conta igualmente. Crie um programa que receba o valor total da conta e a quantidade de amigos. O programa deve calcular quanto cada um deve pagar.

## ✅ Exercício 2 – Qual seu desempenho gamer?
Um jogo classifica seu desempenho de acordo com a pontuação:

* Até 1000 pontos: Iniciante
* De 1001 a 5000: Intermediário
* Acima de 5000: Pro player

Crie um programa que leia a pontuação e mostre o nível do jogador.

## ✅ Exercício 3 – Menu da Lanchonete
Implemente um menu de lanchonete usando `switch case`. O cliente digita o número do item desejado e o programa exibe o nome do item. Exemplo:

1 - Hambúrguer  
2 - Batata Frita  
3 - Refrigerante  

## ✅ Exercício 4 – Contador de passos
Você quer contar quantos passos dá em 7 dias. Faça um programa que leia os passos dados por dia e calcule o total.

## ✅ Exercício 5 – Até acertar
Implemente um jogo em que o usuário deve adivinhar o número secreto (fixo, por exemplo 42). O programa só termina quando ele acertar.

## ✅ Exercício 6 – Notas do semestre
Uma disciplina tem 3 notas. Crie uma função `float calcularMedia(float n1, float n2, float n3)` que retorna a média. No `main`, leia as 3 notas, chame a função e mostre a média.

### ✅ Exercício 7 – Censura automática
Você é programador de uma rede social e precisa censurar uma palavra. Leia uma frase de até 50 caracteres e um caractere proibido, e imprima a frase com os caracteres proibidos substituídos por `*`.

## ✅ Exercício 8 – Média de uma turma
Uma turma tem 5 alunos. Cada aluno tem 2 notas. Armazene essas notas em uma matriz 5x2. Calcule a média de cada aluno e diga se está aprovado (média ≥ 6).

## ✅ Exercício 9 – Busca de nome
Você criou um sistema para um campeonato de eSports com 5 participantes. Os nomes são armazenados em um array de strings. O programa deve perguntar um nome e informar se ele está ou não cadastrado.

## ✅ Exercício 10 – Jogo da Matriz
Você está programando um minigame de labirinto em uma matriz 3x3. O jogador começa no canto superior esquerdo (0,0). Ele se move digitando W (cima), A (esquerda), S (baixo) e D (direita). Após 5 movimentos, o programa deve imprimir a posição final do jogador.

## ✅ **DESAFIO – Controle de Estudantes de Hogwarts**
Você foi contratado para programar um sistema simplificado de controle de notas dos estudantes da Escola de Magia e Bruxaria de Hogwarts.

A escola possui 4 casas: Grifinória, Sonserina, Corvinal e Lufa-Lufa. Cada casa possui 3 alunos. Para cada aluno, devem ser armazenadas 2 notas de provas.

O sistema deve realizar as seguintes tarefas:

1. **Cadastro:** Preencher os nomes dos alunos de cada casa e suas respectivas notas (duas por aluno).
2. **Cálculo da média:** Calcular a média de cada aluno usando uma **função**.
3. **Classificação:** Exibir se o aluno foi aprovado (média ≥ 7), recuperação (entre 4 e 6.9), ou reprovado (abaixo de 4) — usando **if/else**.
4. **Consulta:** O usuário pode digitar o nome de um aluno e o programa informará a casa em que ele está, suas notas e a média.
5. **Relatório final:** Mostrar a média geral de cada casa e destacar qual casa teve o melhor desempenho.

### 🧠 Dicas:

* Crie arrays de `char` para os nomes: `char nomes[4][3][20];`
* Crie uma matriz para as notas: `float notas[4][3][2];`
* Use `switch case` para o menu.
* Crie uma função `float calcularMedia(float n1, float n2)`.
