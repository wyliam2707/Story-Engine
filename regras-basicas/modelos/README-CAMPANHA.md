# [NOME DA HISTÓRIA / CAMPANHA]

STATUS
→ EM PREPARAÇÃO

## Proposta curta

[Uma ou duas frases que permitam reconhecer que história está sendo construída.]

## Autoridades

DIRETOR
Executor: [HUMANO / IA / OUTRO]

NARRADOR / JUIZ
Executor: [HUMANO / IA / OUTRO]

PERSONAGEM DO DIRETOR
- [nome, se houver]
  - vontade: DIRETOR
  - executor padrão: [HUMANO / IA / OUTRO]

CADEIRAS
- [Personagem A] → Executor: [HUMANO / IA / OUTRO]
- [Personagem B] → Executor: [HUMANO / IA / OUTRO]

Outras personagens podem receber Cadeira persistente ou eventual quando adquirirem decisão voluntária relevante.

## Política de Mesa

Escolher uma:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Definições em:

```text
regras-basicas/00-ARQUITETURA-E-MESA.md
```

Padrão quando não definido:

```text
MESA: SOB DEMANDA
```

Em qualquer política:

```text
Mesa aberta
→ proposta, opinião de Cadeira e parecer do Narrador não são ficção.

Diretor autoriza execução
→ Mesa fecha e a versão aprovada pode entrar na Ficção.
```

## Indicador operacional

Escolher uma:

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

Padrão de Story Engine:

```text
INDICADOR OPERACIONAL: SILENCIOSO
```

Mesmo no modo silencioso, perda de contexto ou falha operacional que impeça execução correta deve ser informada.

## Operação pendente

Quando uma Mesa, Auditoria ou outra operação precisar sobreviver a retomada, usar:

```text
operacao.md
```

seguindo:

```text
regras-basicas/modelos/OPERACAO.md
```

Esse arquivo é operacional, não canônico.

## Módulos

- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: INATIVO
- Livro: INATIVO

Ativar somente os módulos realmente usados.

## Convenção textual

Quando útil:

```text
[texto]
→ camada autoral do Diretor fora da ficção.
```

A semântica, a política de Mesa e o modo operacional atual determinam se o conteúdo é Consulta, Auditoria, Direção, Correção, Determinação ou outra operação.

## Cânone externo

[Definir aqui se outra obra, cenário ou fonte externa pode preencher lacunas.]

Regra recomendada:

```text
arquivos desta obra
→ prioridade.

cânone externo
→ referência apenas para lacunas permitidas.
```

## Início operacional

Depois que `direcao.md`, `estado.md` e as fichas iniciais estiverem suficientes:

```text
STATUS
→ PRONTA
```

Então:

```text
START
→ reancorar
→ identificar primeiro ponto aberto
→ iniciar a ficção.
```

Se existir `operacao.md` ativo, `START` ou retomada deve restaurar primeiro a operação pendente em vez de saltar por cima dela.