# [NOME DA HISTÓRIA / CAMPANHA]

STATUS
→ EM PREPARAÇÃO

## Proposta curta

[Premissa aprovada em uma ou duas frases.]

## Estilo / Tom

[Resumo aprovado do que realmente importa para reconhecer a experiência da obra.]

## Personagens centrais

[Adicionar depois da aprovação da etapa correspondente.]

Formato recomendado:

```text
- [Nome] — [papel estrutural curto].
- [Nome] — [papel estrutural curto].
```

```text
README
→ composição central e configuração da obra.

personagens/<nome>.md
→ quem cada pessoa é.
```

---

## Autoridades e funções

Preencher depois de `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md`.

### Diretor

```text
DIRETOR
Executor: [HUMANO / IA / OUTRO]
```

Padrão comum:

```text
DIRETOR
Executor: HUMANO
```

### Narrador

```text
NARRADOR
Executor: [HUMANO / IA / OUTRO]
```

No W4D atual:

```text
NARRADOR
≠ JUIZ
≠ SUPERVISOR DAS CADEIRAS
```

O Narrador apresenta a Ficção e pode emitir Parecer quando houver questão real. Não possui sentença causal soberana nem precisa aprovar novamente a vontade de uma Cadeira.

Arquivos antigos que usem `NARRADOR / JUIZ` devem ser interpretados como rótulo legado e podem ser normalizados mecanicamente para `NARRADOR`.

### Personagem do Diretor

Registrar somente se existir:

```text
PERSONAGEM DO DIRETOR
- [nome]
  - vontade: DIRETOR
  - executor padrão: [HUMANO / IA / OUTRO / IA QUANDO DELEGADA]
```

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

A IA pode executar a personagem com a mesma qualidade literária das demais, escolhendo como realizar a direção dentro do escopo autorizado. Não criar silêncio artificial, novos objetivos ou decisões fora da delegação.

```text
OBJETIVO
→ definido ou delegado pelo Diretor.

ESCOPO
→ somente ações, escolhas e intervalo autorizados.

CONDIÇÃO DE PARADA
→ quando devolver autoria ao Diretor.
```

Não exigir esses campos como formulário quando o contexto já os esclarecer. `Faça como achar melhor` delega a escolha em discussão, não toda a vida da personagem.

### Cadeiras

```text
CADEIRAS
- [Personagem A] → Executor: [HUMANO / IA / OUTRO]
- [Personagem B] → Executor: [HUMANO / IA / OUTRO]
```

```text
PESSOA
→ ficha.

CADEIRA
→ autoria voluntária.

EXECUTOR
→ quem opera essa autoria.
```

Uma mesma IA pode executar Narrador e várias Cadeiras sem fundi-los.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

Na Mesa, a Cadeira oferece julgamento autoral concreto, não uma fala ficcional. Pode concordar, discordar, propor condições ou apresentar intenção própria. A opinião pode ser breve. Não existe obrigação de consenso nem de parecer do Narrador para cada resposta.

### Agendas e iniciativa

Cada Cadeira mantém compromissos, intenções, relações e disponibilidade próprios, inclusive fora da presença da Personagem do Diretor. Na Mesa, pode apresentar o que pretende fazer no intervalo em discussão para permitir alinhamento autoral.

```text
CADEIRA SABE COMO AUTORA
≠ PERSONAGEM SABE NA FICÇÃO
```

Agendas não precisam ser exaustivas nem imutáveis. Compromissos e prazos estabelecidos pertencem ao Estado; propostas ainda em discussão pertencem à Operação. Não canonizar visitas apenas propostas.

---

## Política de Mesa

Padrão do W4D:

```text
MESA: CICLO OBRIGATÓRIO
```

O Diretor pode escolher expressamente outra política:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Fontes normativas:

```text
regras-basicas/00-ARQUITETURA-E-MESA.md
regras-basicas/24-CICLO-DE-AUTORIA.md
```

No ciclo obrigatório:

