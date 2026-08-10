# Dados de Destino

## Regra Básica

Toda ação incerta utiliza **4 Dados de Destino**.

Cada Dado de Destino possui três resultados possíveis:

| Face | Valor |
|---|---:|
| `−` | −1 |
| Neutro | 0 |
| `+` | +1 |

Os resultados dos quatro dados são somados. Dessa forma, o **Destino** pode variar naturalmente de **−4 a +4**.

### Usando dados Fate/Fudge

Dados Fate/Fudge já possuem as faces negativas, neutras e positivas necessárias para a rolagem.

### Usando dados comuns de seis faces (D6)

Quando forem utilizados D6 comuns, converta cada resultado da seguinte forma:

| D6 | Destino |
|---:|---:|
| 1–2 | −1 |
| 3–4 | 0 |
| 5–6 | +1 |

## Exemplo

Uma rolagem apresenta os seguintes resultados:

`+1, +1, 0, −1`

Somando os quatro dados:

`+1 +1 +0 −1 = +1`

O **Destino é +1**.

## Sorte e Azar

Sorte e Azar modificam a quantidade de Dados de Destino rolados, mas o resultado final continua sendo formado por **quatro dados**.

### Sorte

Cada nível de **Sorte** adiciona um dado à mão. Depois da rolagem, conservam-se os **quatro melhores resultados**.

- Normal: role 4 dados e mantenha os 4.
- Sorte [1]: role 5 dados e mantenha os 4 melhores.
- Sorte [2]: role 6 dados e mantenha os 4 melhores.

### Azar

Cada nível de **Azar** adiciona um dado à mão. Depois da rolagem, conservam-se os **quatro piores resultados**.

- Azar [1]: role 5 dados e mantenha os 4 piores.
- Azar [2]: role 6 dados e mantenha os 4 piores.

### Fontes de Sorte

Qualquer regra, Perícia, Poder, item ou circunstância que conceda Sorte utiliza esta mesma mecânica.

Perícias, quando aplicáveis, concedem Sorte conforme seu grau:

- Perícia [0] = Sorte [0];
- Perícia [1] = Sorte [1];
- Perícia [2] = Sorte [2].

Perícia não cria um tipo separado de Dado de Destino.

### Cancelamento e Limite

Todas as fontes de **Sorte** e **Azar** são somadas antes da rolagem. Esses valores acumulados podem ultrapassar [2] apenas para fins de **cancelamento**.

Sorte e Azar se anulam na proporção de **1 para 1**.

Exemplos:

- Sorte [2] + Azar [1] = **Sorte [1]**;
- Sorte acumulada [4] + Azar acumulado [3] = **Sorte [1]**;
- Sorte acumulada [4] + Azar acumulado [1] = Sorte restante [3], mas para a rolagem é tratada como **Sorte [2]**.

Somente depois do cancelamento aplica-se o limite da rolagem: o valor efetivamente utilizado nunca ultrapassa **Sorte [2]** ou **Azar [2]**.

Portanto, mesmo quando existirem fontes acumuladas acima de [2], a mão de Dados de Destino possui máximo absoluto de **6 dados**.

## Estado da Regra

Esta é a regra-base atualmente adotada para os Dados de Destino. Sua interação detalhada com o Patamar e outras mecânicas será definida conforme o desenvolvimento do sistema avançar.
