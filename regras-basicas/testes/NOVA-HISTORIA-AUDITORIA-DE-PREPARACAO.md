# Testes — Nova História: Auditoria de Preparação

Estes cenários verificam `22-CRIACAO-AUDITORIA-DE-PREPARACAO.md`.

O critério principal é:

> **A Auditoria deve verificar reconstruibilidade e autoridade, não exigir planejamento narrativo que não é necessário para o START.**

---

## Cenário 1 — História por descoberta sem arco futuro

A obra possui:

```text
README válido
duas fichas centrais reconstruíveis
autoridades definidas
direcao.md com Premissa, Tom e nenhum arco futuro
estado.md com âncora e primeiro ponto aberto
```

Não existe final, antagonista nem revelação planejada.

### Esperado

```text
AUDITORIA: APROVADA
STATUS → PRONTA
```

A ausência de futuro planejado não bloqueia.

---

## Cenário 2 — Mundo necessário inexistente por decisão legítima

A história contemporânea não depende de regras externas especiais.

Resultado anterior:

```text
MUNDO NECESSÁRIO
→ NENHUM ANTES DO START
```

Não existe pasta `mundo/`.

### Esperado

A Auditoria aprova normalmente.

Não cria worldbuilding apenas para completar a estrutura.

---

## Cenário 3 — Ficha central insuficiente

A personagem B é central e terá Cadeira IA já na abertura.

Seu arquivo contém apenas:

```text
Nome: B
Conceito: interesse amoroso
```

sem personalidade, repertório ou histórico suficiente para reconstruir a pessoa.

### Esperado

```text
AUDITORIA: BLOQUEADA
```

A IA informa que B ainda não é reconstruível.

Não inventa a ficha durante a Auditoria.

---

## Cenário 4 — Figurante sem ficha

O Estado inicial menciona uma atendente de cafeteria sem função persistente e sem decisão relevante necessária.

Ela não possui ficha.

### Esperado

A Auditoria não bloqueia.

```text
PERSONAGEM INCIDENTAL SEM NECESSIDADE DE CONTINUIDADE
→ ficha não obrigatória.
```

---

## Cenário 5 — Primeiro ponto aberto pertence ao Diretor

A obra está pronta e o primeiro ponto aberto é a resposta voluntária da Personagem do Diretor.

### Esperado

A Auditoria aprova.

O fato de o START precisar aguardar o Diretor **não significa preparação incompleta**.

```text
STATUS → PRONTA
START → apresenta o ponto aberto e aguarda.
```

---

## Cenário 6 — Estado pré-escreveu decisão de Cadeira IA

A Cadeira de Kara pertence à IA, mas `estado.md` registra:

```text
Primeiro ponto aberto:
Kara decide procurar Daniel e convidá-lo para sair.
```

Essa decisão ainda não havia sido tomada em Ficção nem fechada por Direção.

### Esperado

A Auditoria identifica contaminação de autoridade.

```text
AUDITORIA: BLOQUEADA
```

O Estado deve ser corrigido para preservar apenas a oportunidade ou situação aberta.

---

## Cenário 7 — Padrão de Mesa não copiado para README

Nenhuma política especial foi escolhida.

O README deixou a seção de Mesa vazia.

### Esperado

A Auditoria pode corrigir mecanicamente:

```text
MESA: SOB DEMANDA
```

sem perguntar ao Diretor.

Depois aprova, se não houver outro bloqueio.

---

## Cenário 8 — Contradição estrutural real

Premissa aprovada:

```text
Ana e Bruno começam como desconhecidos.
```

Estado inicial:

```text
Ana e Bruno são amigos de infância e chegam juntos ao local.
```

Nenhuma decisão posterior resolveu essa diferença.

### Esperado

A Auditoria não escolhe uma versão.

```text
AUDITORIA: BLOQUEADA
→ apresentar a contradição
→ perguntar qual versão prevalece.
```

---

## Cenário 9 — Módulos todos inativos

