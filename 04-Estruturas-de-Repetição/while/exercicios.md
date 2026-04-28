# 🏋️‍♂️ Exercícios: Dominando o Laço While

Agora é a sua vez! Lembre-se: no primeiro exercício você vai usar o `while` clássico com uma condição. No segundo e no terceiro, você vai usar o poder do `while True:` com `break`.

Crie os arquivos `.py` no seu VS Code e mãos à obra!

---

### 💰 Exercício 1: Meta de Economia (While Clássico)

**Arquivo:** `poupanca.py`

**Cenário:** Você quer comprar um videogame que custa R$ 3.000,00. Todo mês você consegue guardar R$ 450,00. Quantos meses você vai levar para bater a meta?

**O que você deve fazer:**

1. Crie as variáveis `saldo = 0.0`, `meta = 3000.0` e `meses = 0`.
2. Crie um `while` que repita o código **enquanto** o saldo for **menor** que a meta.
3. Dentro do laço:
   - Adicione 450.0 ao saldo (`saldo += 450.0`).
   - Adicione 1 à variável meses.
4. No final, **fora do laço**, imprima quantos meses demorou e qual foi o saldo final.

---

### 🎲 Exercício 2: Jogo de Adivinhação (Simulando Do-While)

**Arquivo:** `adivinhacao.py`

**Cenário:** O computador pensou em um número de 1 a 10 e o usuário precisa adivinhar digitando no teclado.

**O que você deve fazer:**

1. Defina um número secreto (ex: `numero_secreto = 7`).
2. Use o `while True:` para iniciar o jogo.
3. Dentro do laço, peça o palpite do usuário usando `int(input("Digite seu palpite: "))`.
4. Se o palpite for igual ao número secreto, imprima _"Parabéns, você acertou!"_ e use o `break`.
5. Se for diferente, dê dicas usando `elif` ("Tente um número maior" ou "Tente um número menor").

---

### 🍕 Desafio: Pedido de Lanchonete

**Arquivo:** `lanchonete.py`

**Cenário:** Crie um sistema de autoatendimento onde o cliente pode escolher vários itens.

**O que você deve fazer:**

1. Crie uma variável `total_conta = 0.0`.
2. Inicie o `while True:` mostrando o cardápio:
   - 1. Hamburguer (R$ 20.0)
   - 2. Refri (R$ 5.0)
   - 0. Finalizar Pedido
3. Leia a escolha do usuário com `input()`.
4. Use `if/elif` (ou o moderno `match case`!) para somar o valor na `total_conta` dependendo da escolha.
5. Se for 0, use o `break` para sair do cardápio.
6. No final (fora do laço), mostre o valor total a pagar.
