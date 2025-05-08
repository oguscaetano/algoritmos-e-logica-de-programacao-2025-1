# **PROVA A2.2 - LÓGICA DE PROGRAMAÇÃO E ALGORITMOS**

## Pontuação total da prova: `3 PONTOS`

## Instruções:  
- Leia atentamente cada enunciado, interprete o que está sendo solicitado e desenvolva o algoritmo na linguagem C; 
- Lembre-se de declarar variáveis corretamente, usar entradas e saídas de dados e aplicar as estruturas de controle conforme pedido;
- Se o aluno for pego utilizando qualquer tipo de dispositivo com acesso a internet sem autorização prévia, sua nota será zerada (celular, tablet, laptop ...);
- Se o aluno for pego colando de outro aluno, sua nota será zerada;
- O aluno deverá enviar as respostas da prova via portal do Blackboard;
    - Para fazer isso, peça autorização ao professor (somente solicite após todo o processo já ter sido feito)
    - O aluno terá apenas uma tentativa de submissão
    - O aluno deverá colocar os códigos um abaixo do outro em uma mesma submissão dentro do campo de texto
    - Exemplo: 
        - // Exercício 1:  
        código
        - // Exercício 2:  
        código
        - // Exercício 3:  
        código
- O aluno que submeter a prova sem estar presente na sala de aula terá sua nota zerada;
- O professor não tirará nenhuma dúvida durante a prova;
- É permitido o uso de qualquer IDE, desde que seja offline;
- Ao final da prova o aluno deverá assinar a lista de chamada;
- Duração da prova: 19h as 21h50

## Questão 1 — Jogos da Nintendo (1 ponto)

Durante o campeonato mundial de *Super Smash Bros.*, um jogador deve escolher seu personagem (Mario, Link ou Pikachu) e informar sua idade e sua pontuação final na competição. Com base nesses dados:

* Se a pontuação for maior ou igual a 8.0 e a idade for menor que 18, ele será classificado como **Jovem Promessa**.
* Se a pontuação for maior ou igual a 8.0 e a idade for 18 ou mais, será classificado como **Campeão Experiente**.
* Se a pontuação estiver entre 5.0 e 7.9, independentemente da idade, será classificado como **Regular**.
* Caso contrário, será considerado **Eliminado**.

**Solicite ao usuário** o nome do personagem, a idade e a pontuação e exiba a classificação.

Exemplo de saída:
```
===================
Jogador: Link
Idade: 18
Pontuacao: 9.3
Classificacao: Campeao Experiente
```

## Questão 2 — Brasileirão Série  (1 ponto)

Você foi contratado(a) para criar um sistema simples que avalia o desempenho de clubes da Série A do Campeonato Brasileiro.

Cada clube recebe 3 notas de avaliação de desempenho tático (entre 0 e 10). Sua missão é:

1. Criar uma função chamada `avaliarClube` que receba um vetor com `N` clubes e retorne a média.
2. Para cada clube, leia suas 3 notas, calcule a média e classifique assim:

   * Média >= 8.0 → **Excelente**
   * Média >= 5.0 e < 8.0 → **Regular**
   * Média < 5.0 → **Fraco**

Exiba a média e a classificação de cada clube.

Exemplo de saída para `N = 2`:
```
Quantos clubes deseja avaliar? 2
Clube 1
Nota 1: 9.5
Nota 2: 2
Nota 3: 7.5

Media: 5.75 - Regular

=================

Clube 2
Nota 1: 1
Nota 2: 2
Nota 3: 3

Media: 1.50 - Fraco

=================
```

## Questão 3 — Spotify (3 pontos)

O Spotify deseja avaliar o desempenho de 3 playlists, cada uma com 4 músicas. Para isso, os usuários deram notas de popularidade (de 0 a 10) para cada música.

Sua missão é:

1. Criar uma função chamada `mediaPlaylist` que receba uma matriz de inteiros e o índice da playlist, e retorne a média de suas 4 músicas.
2. Preencher uma matriz 3x4 com as notas.
3. Calcular e exibir a média de cada playlist.
4. Determinar e exibir qual playlist teve a maior média.

Exemplo de saída:
```
Playlist 1:
Nota da musica 1: 9
Nota da musica 2: 8
Nota da musica 3: 7
Nota da musica 4: 9

Playlist 2:
Nota da musica 1: 2
Nota da musica 2: 7
Nota da musica 3: 6
Nota da musica 4: 9

Playlist 3:
Nota da musica 1: 10
Nota da musica 2: 10
Nota da musica 3: 5
Nota da musica 4: 7

====================

Media da Playlist 1: 8.25
Media da Playlist 2: 6.00
Media da Playlist 3: 8.00

Playlist vencedora: 1 com media 8.25
```
