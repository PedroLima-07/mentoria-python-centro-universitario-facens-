# ✅ Gabarito: Match Case (Python)

Se você chegou até aqui, muito bem! O `match case` é super gostoso de usar quando entendemos a lógica de "selecionar uma gaveta". E como o Python não precisa de `break`, o código fica incrivelmente limpo.

Confira abaixo as sugestões de resolução:

---

## 📅 Resolução: Exercício 1 (dia_da_semana.py)

**Como resolvemos:**
Usamos os números de 1 a 7 como os blocos `case`. O `case _:` garante que o programa saiba o que responder se alguém digitar 8 ou 0.

```python
dia = 3

match dia:
    case 1:
        print("Domingo")
    case 2:
        print("Segunda-feira")
    case 3:
        print("Terça-feira")
    case 4:
        print("Quarta-feira")
    case 5:
        print("Quinta-feira")
    case 6:
        print("Sexta-feira")
    case 7:
        print("Sábado")
    case _:
        print("Erro: Dia inválido! Digite um número de 1 a 7.")
```

## 🎧 Resolução: Exercício 2 (atendimento.py)

Como resolvemos:
Bem parecido com o primeiro, simulando a navegação de um menu de telefone real.

```python
opcao_escolhida = 2

print("Bem-vindo ao Atendimento da NetLink!")

match opcao_escolhida:
    case 1:
        print("Encaminhando para o Suporte Técnico. Tempo de espera: 2 minutos.")
    case 2:
        print("Sua 2ª via do boleto foi enviada para o seu e-mail cadastrado.")
    case 3:
        print("Redirecionando para o setor de Vendas e Planos...")
    case 4:
        print("Poxa, que pena que deseja cancelar. Transferindo para o setor de Retenção.")
    case _:
        print("Opção inválida. Por favor, desligue e ligue novamente.")
```

## 🚀 Resolução: Desafio (calculadora.py)

Como resolvemos:
Aqui está o poder do match trabalhando com Strings! E veja como as f-strings deixam a impressão do resultado muito mais bonita.

```python
num1 = 20.0
num2 = 4.0

# Troque o sinal aqui para testar as outras operações (+, -, *, /)
operacao = "/"

print(f"Calculando: {num1} {operacao} {num2}")

match operacao:
    case "+":
        print(f"Resultado: {num1 + num2}")
    case "-":
        print(f"Resultado: {num1 - num2}")
    case "*":
        print(f"Resultado: {num1 * num2}")
    case "/":
        print(f"Resultado: {num1 / num2}")
    case _:
        print("Operação inválida. Use apenas +, -, * ou /.")
```
