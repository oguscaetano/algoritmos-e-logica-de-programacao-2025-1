## **Exercício 1 – Top 5 Músicas da Semana**
Você foi contratado pelo "TopMusic", um aplicativo de streaming, para desenvolver um programa que permita ao usuário inserir os nomes das 5 músicas mais tocadas da semana.  
O sistema só deve aceitar músicas que tenham mais de 3 caracteres.  
Crie uma função chamada `cadastrarMusicas()` que utilize um `while` para coletar os nomes válidos e armazená-los em um array de strings. Após o cadastro, exiba as músicas na ordem digitada.

## **Exercício 2 – Ranking de Jogadores**
Você está criando um sistema de ranking de um torneio de e-sports com até 10 jogadores. Cada jogador digita seu nome e pontuação (0 a 100).  
O sistema deve perguntar se o próximo jogador deseja se cadastrar. O loop deve continuar até que o usuário digite "n".  
Crie uma função chamada `mostrarRanking()` que exibe todos os jogadores com pontuação maior ou igual a 60, marcando-os como “Aprovado”, e os demais como “Desclassificado”.

## **Exercício 3 – Lanchonete TechBurguer**
A lanchonete TechBurguer quer automatizar os pedidos de até 5 clientes. Cada cliente escolhe um dos três lanches disponíveis:
- 1: X-Burguer
- 2: X-Salada
- 3: Vegano

O sistema deve validar o código (1, 2 ou 3) usando `while`. Crie uma função chamada `resumoPedidos()` que, ao final, exibe quantos pedidos foram feitos de cada tipo de lanche.

## **Exercício 4 – Média de Arremessos**
Em um torneio de basquete, cada jogador pode tentar até 5 arremessos. Você deve criar um sistema que receba os pontos obtidos por tentativa (0, 2 ou 3 pontos) até que o jogador deseje parar (confirmando com 'n').  
Utilize um `do while` para as tentativas e uma função chamada `calcularMedia()` para retornar a média de pontos por tentativa.

## **Exercício 5 – Controle de Leitura de Livros**
Você está desenvolvendo um sistema para ajudar os alunos a monitorarem sua leitura de livros. O sistema deve permitir que o aluno insira o nome de até 6 livros.  
Se o aluno já leu o livro (digitando 's'), ele é armazenado no array. Crie uma função `exibirLidos()` para mostrar todos os livros lidos.
