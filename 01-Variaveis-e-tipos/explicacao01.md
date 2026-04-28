# 📦 Módulo 01: Variáveis e Tipos de Dados em Python

Agora que seu ambiente está configurado e você já fez o computador dizer "Olá, Mundo!", vamos entender como os programas guardam informações. Uma das coisas mais legais do Python é que ele é super inteligente e direto ao ponto!

---

## 🎯 O que você vai aprender

- O que são variáveis
- Como criar variáveis em Python (muito fácil!)
- Tipos de dados básicos
- Boas práticas de nomeação (`snake_case`)
- Como juntar textos e variáveis (As famosas f-strings)

---

## 🧠 Conceito: O que é uma variável?

Pense na memória do seu computador como um grande armazém. Uma **variável** é como uma **caixa** dentro desse armazém onde você guarda um dado.

Toda caixa precisa de duas coisas principais:

1. **Nome (Etiqueta):** Para você achar a caixa depois.
2. **Valor:** O que tem dentro da caixa.

_(O Python é tão esperto que ele adivinha o formato da caixa sozinho, só olhando para o que você colocou lá dentro!)_

---

## ✍️ Como declarar uma variável

A "fórmula" para criar essa caixa em Python é super simples:

```python
nome_da_variavel = valor
Exemplo na prática:
```

```python
idade = 20
nome = "Pedro"
altura = 1.75
```

## 🔢 Tipos de dados mais usados no dia a dia

Mesmo que a gente não precise escrever o tipo, o Python sabe classificá-los por trás dos panos. Vamos focar nos "Quatro Fantásticos":

🔹 Números inteiros (int)
Serve para idades, quantidades, anos.

```python
idade = 20
```

🔹 Números com casas decimais (float)
Serve para dinheiro, altura, peso. (Atenção: em programação usamos ponto ., não vírgula ,)

```python
altura = 1.75
```

🔹 Texto (str ou string)
Serve para nomes, frases, senhas. O texto deve estar sempre entre aspas duplas "" ou simples ''.

```python
nome = "Pedro"
```

🔹 Booleano (bool)
Só aceita dois valores: Verdadeiro ou Falso.
(Dica de Ouro: em Python, a primeira letra deve ser MAIÚSCULA)

```python
estudante = True
trabalhando = False
```

## 🔄 Variáveis podem... variar!

O legal das variáveis é que você pode trocar o que tem dentro da caixa a qualquer momento no seu código:

```Python
pontuacao = 10
```

## ops, ganhei mais pontos!

pontuacao = 15

## Agora a caixa 'pontuacao' não vale mais 10, vale 15.

📏 Regras e Boas Práticas para Nomes
Para dar nome às suas caixas, existem regras:

❌ Não pode começar com número: 1idade

❌ Não usar espaços: nome completo

✅ Use nomes claros: idade, valor_total

✅ Use o padrão snake_case: No Python, a convenção é escrever tudo em minúsculo e separar as palavras por underline (underline imita uma cobrinha, daí o nome snake_case). Ex: valor_da_compra, nome_do_aluno.

🧩 O "Pulo do Gato": Juntando Texto e Variável (f-strings)
Como fazemos para imprimir uma frase bonitinha juntando texto e variáveis? Em Python, nós temos um "superpoder" chamado f-string.

Basta colocar a letra f antes das aspas, e colocar suas variáveis dentro de chaves { }. Veja a mágica:

```python
nome = "Pedro"
idade = 20

print(f"Olá, meu nome é {nome} e eu tenho {idade} anos.")
```

💻 Exemplo completo
Copie e cole este código no seu arquivo, rode, e veja acontecer:

```python
nome = "Maria"
idade = 25
altura = 1.68
gosta_de_cafe = True

print("--- Ficha de Cadastro ---")
print(f"Nome: {nome}")
print(f"Idade: {idade}")
print(f"Altura: {altura}m")
```

# 🧪 Hora de Praticar!

Chegou a sua vez de colocar a mão na massa. Crie um arquivo chamado meus_dados.py e resolva os exercícios abaixo.

Exercício 1
Crie variáveis com os tipos corretos para armazenar:

O seu nome

A sua idade

A sua altura

Se você gosta de programar (True ou False)

Mostre os valores no console usando print().

# 🚀 Desafio Final

Usando o que você aprendeu sobre f-strings (colocar o f antes das aspas e usar { }), crie um programa que imprima exatamente esta frase no terminal, substituindo os espaços pelas suas variáveis:

"Meu nome é {nome}, tenho {idade} anos e minha altura é {altura}."
