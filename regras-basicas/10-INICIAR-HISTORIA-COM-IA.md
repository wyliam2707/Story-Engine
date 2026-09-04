# 10 — Iniciar uma História Nova com IA

Este arquivo define **somente o ramo NOVA HISTÓRIA**.

Ele deve ser carregado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`, quando o usuário escolheu criar uma obra nova ou quando isso já estava explícito no pedido.

> **BOOT escolhe o caminho. Este arquivo coordena a criação da nova história.**

Se o usuário quer continuar uma obra existente, usar `11-CONTINUAR-HISTORIA-COM-IA.md`.

---

# Condição de entrada

Antes de usar este arquivo:

```text
usuário disse que quer criar uma história nova
OU
pedido já deixa isso inequivocamente claro
```

Se a operação ainda estiver aberta, voltar ao BOOT e perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

Não pedir Premissa, Estilo, fichas ou nome antes dessa bifurcação estar resolvida.

---

# Processo por etapas

A criação não acontece em uma única resposta.

Etapas formalizadas:

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
```

Depois da Direção suficiente para início, completar apenas o que ainda for necessário:

```text
políticas operacionais
mundo necessário
Estado inicial
Auditoria de preparação
START
```

> **As etapas separam decisões e fontes; não criam burocracia ritual.**

Quando uma etapa já estiver semanticamente resolvida pelo material do Diretor, a IA deve sintetizar, confirmar somente quando necessário e avançar.

---

# Etapa 1 — Premissa

Carregar `12-CRIACAO-PREMISSA.md`.

Responde:

> **Que história estamos tentando construir?**

Se o Diretor já trouxe uma ideia suficiente, sintetizar e devolver para revisão.

Se trouxe apenas intenção vaga, fazer uma pergunta autoral de alto valor por vez ou oferecer poucas alternativas realmente distintas.

```text
PREMISSA: APROVADA
→ 13-CRIACAO-ESTILO-E-TOM.md
```

---

# Etapa 2 — Estilo / Tom

Carregar `13-CRIACAO-ESTILO-E-TOM.md`.

Responde:

> **Como queremos experimentar e apresentar esta história?**

Informação já dada deve ser organizada, não perguntada novamente.

```text
ESTILO / TOM: APROVADO
→ 14-CRIACAO-NOME-E-DESTINO.md
```

---

# Etapa 3 — Nome / Destino Canônico

Carregar `14-CRIACAO-NOME-E-DESTINO.md`.

Definir:

```text
NOME DA OBRA
SLUG
DESTINO → campanhas/<slug>/
```

Antes de criar, verificar se o slug já existe.

No nascimento do workspace, criar apenas a âncora:

```text
campanhas/<slug>/README.md
```

com o que já foi aprovado:

```text
nome
STATUS → EM PREPARAÇÃO
Premissa
Estilo / Tom
```

Criar a pasta não inicia a Ficção.

```text
NOME / DESTINO: CONCLUÍDO
→ 15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

---

# Etapa 4 — Personagens Centrais

Carregar `15-CRIACAO-PERSONAGENS-CENTRAIS.md`.

Responde:

> **Quem precisa existir no centro desta obra para que a Premissa funcione?**

Definir somente o núcleo inicial suficiente.

```text
PERSONAGEM CENTRAL
≠ FICHA CONCLUÍDA
```

Não criar elenco ornamental nem personalidade automática a partir de função narrativa.

Quando aprovado:

```text
registrar bloco curto no README.md
→ 16-CRIACAO-FICHAS.md
```

---

# Etapa 5 — Fichas

Carregar:

```text
16-CRIACAO-FICHAS.md
04-FICHA.md
modelos/FICHA.md
```

Construir preferencialmente uma personagem por vez:

```text
reunir o que já sabemos
→ identificar lacunas realmente importantes
→ perguntar somente quando necessário
→ propor a pessoa
→ consolidar em ficha
→ Diretor corrige ou aprova
→ salvar
```

```text
FICHA SUFICIENTE
≠ FICHA EXAUSTIVA
```

Não inventar trauma, segredo, fraqueza, romance passado, poder ou drama para preencher campos.

Quando as fichas necessárias à abertura estiverem suficientes:

```text
→ 17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
```

---

# Etapa 6 — Autoridades / Cadeiras / Executores

Carregar `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md`.

Responde:

> **Quem possui cada vontade e quem executa cada autoridade quando a Ficção começar?**

Ordem conceitual:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Definir, quando necessário:

```text
DIRETOR
NARRADOR / JUIZ
PERSONAGEM DO DIRETOR, se houver
CADEIRAS persistentes necessárias
EXECUTOR de cada autoridade
limites de delegação, quando existirem
```

Na configuração mais comum:

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

Quando aprovado:

```text
registrar no README.md
→ 18-CRIACAO-DIRECAO.md
```

---

# Etapa 7 — Direção

Carregar:

```text
18-CRIACAO-DIRECAO.md
01-AUTORIDADE-E-DIRECAO.md
modelos/DIRECAO.md
```

A etapa responde:

> **O que o Diretor já decidiu e ainda precisa permanecer válido quando a história começar?**

A Direção inicial **não é planejamento obrigatório do futuro**.

A IA deve consolidar:

```text
Premissa aprovada
+
Estilo / Tom aprovado
+
fatos estruturais já fechados
+
decisões persistentes ou locais realmente tomadas, se houver
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

