# 🔄 Estrutura For (Para): Percorrendo Caminhos

Se o `while` é o laço da incerteza, o **`for`** é o laço da precisão. Em Python, o `for` é usado quando queremos repetir algo um número específico de vezes ou percorrer cada item de uma coleção.

A frase que define o `for` no Python é: _"Para cada item dentro desta sequência, faça isso..."_

---

## ✍️ A Função `range()`: O nosso contador

Como o Python não usa aquela estrutura complicada do Java `(int i=0; i<10; i++)`, nós usamos a função **`range()`** para gerar uma sequência de números para nós.

### Como o `range(início, fim, passo)` funciona:

1. **Início:** Onde a contagem começa (se você não colocar, começa no 0).
2. **Fim:** Onde a contagem para (**Atenção:** o Python para um número ANTES do fim!).
3. **Passo:** De quanto em quanto ele pula (se não colocar, pula de 1 em 1).

---

## 💻 Exemplos Práticos

### 1. Contagem Simples (0 a 4)

```python
# O range(5) gera os números: 0, 1, 2, 3, 4
for i in range(5):
    print(f"Contagem: {i}")
```

2. Definindo Início e Fim (1 a 10)

```python
# Para contar de 1 até 10, precisamos ir até o 11!
for i in range(1, 11):
    print(f"Número: {i}")
```

3. Pulando de 2 em 2 (Números Pares)

```python
for i in range(0, 11, 2):
    print(f"{i} é um número par.")
```

## ⚙️ O que acontece por trás dos panos?

O Python faz o seguinte:

Ele pega o primeiro valor do range e guarda na variável i.

Executa o código que está indentado (com espaço) embaixo.

Volta para o topo, pega o próximo valor do range e coloca no i.

Repete isso até chegar no final da sequência.

### 💡 Dica do Mentor: Diferente do Java, a variável i continua existindo mesmo depois que o laço acaba, mas por boa prática, só a usamos dentro do for.

## 📉 Contagem Regressiva

Para contar de trás para frente, começamos com o número maior, vamos até o menor e usamos o passo -1.

```python
for i in range(10, 0, -1):
    print(f"Faltam {i} segundos...")
print("Decolar! 🚀")
```

## 🔠 Bônus: Percorrendo Textos

O for em Python é tão poderoso que pode percorrer até as letras de uma palavra:

```python
for letra in "PYTHON":
    print(letra)
# Vai imprimir P, depois Y, depois T... uma embaixo da outra.
```

Pronto para colocar o for para trabalhar? Vá para o arquivo exercicios.md!
