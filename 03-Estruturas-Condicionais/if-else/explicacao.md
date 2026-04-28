# 🔀 Tomando Decisões: If, Elif e Else (Python)

Bem-vindo ao coração da lógica de programação! Até agora, nossos programas faziam sempre a mesma coisa. Mas, no mundo real, as ações dependem de **condições**.

- "Se chover, levo guarda-chuva. Senão, levo óculos de sol."

Em Python, nós ensinamos o computador a tomar essas decisões usando as palavras `if` (se), `elif` (senão se) e `else` (senão).

---

## ⚠️ A Regra de Ouro do Python: Indentação e Dois Pontos ( : )

Diferente de outras linguagens que usam chaves `{}` para agrupar o código, o Python usa **espaços** (indentação).
Toda vez que você criar uma condição, você deve colocar `:` no final da linha e apertar a tecla _Tab_ (ou dar 4 espaços) na linha de baixo.

O Python só sabe que um código está "dentro" do `if` se ele estiver empurradinho para a direita!

---

## 🚦 1. O básico: O `if` (Se)

O `if` é como um porteiro. Ele verifica uma condição. Se for verdadeira (`True`), ele abre a porta e executa o código que está indentado (com espaço) embaixo dele.

```python
idade = 20

# O porteiro faz a pergunta. Não esqueça dos dois pontos no final!
if idade >= 18:
    # Como tem esse espaço aqui, o Python sabe que essa linha pertence ao if
    print("Acesso liberado. Pode entrar!")
```

## 🛑 2. A alternativa: O else (Senão)

E se a pessoa tiver 15 anos? O if vai dar falso. Para dar uma resposta quando a condição falha, usamos o else.

O else nunca tem uma condição do lado dele, porque ele significa "em qualquer outro caso".

```python
idade = 15

if idade >= 18:
    print("Acesso liberado. Pode entrar!")
else:
    # O else também precisa de dois pontos e indentação na linha de baixo!
    print("Acesso negado. Volte para casa.")
```

## 🛤️ 3. Múltiplos Caminhos: O elif (Senão Se)

Às vezes, a vida não é só "preto no branco". Imagine classificar a idade de alguém em Criança, Adolescente ou Adulto.
Em vez de escrever else if como em outras linguagens, o Python encurtou para elif:

```python
idade = 14

if idade < 12:
    print("Você é uma Criança.")
elif idade < 18:
    # O Python só chega aqui se a primeira condição for falsa.
    print("Você é um Adolescente.")
else:
    # Se não for criança nem adolescente, só pode ser adulto!
    print("Você é um Adulto.")
```

## 💻 Exemplo Completo

Copie e cole este código no seu arquivo, mude o valor da variável valor_saque e veja como o programa toma caminhos diferentes:

```python
saldo = 100.0
valor_saque = 150.0

print(f"Tentando sacar R$ {valor_saque}...")

if valor_saque <= saldo:
    saldo -= valor_saque # Atualiza o saldo (Atalho para saldo = saldo - valor_saque)
    print("Saque realizado com sucesso!")
    print(f"Novo saldo: R$ {saldo}")
else:
    print("Operação negada: Saldo insuficiente.")
```

Pronto para testar sua lógica? Vá para o arquivo exercicios.md!
