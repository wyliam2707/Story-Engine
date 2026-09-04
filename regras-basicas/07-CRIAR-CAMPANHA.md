# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico atual do espaço persistente de uma obra.

Este arquivo define **como materializar e completar o workspace persistente**.

Para criação conduzida por IA, ele complementa `10-INICIAR-HISTORIA-COM-IA.md`.

> **Primeiro decidir. Depois persistir. Não criar arquivos para preencher uma árvore ideal.**

---

# Quando a pasta nasce

No ramo `NOVA HISTÓRIA`, criar o destino somente depois de:

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

Conteúdo mínimo:

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

Mesa / Auditoria / criação pendente
→ operacao.md
```

Não criar arquivo vazio nem inventar conteúdo para completar estrutura.

---

# Estrutura possível

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
├── personagens/
├── operacao.md             # somente quando necessário
├── mundo/                  # somente quando necessário
├── arco.md                 # somente com Arco Preparado ativo
├── oposicao.md             # somente com Opositor ativo
└── livro/                  # somente com Livro ativo
```

A ausência de fonte opcional não é erro.

---

# Passo 1 — Personagens centrais

Seguir `15-CRIACAO-PERSONAGENS-CENTRAIS.md`.

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

Rascunho que precisa persistir antes da aprovação pode ficar em `operacao.md`.

---

# Passo 3 — Autoridades, Cadeiras e Executores

Seguir:

```text
17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
03-CADEIRAS-E-EXECUTORES.md
05-NARRADOR.md
```

Ordem:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Registrar no `README.md`:

```text
DIRETOR
NARRADOR
PERSONAGEM DO DIRETOR, se houver
CADEIRAS necessárias
EXECUTOR de cada função
deligações relevantes
```

No W4D atual:

```text
NARRADOR
≠ JUIZ
```

O Narrador apresenta a Ficção. Resultado material realmente aberto pode ir à Mesa.

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

---

# Passo 5 — Políticas Operacionais

Seguir `19-CRIACAO-POLITICAS-OPERACIONAIS.md`.

Registrar:

```text
POLÍTICA DE MESA
INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

Padrões:

```text
MESA: SOB DEMANDA
INDICADOR: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real
```

A Mesa pode ser usada para qualquer domínio narrativo, inclusive combate.

---

# Passo 6 — Mundo Necessário

Seguir `20-CRIACAO-MUNDO-NECESSARIO.md`.

Resultado legítimo:

```text
MUNDO NECESSÁRIO
→ NENHUM ANTES DO START
```

Quando houver fatos externos estáveis realmente necessários:

```text
campanhas/<slug>/mundo/<assunto>.md
```

Não construir enciclopédia por hábito.

---

# Passo 7 — Mesa inicial, quando necessária

Durante a preparação:

```text
DIRETOR PROPÕE
→ CADEIRAS OPINAM
→ NARRADOR PODE EMITIR PARECER
→ DIRETOR ALTERA, CANCELA OU FECHA
```

Nada discutido vira Ficção apenas porque houve concordância.

Uma proposta pode ser ajustada até existir uma versão que as Cadeiras consigam sustentar.

Depois do fechamento:

```text
RESULTADO FECHADO
→ não reabrir.

CAMINHO RESTANTE
→ Cadeiras executam.
```

Se a Mesa precisar sobreviver a pausa:

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

Antes do primeiro START:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

```text
ESTADO INICIAL
≠ PRIMEIRA CENA PRÉ-ESCRITA
```

O primeiro ponto aberto deve preservar a próxima autoria correta.

---

# Passo 9 — Auditoria de Preparação

Seguir:

```text
22-CRIACAO-AUDITORIA-DE-PREPARACAO.md
```

A Auditoria verifica se outra IA consegue reconstruir e iniciar corretamente a obra.

Ela também confirma:

```text
NARRADOR configurado sem função de Juiz
Mesa disponível para resultados materiais abertos
sem RNG universal
sem sentença escondida
```

Se tudo estiver suficiente:

```text
AUDITORIA: APROVADA
STATUS → PRONTA
```

Se houver bloqueio autoral real:

```text
AUDITORIA: BLOQUEADA
STATUS → EM PREPARAÇÃO
```

---

# START

Somente depois da Auditoria aprovada:

```text
START
→ reancorar o mínimo necessário
→ reconstruir Cadeiras separadamente
→ restaurar operação pendente, se houver
→ caso contrário identificar primeiro ponto aberto
→ identificar próxima autoria
→ iniciar a camada correta
```

Uma Cadeira IA disponível pode tomar iniciativa no espaço aberto.

Se surgir resultado material importante ainda não fechado:

```text
→ Mesa, quando necessária
→ não Juiz / RNG invisível
```

Não existe obrigação de começar por ação, conflito ou perigo.

---

# Regra final

> **O workspace cresce junto com a preparação. Fichas preservam pessoas; Direção preserva decisões autorais; políticas configuram o motor; mundo preserva fatos externos necessários; Estado preserva a âncora presente; e a Mesa substitui a necessidade de um Juiz para resultados autorais importantes. O Narrador apresenta a versão executável.**