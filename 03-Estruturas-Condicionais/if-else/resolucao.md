# ✅ Gabarito: If, Elif e Else (Python)

Se você concluiu os exercícios, parabéns! Lidar com várias condições pode dar um nó na cabeça no começo, e o Python não perdoa se esquecermos o `:` ou a indentação, né?

Confira abaixo as sugestões de resolução.

---

## 🗳️ Resolução: Exercício 1 (votacao.py)

**Como resolvemos:**
Usamos a ordem lógica da idade, do menor para o maior, para o `elif` filtrar corretamente. E usamos o operador `or` do Python, que deixa a leitura super fácil.

```python
idade = 65 # Pode testar com 15, 17, 25, 75...

if idade < 16:
    print("Você não pode votar.")
elif idade < 18 or idade > 70:
    # Se a idade for menor que 18 OU maior que 70.
    print("Seu voto é opcional (facultativo).")
else:
    # Se chegou aqui, é porque tem 18 ou mais, e 70 ou menos.
    print("Seu voto é OBRIGATÓRIO.")
```

## 🌡️ Resolução: Exercício 2 (clima.py)

Como resolvemos:
Avaliamos os intervalos de temperatura.

```python
temperatura = 22.5

if temperatura < 15:
    print("Está frio! Leve um casaco.")
elif temperatura <= 25:
    # Se o Python chegou aqui, sabemos que a temperatura é 15 ou mais.
    # Então só precisamos testar se é até 25.
    print("Clima agradável! Uma camiseta está ótimo.")
else:
    print("Está calor! Não esqueça a água e o protetor solar.")
```

## 🚀 Resolução: Desafio (emprestimo.py)

Como resolvemos:
Para o empréstimo ser aprovado, o nome do cliente não pode estar sujo. Ou seja, nome_sujo precisa ser False. Podemos usar nome_sujo == False ou o elegante not nome_sujo.

```python
salario = 3000.00
nome_sujo = False

# Verifica: Salário é maior que 2500 E (and) nome_sujo é falso?
if salario > 2500 and nome_sujo == False:
    print("Parabéns! Empréstimo Aprovado!")
elif nome_sujo == True:
    # Podemos dar um feedback específico se o problema for o nome sujo
    print("Empréstimo Negado: Cliente possui restrições no Serasa.")
else:
    # Se o nome não está sujo, o problema só pode ser a renda baixa
    print("Empréstimo Negado: Renda mínima não atingida.")
```
