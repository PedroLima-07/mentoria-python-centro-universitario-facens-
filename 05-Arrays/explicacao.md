# 📦 Módulo 05: Listas (Arrays) em Python

Até agora, nossas variáveis eram como "caixas pequenas" que guardavam um único valor por vez. Se quiséssemos guardar o nome de 5 alunos, teríamos que criar 5 variáveis diferentes (`aluno1`, `aluno2`...). Imagina fazer isso para uma escola inteira?

É para resolver esse problema que existem as **Listas** (conhecidas como Arrays ou Vetores em outras linguagens).

Uma Lista é como um **armário com várias gavetas numeradas**. Ela guarda vários valores dentro de uma única variável.

---

## ✍️ Como criar uma Lista em Python?

Criar uma lista em Python é a coisa mais fácil do mundo. Nós usamos **colchetes `[ ]`**.

### Forma 1: Criando a lista já preenchida

Se você já sabe quais valores quer guardar, é só colocar tudo lá dentro, separado por vírgula.

```python
# Uma lista de textos (Strings)
nomes = ["Ana", "Carlos", "Beatriz"]

# Uma lista de números
idades = [20, 25, 18]
```

### Forma 2: Criando a lista vazia

Se você ainda não tem os dados (vai pedir para o usuário digitar, por exemplo), pode criar a lista vazia e encher depois.

```python
carrinho_de_compras = []
```

### 🚨 A Regra de Ouro: O índice começa no ZERO!

Na vida real, nós começamos a contar do 1. Na programação, nós começamos a contar do ZERO.
O número da gaveta é chamado de índice (ou index).

Se a sua lista tem 3 itens, as gavetas são: 0, 1 e 2.

```python
nomes = ["Ana", "Carlos", "Beatriz"]

print(nomes[0]) # Imprime "Ana"
print(nomes[1]) # Imprime "Carlos"
print(nomes[2]) # Imprime "Beatriz"

# print(nomes[3]) -> ❌ ERRO! IndexError: list index out of range (Essa gaveta não existe!)
```

## ➕ Adicionando e Alterando valores

Diferente de outras linguagens, a lista do Python é "elástica". Você pode adicionar novos itens no final dela a qualquer momento usando o "poder" .append().

```python
filmes = ["Matrix", "Avatar"]

# Adiciona um novo filme no final da lista
filmes.append("O Senhor dos Anéis")

print(filmes) # Vai imprimir: ['Matrix', 'Avatar', 'O Senhor dos Anéis']
Para trocar um valor que já existe, basta acessar a gaveta e usar o sinal de = :

Python
notas = [8.0, 5.0, 9.0]
notas[1] = 7.0  # Ops, o aluno recuperou a nota! Trocando o 5.0 por 7.0
```

## 🔄 O Pulo do Gato: Listas + Laço For

Aqui é onde o Python brilha muito! Lembra que no for do Python nós lemos "Para cada item na sequência..."?
Você não precisa criar contadores nem acessar índices para ler uma lista. O Python faz o trabalho sujo para você!

```python
frutas = ["Maçã", "Banana", "Uva", "Morango"]

# O Python pega cada item da lista e joga na variável 'fruta', um de cada vez!
for fruta in frutas:
    print(f"Eu adoro comer {fruta}")
```

Pronto para organizar seus dados? Vá para o arquivo exercicios.md e coloque a mão na massa!
