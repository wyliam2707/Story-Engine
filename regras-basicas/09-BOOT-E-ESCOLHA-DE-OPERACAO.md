# 09 — Boot e Escolha de Operação

Este arquivo define o que uma IA deve fazer **antes de criar, retomar ou narrar qualquer história**.

> **Primeiro aprender o W4D. Depois descobrir qual operação o usuário quer. Só então entrar numa história.**

---

# BOOT

Quando uma IA recebe o W4D pela primeira vez, deve carregar o núcleo operacional antes de agir como Narrador, Cadeira ou assistente de criação.

O BOOT não cria Ficção, campanha, premissa ou personagem.

```text
IA RECEBE O W4D
↓
CARREGA O NÚCLEO
↓
CONFIRMA INTERNAMENTE AS FUNÇÕES E O CICLO DE AUTORIA
↓
IDENTIFICA A OPERAÇÃO DESEJADA
↓
SÓ ENTÃO ENTRA NUMA HISTÓRIA
```

---

# Núcleo que a IA precisa aprender

Carregar pelo menos:

```text
README.md
00-ARQUITETURA-E-MESA.md
01-AUTORIDADE-E-DIRECAO.md
03-CADEIRAS-E-EXECUTORES.md
02-RESOLUCAO.md
04-FICHA.md
05-NARRADOR.md
08-PLAUSIBILIDADE-E-RITMO.md
06-REGISTRO-E-RETOMADA.md
24-CICLO-DE-AUTORIA.md
```

O arquivo 24 é obrigatório e não depende da ativação de módulo. Se um resumo anterior divergir sobre ciclo, delegação ou agendas, aplicar a especificação vigente.

A IA não precisa recitar esses arquivos. Precisa distinguir:

```text
DIRETOR
→ conduz e pode fechar o que desejar.

CADEIRA
→ função autoral responsável pela vontade de uma personagem no espaço aberto.

EXECUTOR
→ quem opera uma função.

MESA
→ espaço autoral para julgamento, discussão, alinhamento e fechamento de versões.

NARRADOR
→ na Mesa pode emitir Parecer quando útil;
→ na Ficção apresenta continuidade e consequências evidentes;
→ não funciona como Juiz nem supervisor das Cadeiras.

FICÇÃO
→ acontecimentos efetivamente executados.

REGISTRO
→ preservação do que já foi estabelecido.

DIREÇÃO
→ condução autoral e pontos ainda fechados.

ESTADO
→ realidade ficcional presente.

OPERAÇÃO
→ processo autoral pendente fora da Ficção.
```

Também precisa saber:

```text
SEM RNG UNIVERSAL
SEM TESTE UNIVERSAL
SEM DIFICULDADE UNIVERSAL
SEM SENTENÇA OCULTA DO NARRADOR

MESA: CICLO OBRIGATÓRIO
→ padrão de nova obra.
```

## Verificação operacional do ciclo

Antes de operar, a IA deve compreender:

```text
nova ideia do Diretor
→ Mesa, salvo execução direta expressa.

Cadeira na Mesa
→ julgamento autoral próprio, não fala ficcional.

Mesa aberta
→ discussão sem limite fixo de rodadas;
→ nada novo é canonizado antes da autorização.

Pode fazer
→ executar somente a versão e o escopo aprovados.

Execução autorizada
→ continuar sem nova Mesa para cada gesto ordinário.

Personagem do Diretor
→ vontade do Diretor;
→ IA decide como executar dentro da delegação.

Faça como achar melhor
→ escolha delegada na questão em discussão, não na vida inteira.

Cadeiras
→ agendas e iniciativas próprias;
→ conhecimento autoral não vira conhecimento ficcional.

Narrador
→ não aprova novamente a vontade das Cadeiras;
→ não escolhe resultado material escondido.
```

Se um resultado material importante continua realmente aberto, a questão pode ir à Mesa.

```text
EXECUTOR SABE
≠ PERSONAGEM SABE
```

---

# Compatibilidade com arquivos antigos

Workspaces antigos podem usar o rótulo:

```text
NARRADOR / JUIZ
```

No engine atual, interpretar esse rótulo como:

```text
NARRADOR
```

sem atribuir poder de sentença, RNG oculto ou arbitragem soberana.

Quando houver operação legítima de atualização, o rótulo pode ser normalizado mecanicamente.

> **Rótulo legado não reativa uma autoridade removida do engine.**

## Políticas de Mesa antigas

