# 🏋️‍♂️ Exercícios: Dominando o Match Case

Agora é a sua vez de criar os seus próprios menus e seletores usando a estrutura moderna do Python. Crie os arquivos `.py` e mãos à obra!

---

### 📅 Exercício 1: Dias da Semana

**Arquivo:** `dia_da_semana.py`

**Cenário:** Precisamos de um conversor que transforme um número no dia da semana correspondente.

- 1 = Domingo
- 2 = Segunda-feira
  ...
- 7 = Sábado.

**O que você deve fazer:**

1. Crie uma variável `dia`.
2. Use o `match` para imprimir o nome do dia correto baseado no número.
3. Se o número for menor que 1 ou maior que 7, o `case _:` (default) deve imprimir "Dia inválido!".

---

### 🎧 Exercício 2: Atendimento Eletrônico (URA)

**Arquivo:** `atendimento.py`

**Cenário:** Você foi contratado para programar o robô de atendimento de uma operadora de internet. As opções são:

- 1 - Falar com o Suporte Técnico
- 2 - Pedir 2ª via do Boleto
- 3 - Alterar Plano
- 4 - Cancelar Serviço

**O que você deve fazer:**

1. Crie a variável para receber a opção do cliente.
2. Crie os `case` imprimindo mensagens amigáveis (Ex: "Aguarde, estamos transferindo para o Suporte...").
3. Não esqueça do caso curinga (`case _:`) para opções que não existem.

---

### 🚀 Desafio: A Calculadora Básica

**Arquivo:** `calculadora.py`

**Cenário:** Vamos construir a lógica de uma calculadora que aceita o sinal da operação matemática como texto (String).

**O que você deve fazer:**

1. Crie duas variáveis para os números (ex: `num1 = 10.0` e `num2 = 5.0`).
2. Crie uma variável `operacao = "+"` (teste depois com "-", "\*", "/").
3. Faça um `match` testando a variável `operacao`.
4. Em cada `case`, faça o cálculo correto e imprima o resultado. (Exemplo no `case "+":`, imprima a soma de `num1` e `num2`).
