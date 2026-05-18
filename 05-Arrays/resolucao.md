# ✅ Gabarito: Listas em Python

Parabéns por chegar até aqui! Se você veio de outras linguagens, deve ter notado como o Python deixa o código muito mais limpo na hora de varrer uma lista com o `for`.

Confira as soluções passo a passo:

---

## 📝 Resolução: Exercício 1 (chamada.py)

**Como resolvemos:**
Usamos a estrutura de `for` direta do Python. Não precisamos nos preocupar com índices numéricos aqui.

```python
# 1. Criando a lista já com os valores
alunos = ["Lucas", "Mariana", "Roberto", "Fernanda", "Diego"]

print("--- Lista de Presença ---")

# 2. O laço for pega um por um e guarda na variável 'aluno'
for aluno in alunos:
    print(f"Bem-vindo(a), {aluno}!")
```

## 📊 Resolução: Exercício 2 (boletim.py)

Como resolvemos:
O segredo aqui é usar a variável soma como um acumulador dentro do laço. E para não ter que "adivinhar" o tamanho da lista na hora de dividir, usamos a função mágica len() (de length/tamanho).

```python
notas = [8.5, 7.0, 9.0, 5.5]
soma = 0.0

# Percorre a lista e soma cada nota
for nota in notas:
    soma += nota

# Calcula a média usando o tamanho dinâmico da lista (len)
media = soma / len(notas)

print(f"Soma das notas: {soma}")
print(f"Média final: {media}")
```

### 💡 Curiosidade Pythonica: O Python é tão prático que ele tem uma função chamada sum() que soma tudo automaticamente! Se você quisesse fazer sem o for, bastava escrever: media = sum(notas) / len(notas). Mas usar o for é essencial para treinar a sua lógica!

## 🚀 Resolução: Desafio (maior_numero.py)

Como resolvemos:
Esta é uma lógica clássica de programação. Assumimos que o primeiro número (índice 0) é o maior. Depois, olhamos para os outros. Se algum for maior do que o que temos guardado, nós atualizamos o título de "maior".

```python
pontuacoes = [45, 89, 32, 104, 77]

# Assumimos que o recorde inicial é o primeiro valor da lista
maior = pontuacoes[0]

# O for vai passar por todos os números...
for pontuacao in pontuacoes:

    # Se o valor atual for maior que o nosso recorde guardado...
    if pontuacao > maior:
        maior = pontuacao # ...atualizamos o recorde!

print(f"🏆 O recorde do jogo é: {maior}")
```

### 💡 Curiosidade Pythonica (Parte 2): Assim como a soma, o Python também tem um atalho para isso! A função max(pontuacoes) encontraria o maior número sozinha.
