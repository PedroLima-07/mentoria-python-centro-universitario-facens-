# 🏋️‍♂️ Exercícios: Dominando as Listas

Chegou a hora de praticar! O Python facilita muito o uso de listas, mas a lógica por trás é a mesma de qualquer linguagem. Crie os arquivos `.py` no seu VS Code e resolva os problemas abaixo.

---

### 📝 Exercício 1: A Chamada da Turma

**Arquivo:** `chamada.py`

**Cenário:** Você precisa listar o nome dos alunos que chegaram na sala de aula.

**O que você deve fazer:**

1. Crie uma lista já preenchida com 5 nomes de sua escolha (ex: `["Pedro", "Ana", ...]`).
2. Crie um laço `for` pythonico (`for aluno in lista:`) para percorrer essa lista.
3. Imprima no console uma mensagem de boas-vindas usando f-string para cada aluno. (Ex: "Bem-vindo(a), Pedro!").

---

### 📊 Exercício 2: Calculadora de Boletim

**Arquivo:** `boletim.py`

**Cenário:** Um professor quer automatizar o cálculo da média de um aluno que fez 4 provas durante o ano.

**O que você deve fazer:**

1. Crie uma lista chamada `notas` com os valores: `8.5`, `7.0`, `9.0` e `5.5`.
2. Crie uma variável `soma = 0.0` antes do laço para acumular o total.
3. Use um laço `for` para percorrer a lista e ir somando cada nota na variável `soma`.
4. Após o laço, calcule a média dividindo a soma pela quantidade de notas. _(Dica de Ouro: para saber o tamanho de uma lista em Python, use a função `len(notas)`)._
5. Imprima a soma total e a média final do aluno.

---

### 🚀 Desafio: Encontrando o Maior Número

**Arquivo:** `maior_numero.py`

**Cenário:** Você tem uma lista de pontuações de um jogo e precisa descobrir qual foi o recorde (o maior número).

**O que você deve fazer:**

1. Crie uma lista chamada `pontuacoes` com os valores: `45`, `89`, `32`, `104`, `77`.
2. Crie uma variável chamada `maior` e diga que o valor inicial dela é igual à primeira gaveta da lista (ex: `maior = pontuacoes[0]`).
3. Crie um laço `for` para percorrer a lista.
4. Dentro do laço, faça um `if`: se a pontuação atual for maior que a variável `maior`, então a variável `maior` recebe esse novo valor.
5. No final, imprima o recorde encontrado!