Isso é suficiente.

Não perguntar por obrigação:

```text
final
arco completo
momento de revelação
quem se apaixona primeiro
quem vence conflitos futuros
estrutura de capítulos
```

> **O Diretor não precisa saber para onde a história vai antes de começar.**

A Direção pode crescer durante a Ficção conforme novas decisões autorais surgirem.

```text
DIREÇÃO: SUFICIENTE PARA INÍCIO
→ persistir em direcao.md
```

---

# Persistência progressiva

Depois que o workspace nasce, salvar apenas material aprovado na fonte correta:

```text
Personagens centrais
→ README.md

ficha aprovada
→ personagens/<nome>.md

Autoridades
→ README.md

Direção suficiente
→ direcao.md

ponto inicial
→ estado.md

fato externo estável necessário
→ mundo/
```

Se uma etapa ainda aberta precisar sobreviver à perda de contexto:

```text
operacao.md
→ preserva o processo pendente sem canonizá-lo.
```

> **Persistir o que foi decidido. Não antecipar o que ainda está aberto.**

---

# Políticas operacionais

Antes do START, registrar no `README.md` quando ainda necessário:

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

Padrão quando nada for definido:

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

Não transformar essas configurações em personalidade das personagens.

---

# Mundo necessário

Criar `mundo/` somente quando fatos externos estáveis realmente precisarem persistir antes do início.

Não construir enciclopédia por obrigação.

Cânone externo permitido pode preencher lacunas conforme a configuração da obra, mas decisões locais prevalecem.

---

# Estado inicial

Antes do START, criar `estado.md` quando o ponto inicial estiver definido.

Ele deve preservar somente o presente ficcional necessário:

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

# Auditoria de preparação

Antes do START, verificar:

```text
[ ] nome e slug definidos;
[ ] README.md existe;
[ ] Premissa e Estilo/Tom estão preservados;
[ ] personagens centrais necessárias estão identificadas;
[ ] fichas necessárias são reconstruíveis;
[ ] Diretor e Narrador/Juiz estão definidos;
[ ] Cadeiras e executores necessários estão definidos;
[ ] Personagem do Diretor está corretamente atribuído, se houver;
[ ] delegação não transferiu vontade por acidente;
[ ] direcao.md preserva o que foi realmente decidido sem exigir futuro inventado;
[ ] política de Mesa está definida ou usa SOB DEMANDA;
[ ] indicador está definido ou usa SILENCIOSO;
[ ] estado.md possui último fato e primeiro ponto aberto;
[ ] hipóteses não foram registradas como fatos;
[ ] operacao.md existe somente se houver operação real pendente;
[ ] módulos ativos possuem função real;
```

Se suficiente:

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
→ começar a camada correta
```

Uma Cadeira IA disponível pode tomar a primeira iniciativa quando o espaço aberto permitir.

Não existe obrigação de começar por ação, conflito ou perigo.

---

# Regra de interação

Como regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

E, para a criação inteira:

> **Etapa separada não significa formulário obrigatório.**

Não repetir perguntas já resolvidas e não exigir decisões futuras que o Diretor prefere descobrir escrevendo.

---

# Protocolo atual do ramo

```text
BOOT
↓
NOVA HISTÓRIA
↓
PREMISSA
↓
ESTILO / TOM
↓
NOME / DESTINO
↓
criar campanhas/<slug>/README.md
↓
PERSONAGENS CENTRAIS
↓
FICHAS
↓
AUTORIDADES / CADEIRAS / EXECUTORES
↓
DIREÇÃO MÍNIMA / PROGRESSIVA
↓
POLÍTICAS / MUNDO NECESSÁRIO
↓
ESTADO INICIAL
↓
AUDITORIA DE PREPARAÇÃO
↓
START
```

---

# Regra final

> **Depois que NOVA HISTÓRIA foi escolhida, a IA constrói somente o necessário para a obra começar corretamente. A Direção não obriga planejamento: preserva o que o Diretor já decidiu e deixa o restante aberto. O workspace recebe material aprovado progressivamente, e a Ficção só começa depois do START.**