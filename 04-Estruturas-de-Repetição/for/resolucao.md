# ✅ Gabarito: Laço For (Python)

O segredo do `for` no Python é entender como o `range()` funciona. Se você lembrou que o limite final é exclusivo (ele para um antes), você foi muito bem!

Confira as soluções sugeridas:

---

## 🚀 Resolução: Exercício 1 (foguete.py)

```python
print("Iniciando sequência de lançamento...")

# Começa no 10, vai até o 0 (exclusivo, para no 1) e diminui 1 por vez
for i in range(10, 0, -1):
    print(i)

print("Fogo! 🚀")
```

## ✖️ Resolução: Exercício 2 (tabuada.py)

```python
numero = 7

print(f"Tabuada do {numero}:")

# Usamos range(1, 11) para ele incluir o número 10
for i in range(1, 11):
    resultado = numero * i
    print(f"{numero} x {i} = {resultado}")
```

## 💰 Resolução: Desafio (soma_intervalo.py)

Como resolvemos:
Usamos uma técnica chamada Acumulador. Criamos a variável fora do laço para ela não ser "zerada" a cada repetição.

```python
soma = 0

# Para somar até o 50, o range deve ir até o 51
for i in range(1, 51):
    soma += i # Soma o valor atual de 'i' ao total já guardado

print(f"A soma total de 1 a 50 é: {soma}")
```
