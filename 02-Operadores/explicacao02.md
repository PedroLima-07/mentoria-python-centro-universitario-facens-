# 🧮 Módulo 02: Operadores em Python

No módulo anterior, aprendemos a criar variáveis (nossas caixas) e guardar informações nelas. Mas um programa de verdade precisa fazer cálculos, comparar valores e tomar decisões. É aqui que entram os **Operadores**!

Pense nos operadores como as "ações" que acontecem entre as nossas variáveis. E a boa notícia: em Python, isso é quase como escrever em inglês!

---

## 🎯 O que você vai aprender

- Operadores Aritméticos (Matemática básica + Poderes do Python)
- O perigoso (mas útil) operador de Resto (`%`)
- Operadores de Atribuição (Atalhos)
- Operadores Relacionais (Fazendo perguntas de Sim/Não)
- Operadores Lógicos (`and`, `or`, `not`)

---

## ➕ 1. Operadores Aritméticos (Matemática)

Esses são os que você já conhece da escola. Eles pegam números, fazem uma conta e devolvem um novo número.

- `+` : Soma
- `-` : Subtração
- `*` : Multiplicação (usamos o asterisco, e não o "x")
- `/` : Divisão (Sempre devolve um número com casa decimal, ex: `2.5`)
- `//`: Divisão Inteira (Ignora as casas decimais, ex: `5 // 2` resulta em `2`)
- `**`: Exponenciação (Potência. Ex: `2 ** 3` é 2 elevado a 3, que dá 8)
- `%` : Módulo (Resto da divisão)

**Exemplo prático:**

```python
a = 10
b = 3

print(a + b)  # Imprime 13
print(a * b)  # Imprime 30
print(a / b)  # Imprime 3.333333...
print(a // b) # Imprime 3 (Corta a parte decimal)
```

### 💡 Atenção ao Módulo (%)!

Ele não é porcentagem! Ele pega o resto da divisão.
Exemplo: Se você tem 10 fatias de pizza e divide para 3 pessoas, cada um come 3 fatias e sobra 1.
Logo, 10 % 3 é igual a 1. É muito usado para descobrir se um número é par ou ímpar!

## 🔄 2. Operadores de Atribuição (Os Atalhos)

Lembra que o sinal de igual = significa "recebe"? Ele pega o que está na direita e guarda na variável da esquerda.
Mas na programação, muitas vezes queremos atualizar o valor de uma variável baseada nela mesma.

Em vez de escrever:
pontos = pontos + 5

Nós usamos os atalhos:

+= : Soma e guarda (Ex: pontos += 5)

-= : Subtrai e guarda

\*= : Multiplica e guarda

/= : Divide e guarda

### 🛑 DICA DE OURO DO MENTOR: ONDE ESTÁ O ++?

Se você já viu código em outras linguagens, deve conhecer o idade++ para somar 1. O Python NÃO tem isso! Se quiser somar 1, você deve usar idade += 1.

## ⚖️ 3. Operadores Relacionais (As Comparações)

Aqui as coisas ficam interessantes. Esses operadores comparam dois valores e a resposta SEMPRE será um valor Booleano (True ou False). É como se você estivesse fazendo uma pergunta ao Python.

== : É igual a? (Atenção: são DOIS sinais de igual!)

!= : É diferente de?

> : É maior que?

< : É menor que?

> = : É maior ou igual a?

<= : É menor ou igual a?

Exemplo prático:

```python
idade = 18
maior_de_idade = idade >= 18 # Pergunta: 18 é maior ou igual a 18? SIM (True).

print(f"É maior de idade? {maior_de_idade}") # Imprime True
```

### 🛑 NUNCA CONFUNDA = COM ==

idade = 18 significa "A variável idade AGORA VALE 18".
idade == 18 significa "A variável idade É IGUAL A 18?".

## 🧠 4. Operadores Lógicos (Juntando Regras)

Às vezes, uma comparação só não basta. Imagina que para entrar em uma festa você precisa ter ingresso E ser maior de idade. O Python facilita muito isso usando palavras do inglês!

and (E): Tudo tem que ser verdade.

or (OU): Basta um ser verdade para tudo ser verdade.

not (NÃO): Inverte o resultado (se era True, vira False).

Exemplo prático:

```python
tem_ingresso = True
idade = 20

# Só entra se TIVER ingresso E a idade for MAIOR OU IGUAL a 18
pode_entrar = tem_ingresso and (idade >= 18)

print(f"Pode entrar na festa? {pode_entrar}") # Imprime True
```

## 💻 Exemplo Completo

Copie e rode no seu arquivo para ver como tudo se encaixa:

```python
valor_produto = 100.0
quantidade = 2
```

# 1. Aritmético: Calculando o total

```python
total = valor_produto * quantidade # 200.0
```

# 2. Relacional e Lógico: Regra para frete grátis (Acima de 150 reais OU cliente VIP)

```python
cliente_vip = False
tem_frete_gratis = (total > 150.0) or cliente_vip

print(f"Valor total da compra: R$ {total}")
print(f"Tem frete grátis? {tem_frete_gratis}")
```

## 🧪 Hora de Praticar!

Chegou a sua vez! Vá para a pasta exercicios e abra o arquivo exercicios.md.
Lá você encontrará os desafios para testar se a lógica dos operadores já está fazendo sentido na sua cabeça.
