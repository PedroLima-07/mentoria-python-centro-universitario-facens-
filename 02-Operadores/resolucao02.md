# ✅ Gabarito: Módulo 02 - Operadores (Python)

Se você chegou até aqui, muito bem! Os operadores exigem um pouco mais de atenção lógica, especialmente quando começamos a misturar matemática com decisões de "Verdadeiro ou Falso".

Lembre-se: não existe apenas um jeito certo de escrever código. Se as suas variáveis têm nomes diferentes ou se você fez o cálculo em uma ordem ligeiramente diferente, mas chegou ao mesmo resultado, **você acertou!**

Abaixo estão as soluções sugeridas em Python.

---

## 🥖 Resolução: Exercício 1 (padaria.py)

**O objetivo:** Calcular o valor total da compra de cafés e pão de queijo, e depois calcular o troco com base na nota de R$ 50 entregue.

**Como resolvemos:**

```python
# 1. Criando as variáveis para os preços e quantidades
preco_cafe = 5.50
quantidade_cafe = 3

preco_pao_de_queijo = 12.00
quantidade_pao_de_queijo = 1

dinheiro_entregue = 50.00

# 2. Calculando o total
# Multiplicamos o preço pela quantidade e somamos tudo
total_compra = (preco_cafe * quantidade_cafe) + (preco_pao_de_queijo * quantidade_pao_de_queijo)

# 3. Calculando o troco
troco = dinheiro_entregue - total_compra

# 4. Mostrando o resultado
print("--- Cupom Fiscal ---")
print(f"Valor Total: R$ {total_compra}")
print(f"Valor Entregue: R$ {dinheiro_entregue}")
print(f"Troco a devolver: R$ {troco}")
```

## 🎓 Resolução: Exercício 2 (escola.py)

O objetivo: Usar operadores relacionais e lógicos para descobrir se o aluno passou, lembrando que ele precisa de nota e de presença.

Como resolvemos:

```python
# 1. Dados do aluno
nota1 = 8.5
nota2 = 5.5
frequencia = 80 # 80%

# 2. Calculando a média
# Os parênteses são OBRIGATÓRIOS aqui! O Python faz a divisão antes da soma se você não colocar.
media = (nota1 + nota2) / 2

# 3. Verificando a aprovação
# Ele precisa da média >= 7.0 "E" (and) da frequência >= 75
aprovado = (media >= 7.0) and (frequencia >= 75)

# 4. Exibindo os resultados
print("--- Boletim do Aluno ---")
print(f"Média final: {media}")
print(f"Frequência: {frequencia}%")

# O resultado será False, porque a média (7.0) é atingida, mas se a nota fosse menor, ele reprovaria.
# Como a nota1 e nota2 dão exatamente média 7.0, a resposta será True!
print(f"Aluno aprovado? {aprovado}")
```

## 🚀 Resolução: Desafio (balada.py)

O objetivo: Usar o operador de resto (%) para saber se um número é par e combinar isso com um ingresso VIP.

Como resolvemos:

```python
# 1. Dados do cliente
idade = 24
pagou_vip = True

# 2. A mágica do número par
# Se pegarmos a idade (24) e dividirmos por 2, sobra alguma coisa?
# Não! O resto é 0. Então a comparação (0 == 0) dá True.
idade_par = (idade % 2) == 0

# 3. A regra de entrada
# Só entra se a idade for par E se tiver pagado o VIP
pode_entrar = idade_par and pagou_vip

# 4. Exibindo o resultado
print("--- Controle de Entrada VIP ---")
print(f"Idade do cliente: {idade}")
print(f"Tem ingresso VIP? {pagou_vip}")
print(f"Acesso Liberado? {pode_entrar}")
```
