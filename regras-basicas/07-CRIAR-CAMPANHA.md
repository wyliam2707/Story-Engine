# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico atual do espaço persistente de uma obra.

Este arquivo define **como materializar e completar o workspace persistente** de uma nova história.

Para uma IA começando do zero, ele não substitui `10-INICIAR-HISTORIA-COM-IA.md`.

> **Primeiro construir a identidade da obra. Depois criar seu destino. Só então completar as fontes necessárias.**

---

# Condição para criar a pasta

No ramo `NOVA HISTÓRIA`, a pasta não nasce no BOOT, na Premissa ou durante Estilo/Tom.

Antes de criar:

```text
PREMISSA → APROVADA
ESTILO / TOM → APROVADO
NOME → APROVADO ou provisório autorizado
SLUG → definido e sem conflito
```

Seguir `14-CRIACAO-NOME-E-DESTINO.md`.

Só então criar:

```text
campanhas/<slug>/README.md
```

---

# README âncora

No nascimento do workspace, registrar somente decisões já aprovadas:

```text
# [NOME]

STATUS
→ EM PREPARAÇÃO

## Proposta curta
[Premissa aprovada.]

## Estilo / Tom
[Resumo aprovado.]
```

Não preencher antecipadamente:

```text
Personagens ainda não aprovadas
Cadeiras ainda não definidas
Personagem do Diretor ainda não escolhido
módulos ainda não discutidos
Estado inicial ainda não construído
mundo ainda aberto
```

> **O README nasce como âncora; cresce conforme a preparação produz decisões legítimas.**

---

# Persistência progressiva

Depois que o workspace existe:

```text
material aprovado
→ salvar na fonte canônica correta.
```

Exemplos:

```text
Personagens centrais aprovadas
→ README.md

ficha aprovada
→ personagens/<nome>.md

Autoridades aprovadas
→ README.md

Direção suficiente
→ direcao.md

ponto inicial definido
→ estado.md

fato externo estável necessário
→ mundo/

Mesa/Auditoria/criação pendente
→ operacao.md
```

Não criar arquivo vazio ou inventado para completar árvore ideal.

```text
DESTINO CRIADO
≠ PREPARAÇÃO CONCLUÍDA
≠ START
```

---

# Estrutura esperada quando necessária

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
├── personagens/
├── operacao.md             # somente quando houver operação transitória real
├── mundo/                  # somente quando necessário
├── arco.md                 # somente com Arco Preparado ativo
├── oposicao.md             # somente com Opositor ativo
└── livro/                  # somente com Livro ativo
```

A ausência de fonte opcional não é erro.

A ausência de fonte necessária no START é problema de preparação.

---

# Passo 1 — Personagens centrais

Depois de Nome/Destino, seguir:

```text
15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

Registrar no README apenas o núcleo curto aprovado.

```text
README
→ quem está no centro da obra.

FICHA
→ quem cada pessoa é.
```

---

# Passo 2 — Fichas

Seguir:

```text
16-CRIACAO-FICHAS.md
04-FICHA.md
modelos/FICHA.md
```

Construir preferencialmente uma personagem por vez.

Destino:

```text
campanhas/<slug>/personagens/<slug-da-personagem>.md
```

```text
FICHA SUFICIENTE
≠ FICHA EXAUSTIVA
```

Não criar trauma, segredo, fraqueza, poder, equipamento ou drama apenas para preencher modelo.

Se a criação ainda não aprovada precisar persistir:

```text
operacao.md
→ preserva a etapa pendente.
```

---

# Passo 3 — Autoridades, Cadeiras e Executores

Depois das fichas iniciais suficientes, seguir:

```text
17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
03-CADEIRAS-E-EXECUTORES.md
```

Ordem:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Registrar no README, conforme aprovado:

```text
DIRETOR
NARRADOR / JUIZ
PERSONAGEM DO DIRETOR, quando houver
CADEIRAS INICIAIS
EXECUTOR DE CADA AUTORIDADE
limites de delegação, quando existirem
```

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

---

# Passo 4 — Direção

Depois das Autoridades iniciais, seguir:

```text
18-CRIACAO-DIRECAO.md
01-AUTORIDADE-E-DIRECAO.md
modelos/DIRECAO.md
```

A Direção inicial não exige planejamento do futuro.

Ela consolida somente:

