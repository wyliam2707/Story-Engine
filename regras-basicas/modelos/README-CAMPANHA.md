# [NOME DA HISTÓRIA / CAMPANHA]

STATUS
→ EM PREPARAÇÃO

## Proposta curta

[Premissa aprovada em uma ou duas frases que permitam reconhecer que história está sendo construída.]

## Estilo / Tom

[Resumo aprovado de gênero, tom, ritmo, escala, perspectiva ou limites de apresentação que realmente importem para reconhecer a experiência da obra.]

Não usar esta seção para registrar acontecimentos futuros, decisões de personagem ou clichês importados do gênero.

## Personagens centrais

[Adicionar depois que a etapa de Personagens Centrais for aprovada.]

Formato recomendado:

```text
- [Nome] — [papel estrutural curto na Premissa].
- [Nome] — [papel estrutural curto na Premissa].
```

Esta seção identifica **quem está no centro da obra**. Não substitui as fichas.

```text
README
→ composição central da obra.

personagens/<nome>.md
→ quem cada pessoa é.
```

## Autoridades

Preencher depois que a configuração de `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md` estiver aprovada.

### Diretor

```text
DIRETOR
Executor: [HUMANO / IA / OUTRO]
```

Na configuração mais comum:

```text
DIRETOR
Executor: HUMANO
```

### Narrador / Juiz

```text
NARRADOR / JUIZ
Executor: [HUMANO / IA / OUTRO]
```

### Personagem do Diretor

Registrar somente se existir:

```text
PERSONAGEM DO DIRETOR
- [nome]
  - vontade: DIRETOR
  - executor padrão: [HUMANO / IA / OUTRO / IA QUANDO DELEGADA]
```

```text
vontade: DIRETOR
```

significa que decisões voluntárias da personagem continuam pertencendo ao Diretor mesmo quando outro executor recebe autorização para dar forma textual à ação.

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

### Cadeiras

```text
CADEIRAS
- [Personagem A] → Executor: [HUMANO / IA / OUTRO]
- [Personagem B] → Executor: [HUMANO / IA / OUTRO]
```

Se houver delegação temporária ou limite operacional relevante, registrar somente o escopo real.

Outras personagens podem receber Cadeira persistente ou eventual quando adquirirem decisão voluntária relevante.

```text
PESSOA
→ definida pela ficha.

CADEIRA
→ autoria voluntária da personagem.

EXECUTOR
→ quem opera essa autoria.
```

Uma mesma IA pode executar Narrador e várias Cadeiras sem fundi-los.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

Executor e autoridade não pertencem à ficha da personagem.

Se alguma dessas definições ainda não existe durante `EM PREPARAÇÃO`, não preencher inventando. O README pode crescer progressivamente conforme as etapas são aprovadas.

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

Configurar Cadeiras não escolhe automaticamente a política de Mesa.

```text
CADEIRA
→ quem possui autoria da personagem.

POLÍTICA DE MESA
→ quando essa autoria é consultada fora da Ficção.
```

Em qualquer política:

```text
Mesa aberta
→ proposta, opinião de Cadeira e parecer do Narrador não são Ficção.

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

Depois que `direcao.md`, `estado.md`, as fichas iniciais e as autoridades necessárias estiverem suficientes:

```text
STATUS
→ PRONTA
```

Então:

```text
START
→ reancorar
→ reconstruir Cadeiras separadamente
→ identificar primeiro ponto aberto
→ identificar quem possui a próxima autoria
→ iniciar a Ficção.
```

Se existir `operacao.md` ativo, `START` ou retomada deve restaurar primeiro a operação pendente em vez de saltar por cima dela.

## Nota de criação progressiva

No nascimento do workspace, este README pode existir apenas com:

```text
nome
status EM PREPARAÇÃO
Proposta curta
Estilo / Tom
```

Depois, conforme aprovação:

```text
Personagens centrais
→ adicionar núcleo curto.

Autoridades
→ adicionar depois das fichas iniciais suficientes e da configuração aprovada.

políticas / módulos
→ adicionar somente quando definidos.
```

> **README incompleto durante preparação é melhor que README preenchido com decisões que o Diretor ainda não tomou.**