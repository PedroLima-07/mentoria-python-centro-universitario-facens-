# 🏋️‍♂️ Exercícios: Operadores em Ação (Python)

Chegou a hora de colocar a mão na massa! Crie os arquivos `.py` no seu VS Code para resolver cada um dos problemas abaixo. Lembre-se: errar faz parte do processo, então não tenha medo de testar!

---

### 🥖 Exercício 1: A Padaria (Operadores Aritméticos)

**Arquivo:** `padaria.py`

**Cenário:** Você foi contratado para fazer o sistema de caixa de uma padaria. O cliente João comprou:

- 3 cafés (R$ 5.50 cada)
- 1 pão de queijo (R$ 12.00)

O João entregou uma nota de R$ 50.00 para pagar a conta.

**O que você deve fazer:**

1. Crie variáveis para armazenar o valor dos produtos e a quantidade.
2. Calcule o valor **total** da compra.
3. Calcule o **troco** que o João deve receber.
4. Imprima no console o valor total e o troco usando f-strings.

---

### 🎓 Exercício 2: O Sistema Escolar (Operadores Relacionais e Lógicos)

**Arquivo:** `escola.py`

**Cenário:** Uma escola precisa de um sistema que verifique automaticamente se um aluno foi aprovado ou reprovado.
As regras para aprovação são rigorosas: O aluno precisa ter uma **média maior ou igual a 7.0** E uma **frequência maior ou igual a 75%**.

**Dados do aluno:**

- Nota 1: 8.5
- Nota 2: 5.5
- Frequência: 80 (ou seja, 80%)

**O que você deve fazer:**

1. Crie as variáveis para as notas e calcule a média (soma das notas dividida por 2).
2. Crie a variável para a frequência.
3. Crie uma variável `aprovado` que use os operadores `and` e `>=` para verificar se o aluno passou.
4. Imprima no console a média do aluno e se ele foi aprovado (`True` ou `False`).

> 💡 **Dica:** Na hora de calcular a média, lembre-se de usar parênteses para somar as notas antes de dividir! Ex: `(nota1 + nota2) / 2`.

---

### 🚀 Desafio: O Guardião da Balada (O temido Módulo `%`)

**Arquivo:** `balada.py`

**Cenário:** Você está criando o sistema de entrada de uma balada muito exclusiva. Hoje é a "Noite dos Pares". Só podem entrar pessoas cuja idade seja um **número par** e que **tenham pagado o ingresso VIP**.

**Dados do cliente:**

- Idade: 24
- Pagou VIP: `True`

**O que você deve fazer:**

1. Crie as variáveis de idade e do ingresso VIP.
2. Descubra se a idade é par. _(Como? Lembra do operador de resto `%`? Se o resto da divisão da idade por 2 for IGUAL a 0, significa que é par!)_.
3. Verifique se ele pode entrar (Idade par E VIP).
4. Imprima o resultado (`True` ou `False`).

> 💡 **Dica do Mentor:** Para comparar se o resto da divisão é igual a zero, usamos DOIS sinais de igual: `(idade % 2) == 0`.
