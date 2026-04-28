# ✅ Gabarito: Módulo 01 - Variáveis e Tipos (Python)

Se você chegou até aqui, **parabéns por ter tentado!** É super normal travar no começo. A programação é como aprender um novo idioma: no início, a gente tropeça nas palavras, mas com a prática tudo fica natural.

Como você deve ter percebido, escrever em Python é muito rápido e direto! Abaixo estão as nossas sugestões de resolução.

---

## 🛠️ Resolução: Exercício 1 (meus_dados.py)

**O objetivo:** Criar variáveis com os tipos corretos para nome, idade, altura e se gosta de programar, e depois imprimir tudo.

**Como resolvemos:**

```python
# 1. O seu nome é um TEXTO (String), fica entre aspas.
nome = "Carlos"

# 2. A sua idade é um número INTEIRO (int).
idade = 28

# 3. A sua altura tem casas decimais (float).
# Lembre-se: usamos ponto (.) ao invés de vírgula (,).
altura = 1.82

# 4. Se gosta de programar é uma pergunta de SIM ou NÃO (Booleano).
# Lembre-se: em Python, começa com a primeira letra maiúscula!
gosta_de_programar = True

# Agora, usamos o comando print() para mostrar tudo na tela:
print("--- Meus Dados ---")
print(nome)
print(idade)
print(altura)
print(gosta_de_programar)
```

# 🚀 Resolução: Desafio Final (desafio_final.py)

O objetivo: Usar as f-strings para montar uma frase dinâmica.

Como resolvemos:

```python
# Primeiro, criamos as nossas variáveis
nome = "Ana"
idade = 22
altura = 1.65

# Agora vem a mágica da f-string!
# O 'f' minúsculo fica coladinho do lado de fora das aspas,
# e o nome das variáveis entram nas chaves {}

print(f"Meu nome é {nome}, tenho {idade} anos e minha altura é {altura}.")
```

## 💡 Dica do Mentor: O erro do "f" esquecido

Um erro muito comum no começo é esquecer de colocar a letrinha f antes das aspas.
Se você escrever: print("Meu nome é {nome}") sem o f, o Python vai imprimir literalmente as chaves, ignorando a sua variável! Sempre verifique se o f está lá!