A história não usa Arco Preparado, Opositor, Romance nem Livro no início.

### Esperado

A Auditoria aprova.

```text
MÓDULOS OPCIONAIS INATIVOS
≠ PREPARAÇÃO INCOMPLETA
```

---

## Cenário 10 — Mesa de criação ainda pendente

Existe `operacao.md` registrando uma Mesa ainda aberta sobre uma decisão estrutural necessária para a abertura.

### Esperado

```text
AUDITORIA: BLOQUEADA
STATUS → EM PREPARAÇÃO
START → NÃO EXECUTAR
```

A operação pendente deve ser retomada primeiro.

---

## Cenário 11 — Observação editorial não bloqueante

Todos os fatos estão corretos, mas um cabeçalho usa `Tom da História` em vez de `Estilo / Tom`.

O significado é inequívoco.

### Esperado

A Auditoria não bloqueia.

Pode normalizar mecanicamente ou apenas aceitar a equivalência.

---

## Cenário 12 — Segredo global não virou conhecimento da personagem

`mundo/segredo.md` contém um fato oculto.

A ficha de A e o Estado não dizem que A o conhece.

### Esperado

A Auditoria aprova e preserva:

```text
ARQUIVO SABE
≠ PERSONAGEM SABE
```

Não distribui o segredo às Cadeiras por estar disponível ao executor.

---

## Cenário 13 — Auditoria não mostra checklist sem necessidade

Tudo passa.

### Esperado

Resposta adequada:

```text
Auditoria concluída. A obra está reconstruível e o primeiro ponto aberto está claro.
STATUS → PRONTA.
```

Não despejar toda a lista de verificação, salvo se o Diretor pedir.

---

## Cenário 14 — Rótulo legado Narrador / Juiz

README antigo contém:

```text
NARRADOR / JUIZ
Executor: IA
```

O restante do workspace não depende de dados, dificuldade, sentença causal ou poder soberano do Narrador.

### Esperado

```text
interpretar como NARRADOR → IA
normalizar mecanicamente quando houver atualização legítima
não pedir decisão autoral ao Diretor
não bloquear a preparação só pelo rótulo legado
```

A Auditoria pode aprovar se todo o restante estiver correto.

```text
RÓTULO LEGADO
≠ FUNÇÃO ATUAL REATIVADA
```

---

## Cenário 15 — Workspace ainda depende de Juiz

README ou regras locais dizem:

```text
quando um resultado importante estiver aberto,
o Narrador/Juiz decide sucesso ou falha por sentença própria.
```

Não existe decisão do Diretor nem Mesa prevista para esse resultado.

### Esperado

```text
AUDITORIA: BLOQUEADA
```

A IA não trata isso como mera formatação antiga, porque a semântica depende de uma função removida do W4D atual.

A correção deve restaurar:

```text
consequência ordinária/evidente
→ Narrador pode apresentar.

resultado material importante realmente aberto
→ permanece autoral
→ Mesa, quando necessária.
```

Não criar RNG, dificuldade ou Juiz invisível para preservar o comportamento antigo.

---

## Critério geral de conformidade

A implementação falha se:

```text
exigir final ou arco para aprovar;
exigir mundo completo;
exigir ficha de figurantes;
confundir próxima autoria do Diretor com falta de preparação;
canonizar uma escolha aberta para “corrigir” o Estado;
transformar padrão operacional em questionário;
tratar observação editorial como bloqueio;
tratar rótulo legado como poder atual de Juiz;
permitir workspace que ainda depende de sentença oculta para resultado material;
iniciar Ficção durante a Auditoria.
```

A implementação passa quando:

> **verifica autonomamente tudo que pode verificar, corrige apenas o que é mecânico e seguro, devolve ao Diretor somente decisões autorais realmente bloqueantes e marca PRONTA quando uma nova IA já conseguiria iniciar a obra corretamente pelos arquivos e pela arquitetura atual do W4D.**