# 10 — Iniciar uma História Nova com IA

Este arquivo coordena **somente o ramo NOVA HISTÓRIA**.

Ele deve ser usado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`, quando criar uma obra nova já foi escolhido ou está inequívoco.

> **BOOT escolhe o caminho. Este arquivo coordena as etapas. Cada etapa específica define seu próprio trabalho.**

Se o usuário quer continuar uma obra existente, usar `11-CONTINUAR-HISTORIA-COM-IA.md`.

---

# Condição de entrada

Antes de usar este ramo:

```text
usuário escolheu criar uma história nova
OU
pedido já deixa isso inequivocamente claro.
```

Se isso ainda estiver aberto, voltar ao BOOT e perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

Não pedir Premissa, Estilo, fichas ou nome antes de resolver essa bifurcação.

---

# Princípio do processo

A criação acontece por etapas autorais separadas.

As etapas existem para evitar que a IA transforme uma ideia curta em obra inteira sem participação do Diretor.

Ao mesmo tempo:

> **Etapa separada não significa formulário obrigatório.**

Quando uma etapa já estiver semanticamente resolvida pelo material do Diretor:

```text
organizar
→ propor ou registrar
→ confirmar somente quando necessário
→ avançar.
```

Regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

Não repetir perguntas já respondidas.

Não exigir planejamento futuro que o Diretor prefere descobrir escrevendo.

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
→ modelos/ESTADO.md

11. AUDITORIA DE PREPARAÇÃO

12. START
```

---

# 1 — Premissa

A Premissa responde:

> **Que história estamos tentando construir?**

Não transformar Premissa em sinopse completa.

Quando aprovada:

```text
PREMISSA: APROVADA
→ Estilo / Tom
```

---

# 2 — Estilo / Tom

Responde:

> **Como queremos experimentar e apresentar esta história?**

Pode definir gênero, tom, ritmo, escala, perspectiva ou limites de apresentação quando realmente importarem.

Não usar gênero para importar clichês como fatos.

```text
ESTILO / TOM: APROVADO
→ Nome / Destino
```

---

# 3 — Nome / Destino Canônico

Definir:

```text
NOME DA OBRA
SLUG
DESTINO → campanhas/<slug>/
```

Antes de criar, verificar se o slug já existe.

Ao nascer o workspace, criar primeiro:

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

Definir quem precisa sustentar materialmente a Premissa no início.

```text
PERSONAGEM CENTRAL
≠ FICHA CONCLUÍDA
```

Não criar elenco ornamental por hábito.

Depois da aprovação, registrar apenas um bloco curto no `README.md`.

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

Não inventar trauma, segredo, fraqueza, poder ou drama apenas para preencher campos.

---

# 6 — Autoridades / Cadeiras / Executores

Definir quem possui cada vontade e quem opera cada autoridade.

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Na configuração comum:

```text
DIRETOR → HUMANO
NARRADOR / JUIZ → IA
CADEIRAS não atribuídas ao Diretor → IA
```

Não escolher silenciosamente qual personagem pertence ao Diretor.

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE
```

Registrar a configuração aprovada no `README.md`.

---

# 7 — Direção

Usar `18-CRIACAO-DIRECAO.md`.

A Direção inicial preserva o que o Diretor já decidiu e ainda precisa continuar válido.

> **Direção não é um plano obrigatório do futuro.**

Se não há arco, final ou trajetória futura decididos, eles permanecem abertos.

Uma Direção mínima é válida.

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

Definir como o W4D opera nesta obra:

```text
POLÍTICA DE MESA
POLÍTICA DE INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

Padrões quando o Diretor não demonstra preferência:

```text
MESA: SOB DEMANDA
INDICADOR OPERACIONAL: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real.
```

> **Padrões existem para evitar perguntas desnecessárias.**

Registrar no `README.md`.

---

# 9 — Mundo Necessário

Usar `20-CRIACAO-MUNDO-NECESSARIO.md`.

Pergunta central:

> **Existe algum fato externo às personagens que precisa estar definido antes do START?**

Resultado válido:

```text
MUNDO NECESSÁRIO: NENHUM ANTES DO START
```

Não construir enciclopédia por obrigação.

Quando houver fatos realmente necessários:

```text
campanhas/<slug>/mundo/<assunto>.md
```

Cânone externo pode preencher lacunas permitidas; decisões locais da obra prevalecem.

---

# 10 — Estado inicial

Criar `estado.md` somente quando o ponto inicial da Ficção estiver definido.

Usar `modelos/ESTADO.md`.

Preservar somente o presente necessário:

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

Antes da primeira cena:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

Não colocar futuros desejados no Estado.

---

# Persistência progressiva

Depois que o workspace existe, salvar somente material aprovado na fonte correta.

```text
Premissa / Estilo / composição central / autoridades / políticas
→ README.md

ficha aprovada
→ personagens/<nome>.md

Direção
→ direcao.md

mundo necessário
→ mundo/<assunto>.md

presente ficcional
→ estado.md
```

Se uma etapa ainda aberta precisar sobreviver a perda de contexto:

```text
operacao.md
→ preserva o processo pendente sem canonizá-lo.
```

> **Persistir o que foi decidido. Não antecipar o que continua aberto.**

---

# 11 — Auditoria de preparação

Antes do START, verificar:

```text
[ ] nome e slug definidos;
[ ] README.md existe;
[ ] Premissa e Estilo/Tom estão preservados;
[ ] personagens centrais necessárias estão identificadas;
[ ] fichas necessárias são reconstruíveis;
[ ] Diretor e Narrador/Juiz estão definidos;
[ ] Cadeiras e executores necessários estão definidos;
[ ] Personagem do Diretor está corretamente atribuída, se houver;
[ ] delegação não transferiu vontade por acidente;
[ ] direcao.md preserva o decidido sem exigir futuro inventado;
[ ] política de Mesa está definida ou usa SOB DEMANDA;
[ ] indicador está definido ou usa SILENCIOSO;
[ ] módulos ativos possuem função real;
[ ] mundo necessário foi definido ou legitimamente considerado desnecessário;
[ ] estado.md possui último fato e primeiro ponto aberto;
[ ] hipóteses não foram registradas como fatos;
[ ] operacao.md existe somente se houver operação real pendente.
```

Se suficiente:

```text
STATUS
→ PRONTA
```

---

# 12 — START

Depois da preparação:

```text
START
→ reancorar o mínimo necessário
→ reconstruir pacotes separados das Cadeiras
→ restaurar operação pendente, se houver
→ caso contrário identificar o primeiro ponto aberto
→ identificar quem possui a próxima autoria
→ começar a camada correta
```

Uma Cadeira IA disponível pode tomar a primeira iniciativa quando o espaço aberto permitir.

Não existe obrigação de começar por ação, conflito ou perigo.

---

# Regra final

> **Uma nova história no W4D nasce por decisões suficientes, não por planejamento exaustivo. A IA constrói cada etapa somente até o ponto necessário, usa padrões para evitar perguntas inúteis, cria mundo apenas quando há algo real para preservar e só abre a Ficção depois da preparação suficiente e do START.**