```text
IDEIA / DIREÇÃO / QUESTÃO
→ JULGAMENTO DAS CADEIRAS PERTINENTES
→ DISCUSSÃO SEM LIMITE FIXO DE RODADAS
→ PODE FAZER / AUTORIZAÇÃO EQUIVALENTE
→ FICÇÃO EXECUTA O ESCOPO APROVADO
```

Uma nova proposta não vira Ficção antes da autorização. O Diretor pode dispensar expressamente a consulta num escopo local, sem alterar a política persistente. A execução aprovada não exige nova Mesa para cada gesto ordinário.

Não perguntar ao Diretor se deseja ativar o ciclo obrigatório quando não houver preferência diferente. Registrar o padrão.

---

## Indicador operacional

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

Padrão:

```text
INDICADOR OPERACIONAL: SILENCIOSO
```

Exemplo atual, quando visível:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

Falha operacional que impeça execução correta deve ser informada mesmo no modo silencioso.

---

## Operação pendente

Quando Mesa, Auditoria ou outra operação precisar persistir:

```text
operacao.md
```

seguir:

```text
regras-basicas/modelos/OPERACAO.md
```

Esse arquivo é operacional, não canônico. Deve preservar a versão em discussão, as Cadeiras consultadas, as opiniões necessárias e o que aguarda o Diretor, sem promover propostas a fatos.

---

## Módulos

Módulos opcionais:

- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: INATIVO

Livro:

- Livro: PREPARADO — ativação obrigatória no START / primeira Ficção

Ativar somente módulos opcionais realmente usados.

O Livro não é opcional durante a Ficção:

```text
OBRA EM PREPARAÇÃO
→ Livro pode permanecer PREPARADO.

PRIMEIRA FICÇÃO EXECUTADA
→ Livro: ATIVO.
```

---

## Convenção textual

Quando útil:

```text
[texto]
→ camada autoral do Diretor fora da Ficção.
```

A semântica, a política de Mesa e o modo atual determinam a operação. Dentro de Mesa aberta, uma formulação declarativa continua em consulta até autorização ou cancelamento.

No Livro canônico, falas e pensamentos preservam a origem explicitamente:

```text
[Personagem] — fala.
[Personagem], pensa — pensamento.
```

A forma normativa completa está em `regras-basicas/modulos/LIVRO.md`.

---

## Cânone externo

[Definir aqui se outra obra, cenário ou fonte externa pode preencher lacunas.]

Regra recomendada:

```text
arquivos desta obra
→ prioridade.

cânone externo
→ referência para lacunas permitidas.
```

---

## Início operacional

Depois que `direcao.md`, `estado.md`, fichas e autoridades estiverem suficientes e a Auditoria for aprovada:

```text
STATUS
→ PRONTA
```

```text
PRONTA
≠ FICÇÃO JÁ INICIADA
```

Seguir:

```text
regras-basicas/23-START.md
```

Quando houver autorização semântica para começar:

```text
START
→ reancorar
→ reconstruir Cadeiras separadamente
→ identificar primeiro ponto aberto
→ identificar próxima autoria ou função
→ respeitar ciclo de Mesa e escopo já autorizados
→ ativar Livro obrigatoriamente
→ iniciar a Ficção sem redistribuir autoridade.
```

Se o Diretor já autorizou o começo antes da Auditoria, não perguntar novamente. Se pediu somente preparação, permanecer em `PRONTA` até autorização.

Quando a primeira Ficção realmente for executada:

```text
STATUS
→ EM EXECUÇÃO

Livro
→ ATIVO
```

Se existir `operacao.md` ativo, restaurar a operação pendente antes de saltar para Ficção.

---

## Nota de criação progressiva

No nascimento do workspace, este README pode conter apenas:

```text
nome
STATUS → EM PREPARAÇÃO
Proposta curta
Estilo / Tom
```

Depois acrescentar, conforme aprovação:

```text
Personagens centrais
Autoridades
Políticas
Módulos
```

> **README incompleto durante preparação é melhor que README preenchido com decisões que o Diretor ainda não tomou.**
