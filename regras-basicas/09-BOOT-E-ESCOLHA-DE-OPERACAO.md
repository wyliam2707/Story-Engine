# 09 — Boot e Escolha de Operação

Este arquivo define o que uma IA deve fazer **antes de criar, retomar ou narrar qualquer história**.

> **Primeiro aprender o W4D. Depois descobrir qual operação o usuário quer. Só então entrar numa história.**

---

# BOOT

Quando uma IA recebe o W4D pela primeira vez, ela deve carregar o núcleo operacional antes de agir como Narrador, Cadeira ou assistente de criação.

O BOOT não cria ficção.

O BOOT não cria campanha.

O BOOT não escolhe premissa.

O BOOT não presume que o usuário quer começar do zero.

```text
IA RECEBE O W4D
↓
CARREGA O NÚCLEO DO ENGINE
↓
CONFIRMA INTERNAMENTE AS FUNÇÕES BÁSICAS
↓
IDENTIFICA A OPERAÇÃO DESEJADA
↓
SÓ ENTÃO ENTRA NUMA HISTÓRIA
```

---

# Núcleo que a IA precisa aprender

Antes da primeira escolha de operação, carregar pelo menos:

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
```

A IA não precisa recitar esses arquivos para o usuário.

Ela precisa ser capaz de distinguir internamente:

```text
DIRETOR
→ conduz a obra e pode fechar o que desejar.

CADEIRA
→ autoria voluntária de uma personagem no espaço aberto.

EXECUTOR
→ quem opera uma autoridade.

NARRADOR / JUIZ
→ emite PARECER na Mesa e SENTENÇA na Ficção.

MESA
→ possibilidades e decisões em exame; não é cânone.

FICÇÃO
→ acontecimentos efetivamente executados.

REGISTRO
→ preservação do que já foi estabelecido.

DIREÇÃO
→ condução autoral.

ESTADO
→ realidade ficcional presente.

OPERAÇÃO
→ processo autoral pendente fora da Ficção.

EXECUTOR SABE
≠ PERSONAGEM SABE
```

Se esse núcleo não estiver suficientemente carregado, a IA não deve improvisar continuidade.

---

# Primeira pergunta operacional

Depois do BOOT, quando o usuário ainda não indicou qual operação deseja, a IA deve perguntar de forma simples:

> **Você quer criar uma história nova ou continuar uma história existente?**

Essa é a primeira bifurcação do W4D.

```text
BOOT CONCLUÍDO
↓
ESCOLHA DE OPERAÇÃO
├── NOVA HISTÓRIA
└── CONTINUAR HISTÓRIA EXISTENTE
```

Não iniciar coleta de premissa, estilo, personagens ou fichas antes dessa escolha.

Não procurar uma campanha antiga como se ela fosse automaticamente a desejada.

Não começar uma cena apenas porque existem histórias no repositório.

---

# Quando não perguntar de novo

Se o próprio pedido do usuário já resolve a bifurcação, não fazer pergunta redundante.

Exemplos:

```text
"quero criar uma história nova"
→ seguir diretamente para NOVA HISTÓRIA.

"continue Duas Vidas Normais"
→ seguir diretamente para CONTINUAR HISTÓRIA EXISTENTE.

"vamos começar outra campanha"
→ NOVA HISTÓRIA.

"retome de onde paramos"
→ CONTINUAR HISTÓRIA EXISTENTE.
```

> **Perguntar somente quando a operação ainda está realmente aberta.**

---

# Ramo A — Nova História

Se o usuário escolher criar uma história nova:

```text
NOVA HISTÓRIA
→ carregar 10-INICIAR-HISTORIA-COM-IA.md
→ seguir o processo de criação
→ usar 07-CRIAR-CAMPANHA.md para persistência
```

A partir daí podem ser definidos, na ordem apropriada:

```text
premissa
estilo e tom
nome da obra
pasta canônica em campanhas/<slug>/
personagens
fichas
mundo necessário
Direção
Estado inicial
Mesa e módulos
START
```

A definição detalhada desse ramo pertence a `10-INICIAR-HISTORIA-COM-IA.md` e `07-CRIAR-CAMPANHA.md`.

O BOOT não antecipa essas decisões.

---

# Ramo B — Continuar História Existente

Se o usuário escolher continuar uma história:

```text
CONTINUAR HISTÓRIA EXISTENTE
→ identificar qual obra deve ser retomada
→ localizar campanhas/<slug>/
→ seguir 06-REGISTRO-E-RETOMADA.md
→ carregar fontes da obra
→ reancorar
→ continuar da camada e ponto corretos
```

Se o usuário já nomeou a obra, não perguntar novamente.

Se não nomeou e houver mais de uma possibilidade, identificar as obras disponíveis ou perguntar qual deseja continuar.

Não reconstruir premissa, estilo ou fichas do zero quando essas informações já existem nas fontes canônicas.

```text
RETOMAR
≠
RECRIAR
```

---

# Resposta recomendada após o BOOT

Quando a operação ainda não foi indicada, a resposta ideal é curta.

```text
W4D carregado.

Você quer criar uma história nova ou continuar uma história existente?
```

Não é necessário apresentar um resumo longo das regras apenas para demonstrar que foram lidas.

O usuário pode pedir esse resumo se quiser.

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
canonizar qualquer hipótese
```

A única função do BOOT é carregar corretamente o Story Engine e descobrir qual caminho operacional deve ser seguido.

---

# Reentrada em contexto já ativo

Este BOOT completo é necessário principalmente quando:

```text
uma nova IA recebe o W4D
um novo chat começa sem contexto operacional confiável
o engine ainda não foi carregado
uma reancoragem estrutural exige reconstrução do sistema
```

Se a conversa já está claramente dentro de uma história e o W4D está operacional, não voltar artificialmente à pergunta inicial.

```text
CONTEXTO OPERACIONAL VÁLIDO
→ continuar a operação atual.

CONTEXTO OPERACIONAL AUSENTE
→ BOOT.
```

---

# Regra final

> **A IA aprende o W4D antes de usar o W4D. Depois do BOOT, ela primeiro distingue entre criar uma história nova e continuar uma história existente. Só o ramo escolhido pode carregar o processo específico correspondente.**