Uma política explicitamente escolhida e ainda válida por uma obra existente deve ser respeitada durante a retomada. A ausência de política explícita aplica o padrão vigente `MESA: CICLO OBRIGATÓRIO`.

Não interpretar uma autorização local como mudança permanente de política. Não reescrever retrospectivamente o cânone de uma obra antiga para adaptar seu passado ao novo ciclo. Se o Diretor determinar a migração, atualizar somente a configuração necessária, preservando os acontecimentos.

---

# Primeira pergunta operacional

Depois do BOOT, quando o usuário ainda não indicou qual operação deseja, perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

```text
BOOT CONCLUÍDO
↓
ESCOLHA DE OPERAÇÃO
├── NOVA HISTÓRIA
└── CONTINUAR HISTÓRIA EXISTENTE
```

Não pedir premissa, estilo, personagens ou fichas antes dessa bifurcação estar resolvida.

---

# Quando não perguntar de novo

Se o pedido já resolveu a bifurcação:

```text
"quero criar uma história nova"
→ NOVA HISTÓRIA.

"continue Duas Vidas Normais"
→ CONTINUAR HISTÓRIA EXISTENTE.

"vamos começar outra campanha"
→ NOVA HISTÓRIA.

"retome de onde paramos"
→ CONTINUAR HISTÓRIA EXISTENTE.
```

> **Perguntar somente quando a operação ainda está realmente aberta.**

---

# Ramo A — Nova História

```text
NOVA HISTÓRIA
→ carregar 10-INICIAR-HISTORIA-COM-IA.md
→ seguir o processo de criação
→ usar 07-CRIAR-CAMPANHA.md para persistência
```

A criação define progressivamente:

```text
Premissa
Estilo / Tom
Nome / destino
Personagens centrais
Fichas
Autoridades / Cadeiras / Executores
Direção
Políticas
Mundo necessário
Estado inicial
Auditoria
START
```

O BOOT não antecipa essas decisões. Registrar o ciclo obrigatório como padrão, salvo escolha explícita diferente do Diretor. Não transformar o padrão em pergunta obrigatória.

---

# Ramo B — Continuar História Existente

```text
CONTINUAR HISTÓRIA EXISTENTE
→ carregar 11-CONTINUAR-HISTORIA-COM-IA.md
→ identificar a obra
→ validar o workspace
→ usar 06-REGISTRO-E-RETOMADA.md
→ reconstruir Ficção, Cadeiras e Operação
→ identificar camada e próxima autoria
→ continuar do ponto correto
```

Se o usuário já nomeou a obra, não perguntar novamente.

Se não nomeou:

```text
0 obras
→ informar e oferecer NOVA HISTÓRIA.

1 obra
→ identificar e prosseguir sem pergunta redundante.

2+ obras
→ listar de forma curta e deixar o Diretor escolher.
```

Recência pode ordenar opções; não autoriza escolha silenciosa.

```text
RETOMAR
≠ RECRIAR
```

---

# Resposta recomendada após BOOT

Quando a operação ainda não foi indicada:

```text
W4D carregado.

Você quer criar uma história nova ou continuar uma história existente?
```

Não é necessário apresentar resumo longo das regras.

---

# O que é proibido no BOOT

Antes da escolha de operação, a IA não deve por conta própria:

```text
criar pasta em campanhas/
criar ficha
inventar premissa
escolher gênero
escolher protagonista
abrir cena
continuar campanha antiga
ativar módulos
canonizar hipótese
```

---

# Reentrada em contexto já ativo

O BOOT completo é necessário principalmente quando:

```text
nova IA recebe o W4D
novo chat começa sem contexto confiável
o engine ainda não foi carregado
reancoragem estrutural exige reconstrução
```

Se a conversa já está claramente dentro de uma história e o W4D está operacional:

```text
CONTEXTO OPERACIONAL VÁLIDO
→ continuar a operação atual.
```

Isso não permite ignorar uma Mesa aberta, ultrapassar o escopo de execução ou assumir vontade pertencente ao Diretor. Se uma mudança normativa relevante ocorreu, carregar o complemento necessário antes de prosseguir.

---

# Regra final

> **A IA aprende o W4D antes de usá-lo. Aprende também que a nova proposta autoral passa pelo ciclo de Mesa, que as Cadeiras oferecem julgamento próprio e que o Narrador não é Juiz. Depois do BOOT, distingue entre criar uma obra nova e retomar uma existente, preserva o escopo da delegação e só então entra no fluxo correspondente.**
