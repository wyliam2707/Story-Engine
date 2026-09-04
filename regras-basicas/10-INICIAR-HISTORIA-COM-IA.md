# 10 — Iniciar uma História Nova com IA

Este arquivo coordena **somente o ramo NOVA HISTÓRIA**.

Ele deve ser usado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`.

> **BOOT escolhe o caminho. Este arquivo coordena as etapas. Cada etapa específica define seu trabalho.**

Se o usuário quer continuar uma obra existente, usar `11-CONTINUAR-HISTORIA-COM-IA.md`.

---

# Princípio do processo

A criação acontece por etapas autorais separadas para evitar que a IA transforme uma ideia curta em obra inteira sem participação do Diretor.

Ao mesmo tempo:

> **Etapa separada não significa formulário obrigatório.**

Quando uma etapa já estiver semanticamente resolvida:

```text
organizar
→ propor ou registrar
→ confirmar somente quando necessário
→ avançar.
```

Regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

Não repetir perguntas já respondidas e não exigir planejamento futuro que o Diretor prefere descobrir escrevendo.

---

# Pipeline oficial de NOVA HISTÓRIA

```text
1. PREMISSA
→ 12-CRIACAO-PREMISSA.md

2. ESTILO / TOM
→ 13-CRIACAO-ESTILO-E-TOM.md

3. NOME / DESTINO CANÔNICO
→ 14-CRIACAO-NOME-E-DESTINO.md

4. PERSONAGENS CENTRAIS
→ 15-CRIACAO-PERSONAGENS-CENTRAIS.md

5. FICHAS
→ 16-CRIACAO-FICHAS.md

6. AUTORIDADES / CADEIRAS / EXECUTORES
→ 17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md

7. DIREÇÃO
→ 18-CRIACAO-DIRECAO.md

8. POLÍTICAS OPERACIONAIS
→ 19-CRIACAO-POLITICAS-OPERACIONAIS.md

9. MUNDO NECESSÁRIO
→ 20-CRIACAO-MUNDO-NECESSARIO.md

10. ESTADO INICIAL
→ 21-CRIACAO-ESTADO-INICIAL.md
→ modelos/ESTADO.md

11. AUDITORIA DE PREPARAÇÃO
→ 22-CRIACAO-AUDITORIA-DE-PREPARACAO.md

12. START
→ 23-START.md
```

---

# 1 — Premissa

Responde:

> **Que história estamos tentando construir?**

Não transformar Premissa em sinopse completa.

```text
PREMISSA: APROVADA
→ Estilo / Tom
```

---

# 2 — Estilo / Tom

Responde:

> **Como queremos experimentar e apresentar esta história?**

Pode definir gênero, tom, ritmo, escala, perspectiva e limites quando realmente importarem.

Não importar clichês como fatos.

---

# 3 — Nome / Destino

Definir:

```text
NOME
SLUG
DESTINO → campanhas/<slug>/
```

Antes de criar, verificar conflito.

Criar primeiro:

```text
campanhas/<slug>/README.md
```

com somente o que já foi aprovado.

```text
DESTINO CRIADO
≠ FICÇÃO INICIADA
```

---

# 4 — Personagens Centrais

Definir quem precisa sustentar a Premissa no início.

```text
PERSONAGEM CENTRAL
≠ FICHA CONCLUÍDA
```

Não criar elenco ornamental por hábito.

Não antecipar configuração de Cadeiras se ela ainda não foi dada.

```text
PESSOA
→ primeiro.
```

---

# 5 — Fichas

Usar:

```text
16-CRIACAO-FICHAS.md
04-FICHA.md
modelos/FICHA.md
```

Preferir uma personagem por vez:

```text
reunir o que já sabemos
→ identificar lacunas realmente importantes
→ propor
→ revisar
→ aprovar
→ salvar
```

```text
FICHA SUFICIENTE
≠ FICHA EXAUSTIVA
```

Não inventar trauma, segredo, fraqueza, poder ou drama para preencher campos.

---

# 6 — Autoridades / Cadeiras / Executores

Usar `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md`.

Ordem:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Configuração comum:

```text
DIRETOR → HUMANO
NARRADOR → IA
CADEIRAS não atribuídas ao Diretor → IA
```

No W4D atual:

```text
NARRADOR
≠ JUIZ
```

O Narrador apresenta a Ficção; resultados materiais abertos podem ir à Mesa.

Não escolher silenciosamente qual personagem pertence ao Diretor.

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

Registrar configuração aprovada no `README.md`.

---

# 7 — Direção

Usar `18-CRIACAO-DIRECAO.md`.

A Direção inicial preserva o que o Diretor já decidiu e ainda precisa continuar válido.

> **Direção não é plano obrigatório do futuro.**

```text
DIRETOR NÃO DECIDIU
→ NÃO PRECISA PREENCHER.
```

Salvar em:

```text
campanhas/<slug>/direcao.md
```

---

# 8 — Políticas Operacionais

Usar `19-CRIACAO-POLITICAS-OPERACIONAIS.md`.

Definir:

```text
POLÍTICA DE MESA
INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

