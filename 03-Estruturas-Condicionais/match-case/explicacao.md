# 💡 Escolhas Diretas: A Estrutura Match Case (O "Switch" do Python)

Você já sabe usar o `if` e `elif` para tomar decisões. Ele é ótimo para checar "maior que" ou "menor que". Mas e quando você tem um **menu de opções exatas**?

Imagine um menu de telefone: _"Digite 1 para Vendas, 2 para Suporte, 3 para Financeiro"_.
Fazer isso com vários `elif` ficaria gigante e repetitivo. Em outras linguagens, usamos o `switch`. No Python (a partir da versão 3.10), nós usamos o moderno **Match Case**!

O `match` age como um seletor. Ele pega uma variável e testa: "É o caso 1? É o caso 2?".

---

## ✍️ A Estrutura do Match Case

A sintaxe é super limpa. Usamos a palavra `match` seguida da variável, e depois os blocos `case` com a indentação (espaço) correta.

```python
opcao = 2

# O match "liga" a verificação na variável 'opcao'
match opcao:
    case 1:
        print("Você escolheu a Opção 1")
    case 2:
        print("Você escolheu a Opção 2")
    case _: # O underline (_) funciona como o 'default', roda se nenhum for verdadeiro
        print("Opção inválida!")
```

🎉 A Maior Vantagem do Python: Adeus, break!
Se você já estudou linguagens como Java ou C, deve lembrar que o switch exigia a palavra break no final de cada caso, senão ele executava tudo de uma vez (o famoso Efeito Cascata).

O Python é inteligente! Assim que ele encontra o case verdadeiro e roda o código dele, ele sai do match automaticamente. Você não precisa digitar break!

🧵 Funciona com Textos (Strings) também!
Assim como os números, podemos criar menus baseados em palavras ou letras.

```python
plano = "PREMIUM"

match plano:
    case "BASICO":
        print("Você tem 10GB de espaço.")
    case "PREMIUM":
        print("Você tem espaço ilimitado!")
    case _:
        print("Plano não reconhecido.")
```

## 💻 Exemplo Completo: Máquina de Café

Copie o código abaixo no seu arquivo, troque o número da variável botao_apertado e veja o que a máquina de café vai te servir!

```python
botao_apertado = 1

print("Preparando sua bebida...")

match botao_apertado:
    case 1:
        print("☕ Aqui está o seu Café Expresso!")
    case 2:
        print("🥛 Aqui está o seu Café com Leite!")
    case 3:
        print("🍫 Aqui está o seu Cappuccino!")
    case _:
        print("❌ Erro: Botão inexistente. Tente 1, 2 ou 3.")
```

Pronto para testar? Vá para o arquivo exercicios.md!