```text
Premissa aprovada
Estilo / Tom aprovado
fatos estruturais já fechados
decisões persistentes realmente tomadas, se houver
decisões locais ainda ativas, se houver
```

Se o Diretor não decidiu trajetórias futuras:

```text
Direções Persistentes
→ nenhuma além das premissas já estabelecidas.

Direções Ativas
→ nenhuma.

Espaço Aberto
→ o desenvolvimento permanece aberto fora do que foi explicitamente fechado.
```

Isso é suficiente para o início.

> **Direção não é plano obrigatório. É memória do que ainda governa a obra.**

Não exigir:

```text
final
arco completo
revelações futuras
marcos de romance
estrutura de capítulos
```

apenas para considerar `direcao.md` válido.

A Direção pode crescer enquanto a história é escrita.

---

# Passo 5 — Políticas operacionais

Registrar no `README.md` quando necessário:

```text
POLÍTICA DE MESA
POLÍTICA DE INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

## Política de Mesa

Conforme `00-ARQUITETURA-E-MESA.md`:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Padrão:

```text
MESA: SOB DEMANDA
```

## Indicador operacional

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

Padrão:

```text
SILENCIOSO
```

---

# Passo 6 — Mundo necessário

Criar `mundo/` somente quando fatos externos estáveis precisam persistir para a abertura ou continuidade.

Não construir enciclopédia por obrigação.

Detalhes neutros podem surgir por criação emergente conforme `02-RESOLUCAO.md`.

---

# Passo 7 — Mesa inicial, quando necessária

Durante a preparação:

```text
DIRETOR PROPÕE
→ CADEIRAS ENVOLVIDAS OPINAM
→ NARRADOR EMITE PARECER
→ DIRETOR AJUSTA, CANCELA OU CONFIRMA
```

Nada discutido vira Ficção apenas porque houve concordância.

Se precisar sobreviver a uma pausa:

```text
operacao.md
```

---

# Passo 8 — Estado inicial

Criar `estado.md` apenas quando o ponto inicial da Ficção estiver definido.

Usar `modelos/ESTADO.md`.

Registrar, quando pertinente:

```text
momento
local
presenças
condições relevantes
intenções persistentes já existentes
processos e prazos
último fato estabelecido
primeiro ponto aberto
```

Antes do início:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

Não colocar hipótese de Mesa ou futuro desejado no Estado.

---

# Passo 9 — Módulos opcionais

Ativar somente o que a obra realmente usa:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

Módulo inativo não produz arquivo nem comportamento por hábito.

---

# Passo 10 — Auditoria de início

Antes da Ficção, confirmar:

```text
[ ] nome e slug definidos;
[ ] README.md existe;
[ ] Premissa e Estilo/Tom estão preservados;
[ ] Personagens centrais necessárias estão aprovadas;
[ ] fichas necessárias são reconstruíveis;
[ ] Diretor e Narrador/Juiz estão definidos;
[ ] Cadeiras e executores necessários estão definidos;
[ ] Personagem do Diretor está corretamente atribuída, se houver;
[ ] delegações não transferiram vontade por acidente;
[ ] direcao.md preserva o que foi decidido e deixa o restante aberto;
[ ] política de Mesa está definida ou usa SOB DEMANDA;
[ ] indicador está definido ou usa SILENCIOSO;
[ ] estado.md possui último fato e primeiro ponto aberto;
[ ] hipóteses não foram registradas como fatos;
[ ] operacao.md existe somente se houver operação real pendente;
[ ] módulos ativos possuem função real;
```

Quando suficiente:

```text
STATUS
→ PRONTA
```

---

# START

Depois da preparação:

```text
START
→ reancorar o mínimo necessário
→ reconstruir pacotes separados das Cadeiras
→ restaurar operação pendente, se houver
→ caso contrário identificar o primeiro ponto aberto
→ identificar quem possui a próxima autoria
→ iniciar a camada correta
```

Uma Cadeira IA disponível pode tomar a primeira iniciativa se o espaço aberto permitir.

Não existe obrigação de começar por ação, conflito ou perigo.

---

# Regra final

> **A pasta nasce quando Nome e Destino estão definidos. Depois, o W4D identifica quem sustenta a obra, constrói cada pessoa, configura autoria e execução, preserva apenas a Direção realmente decidida e deixa o futuro aberto quando o Diretor prefere descobri-lo escrevendo. START inicia a Ficção; a preparação não precisa prever a história inteira.**