Padrões:

```text
MESA: SOB DEMANDA
INDICADOR OPERACIONAL: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real
```

Padrões existem para evitar perguntas inúteis.

---

# 9 — Mundo Necessário

Usar `20-CRIACAO-MUNDO-NECESSARIO.md`.

Pergunta:

> **Existe fato externo às personagens que precisa estar definido antes do START?**

Resultado válido:

```text
MUNDO NECESSÁRIO: NENHUM ANTES DO START
```

Não construir enciclopédia por obrigação.

---

# 10 — Estado Inicial

Usar:

```text
21-CRIACAO-ESTADO-INICIAL.md
modelos/ESTADO.md
```

Pergunta:

> **Onde estamos quando a Ficção abrir, o que já é verdade e qual é a primeira coisa que continua aberta?**

```text
ESTADO SUFICIENTE
≠ PRIMEIRA CENA PRÉ-ESCRITA
```

Antes da primeira cena:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

O primeiro ponto aberto deve preservar a autoria correta ou identificar que o próximo passo é apenas continuidade evidente.

---

# Persistência progressiva

Depois que o workspace existe:

```text
Premissa / Estilo / composição central / autoridades / políticas
→ README.md

ficha aprovada
→ personagens/<nome>.md

Direção
→ direcao.md

mundo necessário
→ mundo/<assunto>.md

âncora e presente ficcional
→ estado.md
```

Se etapa ainda aberta precisar sobreviver à perda de contexto:

```text
operacao.md
→ preserva processo pendente sem canonizá-lo.
```

> **Persistir o que foi decidido. Não antecipar o que continua aberto.**

---

# 11 — Auditoria de Preparação

Usar:

```text
22-CRIACAO-AUDITORIA-DE-PREPARACAO.md
```

A Auditoria responde:

> **Uma nova IA conseguiria iniciar corretamente esta obra usando somente as fontes persistentes?**

Ela verifica também que a obra usa a arquitetura atual:

```text
Narrador sem função de Juiz
Mesa disponível para resultados materiais abertos
sem RNG universal
sem sentença causal escondida
```

```text
PRONTA
→ reconstruível e executável.

PRONTA
≠ completamente planejada.

PRONTA
≠ Ficção já iniciada.
```

Se aprovada:

```text
AUDITORIA: APROVADA
STATUS → PRONTA
→ START quando houver autorização semântica para começar.
```

Se o Diretor já havia dito `crie e comece`, `quando estiver pronta pode iniciar` ou equivalente, não pedir nova confirmação ritual.

Se pediu somente preparação/criação, parar em `PRONTA`.

---

# 12 — START

Usar:

```text
23-START.md
```

START:

```text
→ confirma autorização semântica para começar
→ reancora o mínimo necessário
→ reconstrói pacotes separados das Cadeiras
→ restaura operação pendente, se houver
→ caso contrário identifica primeiro ponto aberto
→ identifica próxima autoria ou função
→ começa a Ficção sem redistribuir autoridade
```

A partir do primeiro ponto:

```text
Cadeira IA disponível
→ decide e continua.

Personagem do Diretor / executor externo indisponível
→ Narrador pode apresentar a moldura inicial
→ parar antes da vontade necessária.

consequência ordinária/evidente
→ Narrador apresenta e continua.

resultado material importante realmente aberto
→ Mesa, quando necessária.
```

Não usar Juiz ou RNG invisível.

Não existe obrigação de começar por ação, conflito ou perigo.

Quando a primeira Ficção realmente for executada:

```text
STATUS
PRONTA
→ EM EXECUÇÃO
```

---

# Regra final

> **Uma nova história nasce por decisões suficientes, não por planejamento exaustivo. A preparação torna a obra reconstruível; a Auditoria verifica a arquitetura; e o START abre a Ficção exatamente no primeiro ponto aberto, preservando Diretor, Cadeiras, Mesa e Narrador em funções separadas — sem Juiz permanente.**