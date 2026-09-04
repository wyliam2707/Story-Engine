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
```

O Narrador apresenta a Ficção e pode emitir Parecer na Mesa. Ele não possui sentença causal soberana sobre resultados materiais abertos.

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

---

## Política de Mesa

Escolher uma:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Fonte normativa:

```text
regras-basicas/00-ARQUITETURA-E-MESA.md
```

Padrão:

```text
MESA: SOB DEMANDA
```

A Mesa pode ser usada para qualquer resultado autoral importante, inclusive combate, romance ou investigação.

```text
Mesa aberta
→ proposta, opinião e Parecer não são Ficção.

Diretor autoriza execução
→ versão fechada entra na Ficção.
```

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

Esse arquivo é operacional, não canônico.

---

## Módulos

- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: INATIVO
- Livro: INATIVO

Ativar somente módulos realmente usados.

---

## Convenção textual

Quando útil:

```text
[texto]
→ camada autoral do Diretor fora da Ficção.
```

A semântica, a política de Mesa e o modo atual determinam a operação.

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

Então:

```text
START
→ reancorar
→ reconstruir Cadeiras separadamente
→ identificar primeiro ponto aberto
→ identificar próxima autoria
→ iniciar a Ficção.
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