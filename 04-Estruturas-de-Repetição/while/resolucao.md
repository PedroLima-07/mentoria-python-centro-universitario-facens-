# ✅ Gabarito: Laços While (Python)

Se você conseguiu fazer os exercícios sem criar um loop infinito que travou a sua máquina, você já é um vencedor! 😂

O `while` exige muita atenção lógica. Confira abaixo como resolvemos os exercícios, misturando o estilo clássico e o estilo interativo.

---

## 💰 Resolução: Exercício 1 (poupanca.py)

**Como resolvemos (While Clássico):**
Aqui o `while` normal brilha! Nós não sabíamos quantos meses iam demorar, então deixamos o Python calcular isso repetindo o laço até a condição ser atingida.

```python
saldo = 0.0
meta = 3000.0
meses = 0

print("Iniciando o projeto Videogame Novo!")

# Enquanto não atingir a meta, continue guardando
while saldo < meta:
    saldo += 450.0  # Guarda o dinheiro do mês
    meses += 1      # Conta que se passou um mês
    print(f"Mês {meses}: Saldo atual R$ {saldo}")

print("\n--- Parabéns! ---")
print(f"Você atingiu a meta em {meses} meses.")
print(f"Saldo final: R$ {saldo}")
```

## 🎲 Resolução: Exercício 2 (adivinhacao.py)

Como resolvemos (While True):
Como queríamos que o programa perguntasse o palpite pelo menos uma vez, o while True foi a melhor escolha. O break só é ativado no momento da vitória.

```python
numero_secreto = 7

print("Bem-vindo ao Jogo de Adivinhação!")
print("Pensei em um número de 1 a 10. Tente adivinhar!")

while True:
    palpite = int(input("Qual é o seu palpite? "))

    if palpite == numero_secreto:
        print("🎉 Parabéns! Você acertou na mosca!")
        break # O jogo acaba aqui!
    elif palpite < numero_secreto:
        print("Errado! Tente um número MAIOR. ⬆️")
    elif palpite > numero_secreto:
        print("Errado! Tente um número MENOR. ⬇️")
```

## 🍕 Resolução: Desafio (lanchonete.py)

Como resolvemos:
Usamos a mesma lógica do loop infinito combinada com o moderno match case (poderia ser if/elif também) para montar um sistema de caixa registradora.

```python
total_conta = 0.0

print("Bem-vindo à Lanchonete Dev!")

while True:
    print("\n--- Cardápio ---")
    print("1. Hamburguer - R$ 20.00")
    print("2. Refrigerante - R$ 5.00")
    print("0. Finalizar Pedido")

    escolha = int(input("O que deseja adicionar ao pedido? "))

    match escolha:
        case 1:
            total_conta += 20.00
            print("🍔 Hamburguer adicionado!")
        case 2:
            total_conta += 5.00
            print("🥤 Refrigerante adicionado!")
        case 0:
            print("Preparando sua conta...")
            break # Cliente escolheu fechar a conta, saímos do loop!
        case _:
            print("Opção inválida! Digite 1, 2 ou 0.")

print("\n=========================")
print(f"Total a pagar: R$ {total_conta}")
print("Bom apetite!")
```
