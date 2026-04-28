# 🏋️‍♂️ Exercícios: Dominando o If, Elif e Else

Chegou a hora de treinar a sua lógica no padrão Python! Crie os arquivos `.py` para cada um dos desafios abaixo. Lembre-se sempre de alinhar o código direitinho com a tecla _Tab_!

---

### 🗳️ Exercício 1: O Sistema de Votação

**Arquivo:** `votacao.py`

**Cenário:** No Brasil, as regras para votação baseadas na idade são:

- Menores de 16 anos: Não podem votar.
- Entre 16 e 17 anos, ou acima de 70 anos: Voto opcional (facultativo).
- Entre 18 e 70 anos: Voto obrigatório.

**O que você deve fazer:**

1. Crie uma variável `idade`.
2. Crie uma estrutura de `if / elif / else` para classificar o tipo de voto da pessoa.
3. Imprima no console o resultado (Ex: "Voto obrigatório").

---

### 🌡️ Exercício 2: O Conselheiro do Clima

**Arquivo:** `clima.py`

**Cenário:** Você vai criar um pequeno assistente que diz o que a pessoa deve vestir baseado na temperatura do dia.

- Temperatura abaixo de 15 graus: "Está frio! Leve um casaco."
- Temperatura entre 15 e 25 graus: "Clima agradável! Uma camiseta está ótimo."
- Temperatura acima de 25 graus: "Está calor! Não esqueça a água e o protetor solar."

**O que você deve fazer:**

1. Crie uma variável `temperatura`.
2. Avalie essa temperatura usando o `if`, `elif` e `else`, e imprima o conselho correto.

---

### 🚀 Desafio: O Gerente do Banco

**Arquivo:** `emprestimo.py`

**Cenário:** Um cliente quer fazer um empréstimo. O sistema do banco só aprova se duas regras forem seguidas ao mesmo tempo:

1. O salário do cliente precisa ser maior que R$ 2.500,00.
2. O cliente NÃO pode ter o nome sujo no Serasa.

**O que você deve fazer:**

1. Crie uma variável `salario` e uma variável booleana `nome_sujo` (lembre-se: `True` significa que o nome está sujo).
2. Se ele atender a todas as regras (salário alto `and` `not` nome_sujo), imprima "Empréstimo Aprovado!".
3. Se ele não atender a alguma regra, imprima "Empréstimo Negado." e tente explicar o porquê (usando um `elif` se quiser ir além!).
