# 🔄 Estrutura While: O Clássico e o Infinito

Se no módulo do `for` nós sabíamos exatamente quantas vezes o código ia repetir (ex: contar de 1 até 10), aqui nós entramos no mundo da incerteza.

Imagine um jogo de videogame: você não sabe quantos passos o jogador vai dar, não sabe quantas vezes ele vai pular, mas sabe que o jogo deve continuar **enquanto** o personagem estiver vivo. Para resolver problemas onde não sabemos o número exato de repetições, usamos a estrutura **`while`** (que significa "enquanto").

Neste material, vamos destrinchar as duas formas de usar o `while` no Python: o estilo clássico e o estilo infinito (muito usado para menus).

---

## 🚦 1. O While Clássico (Pergunta primeiro, faz depois)

A lógica do `while` normal é muito parecida com a de um porteiro de balada super rigoroso. Ele funciona no seguinte passo a passo:

1. O Python avalia a condição (A variável é maior que zero? A senha está errada?).
2. Se a resposta for **Verdadeira (`True`)**, ele entra no bloco e executa todo o código indentado (com espaço).
3. Quando chega na última linha do bloco, ele **volta automaticamente para o topo** e faz a pergunta de novo.
4. Ele só para de repetir quando a condição virar **Falsa (`False`)**. Aí ele pula o bloco e segue a vida.

### A Anatomia do While Clássico

```python
fatias_pizza = 8

# A condição é: "Fatias de pizza é maior que zero?"
while fatias_pizza > 0:
    print(f"Comi uma fatia! Restam {fatias_pizza}")

    # 🚨 PASSO CRÍTICO: Atualizar a variável!
    # Se nós não diminuirmos a fatia, a condição sempre será Verdadeira.
    fatias_pizza -= 1

# Quando fatias_pizza chegar a 0, o Python ignora o while e vem direto para cá:
print("Acabou a pizza!")
```

## ⚠️ O Perigo Oculto: O Loop Infinito!

O maior erro de todo programador iniciante é criar um loop infinito. Se você esquecer de atualizar a variável que está sendo testada na condição do while (como esquecer o fatias_pizza -= 1 no exemplo acima), a condição será verdadeira para sempre.
O seu programa vai rodar infinitamente até travar o computador! Se isso acontecer com você, clique no terminal e aperte Ctrl + C para forçar a parada.

## 🔄 2. O "Do-While" do Python (Faz primeiro, pergunta depois)

Em linguagens como Java ou C, existe um comando chamado do-while, que garante que o código rode pelo menos uma vez antes de testar a condição.

O Python NÃO tem esse comando! Mas nós, programadores Python, simulamos isso usando um Loop Infinito Proposital (while True:) combinado com o botão de emergência: o comando break.

Isso é perfeito para criar Menus Interativos, onde queremos mostrar as opções na tela pelo menos a primeira vez, ler o que o usuário digitou, e só depois decidir se o programa fecha ou repete.

Como o while True funciona?
A palavra True significa Verdadeiro. Como "Verdadeiro é sempre Verdadeiro", esse laço nunca vai terminar sozinho. A única forma de escapar dele é usando o comando break (quebrar). Assim que o Python lê a palavra break, ele destrói o laço na hora e pula para fora.

```python
# O 'True' com T maiúsculo cria o laço infinito
while True:
    print("\n--- MENU DE CAIXA ELETRÔNICO ---")
    print("1. Ver Saldo")
    print("2. Depositar")
    print("0. Sair")

    # Lemos o teclado e convertemos para número inteiro (int)
    opcao = int(input("Escolha uma opção: "))

    if opcao == 1:
        print("Seu saldo é R$ 100,00.")
    elif opcao == 2:
        print("Por favor, insira as notas na máquina.")
    elif opcao == 0:
        print("Devolvendo o cartão. Saindo do sistema...")
        # O 'break' é o nosso salvador! Ele quebra o laço e o programa acaba.
        break
    else:
        print("Opção inválida. Tente novamente.")
```

## 🎁 Bônus Mestre Jedi: O comando continue

Já conhecemos o break (que destrói o laço e vai embora). Mas existe um "irmão" dele chamado continue.

Enquanto o break encerra tudo, o continue apenas aborta a volta atual e pula direto para o topo do laço de novo, ignorando tudo o que estiver abaixo dele.

Veja como é útil para pular números indesejados:

```python
contador = 0

while contador < 5:
    contador += 1

    if contador == 3:
        print("Opa, o 3 eu não quero imprimir. Pulando!")
        continue # O Python ignora o print de baixo e volta pro 'while contador < 5'

    print(f"Número atual: {contador}")

# Resultado no terminal: 1, 2, (mensagem pulando), 4, 5.
```

## 🧠 Resumo da Ópera

Use o while com condição (ex: while saldo < 1000:) quando a repetição depende de um cálculo ir mudando aos poucos.

Use o while True: com break quando precisar de um menu interativo que leia o teclado do usuário ou precise rodar obrigatoriamente uma vez.

Cuidado com loops infinitos sem querer! Sempre verifique se a sua variável está sendo atualizada.

Pronto para testar os dois estilos? Vá para o arquivo exercicios.md!
