# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico atual do espaço persistente de uma obra.

Este arquivo define **como materializar e completar o workspace persistente**.

Para criação conduzida por IA, ele complementa `10-INICIAR-HISTORIA-COM-IA.md`; não substitui o processo autoral.

> **Primeiro decidir. Depois persistir. Não criar arquivos para preencher uma árvore ideal.**

---

# Quando a pasta nasce

No ramo `NOVA HISTÓRIA`, a pasta nasce somente depois de:

```text
PREMISSA → APROVADA
ESTILO / TOM → APROVADO
NOME → APROVADO ou provisório autorizado
SLUG → definido e sem conflito
```

Seguir `14-CRIACAO-NOME-E-DESTINO.md`.

Criar primeiro:

```text
campanhas/<slug>/README.md
```

Conteúdo mínimo inicial:

```text
# [NOME]

STATUS
→ EM PREPARAÇÃO

## Proposta curta
[Premissa aprovada.]

## Estilo / Tom
[Resumo aprovado.]
```

```text
DESTINO CRIADO
≠ PREPARAÇÃO CONCLUÍDA
≠ START
```

---

# Persistência progressiva

Depois que o workspace existe:

```text
material aprovado
→ fonte canônica correta.
```

Exemplos:

```text
Personagens centrais
→ README.md

ficha aprovada
→ personagens/<slug-da-personagem>.md

Autoridades / políticas
→ README.md

Direção
→ direcao.md

Mundo necessário
→ mundo/<assunto>.md

Estado inicial / atual
→ estado.md

Mesa / Auditoria / criação pendente que precisa sobreviver
→ operacao.md
```

Não criar arquivo vazio nem inventar conteúdo apenas para completar estrutura.

---

# Estrutura possível

Conforme a obra realmente precisar:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
├── personagens/
├── operacao.md             # somente quando houver operação transitória real
├── mundo/                  # somente quando houver mundo necessário persistente
├── arco.md                 # somente com Arco Preparado ativo
├── oposicao.md             # somente com Opositor ativo
└── livro/                  # somente com Livro ativo
```

A ausência de fonte opcional não é erro.

---

# Passo 1 — Personagens centrais

Seguir `15-CRIACAO-PERSONAGENS-CENTRAIS.md`.

Registrar no `README.md` somente a composição curta aprovada.

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

Preferir uma personagem por vez.

Salvar somente quando aprovada:

```text
campanhas/<slug>/personagens/<slug-da-personagem>.md
```

```text
FICHA SUFICIENTE
≠ FICHA EXAUSTIVA
```

Se uma ficha ainda não aprovada precisar sobreviver à perda de contexto:

```text
operacao.md
→ preserva a criação pendente.
```

---

# Passo 3 — Autoridades, Cadeiras e Executores

Seguir:

```text
17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
03-CADEIRAS-E-EXECUTORES.md
```

Ordem conceitual:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Registrar no `README.md`, conforme aprovado:

```text
DIRETOR
NARRADOR / JUIZ
PERSONAGEM DO DIRETOR, se houver
CADEIRAS necessárias
EXECUTOR de cada autoridade
limites de delegação, quando houver
```

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

---

# Passo 4 — Direção

Seguir:

```text
18-CRIACAO-DIRECAO.md
01-AUTORIDADE-E-DIRECAO.md
modelos/DIRECAO.md
```

Criar:

```text
campanhas/<slug>/direcao.md
```

A Direção pode ser mínima.

```text
DIRETOR NÃO DECIDIU O FUTURO
→ NÃO PREENCHER O FUTURO.
```

A Direção cresce conforme decisões autorais reais surgem.

---

# Passo 5 — Políticas Operacionais

Seguir:

```text
19-CRIACAO-POLITICAS-OPERACIONAIS.md
```

Registrar no `README.md`:

```text
POLÍTICA DE MESA
POLÍTICA DE INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

Padrões:

```text
MESA: SOB DEMANDA
INDICADOR OPERACIONAL: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real
```

Não transformar os padrões em questionário obrigatório.

---

# Passo 6 — Mundo Necessário

Seguir:

```text
20-CRIACAO-MUNDO-NECESSARIO.md
```

Resultado legítimo:

```text
MUNDO NECESSÁRIO
→ NENHUM ANTES DO START
```

Quando houver fatos externos estáveis realmente necessários, criar:

```text
campanhas/<slug>/mundo/<assunto>.md
```

Não construir enciclopédia por hábito.

Cânone externo permitido pode preencher lacunas; decisões locais da obra prevalecem.

---

# Passo 7 — Mesa inicial, quando necessária

Durante a preparação, Mesa pode ser usada quando já houver informação suficiente para consulta significativa.

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

# Passo 8 — Estado Inicial

Seguir:

```text
21-CRIACAO-ESTADO-INICIAL.md
modelos/ESTADO.md
```

Criar:

```text
campanhas/<slug>/estado.md
```

O Estado inicial é a âncora imediatamente anterior à primeira execução da Ficção.

Preservar somente quando pertinente:

```text
momento
local
presenças e posições
condições temporárias
intenções persistentes já estabelecidas
processos e prazos já existentes
conhecimentos recentes necessários
último fato estabelecido
primeiro ponto aberto
```

Antes do primeiro START:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

```text
ESTADO INICIAL
≠ PRIMEIRA CENA PRÉ-ESCRITA
```

Não colocar hipótese de Mesa, futuro desejado ou decisão voluntária ainda aberta como se já fosse fato.

O primeiro ponto aberto deve permitir reconhecer quem possui a próxima autoria.

```text
Cadeira IA disponível
→ START pode continuar.

Personagem do Diretor
→ START aguarda o Diretor, salvo Direção ou delegação suficiente.
```

Não exigir conflito, ameaça ou incidente incitante para considerar o Estado suficiente.

---

# Passo 9 — Auditoria de início

Antes do START, confirmar:

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
[ ] direcao.md é suficiente sem inventar futuro;
[ ] política de Mesa está definida ou usa SOB DEMANDA;
[ ] indicador está definido ou usa SILENCIOSO;
[ ] módulos ativos possuem função real;
[ ] mundo necessário foi definido ou legitimamente considerado desnecessário;
[ ] estado.md possui âncora inicial suficiente;
[ ] estado.md possui último fato e primeiro ponto aberto;
[ ] Estado não pré-escreveu decisão ainda aberta;
[ ] hipóteses não foram registradas como fatos;
[ ] operacao.md existe somente se houver operação real pendente.
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
→ caso contrário identificar o primeiro ponto aberto em estado.md
→ identificar quem possui a próxima autoria
→ iniciar a camada correta
```

Uma Cadeira IA disponível pode tomar a primeira iniciativa se o espaço aberto permitir.

Não existe obrigação de começar por ação, conflito ou perigo.

> **START continua do primeiro ponto aberto; não reinventa a preparação nem transforma o Estado inicial em cena já ocorrida.**

---

# Regra final

> **O workspace cresce junto com a preparação e com a própria história. O W4D persiste apenas decisões e fatos que realmente precisam sobreviver: fichas preservam pessoas, Direção preserva decisões autorais, políticas configuram o motor, mundo preserva estrutura externa necessária e Estado preserva a âncora presente. START só acontece quando existe base suficiente para executar corretamente.**