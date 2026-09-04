# 10 — Iniciar uma História Nova com IA

Este arquivo define **somente o ramo NOVA HISTÓRIA**.

Ele deve ser carregado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`, quando o usuário escolheu criar uma obra nova ou quando isso já estava explícito no pedido.

> **BOOT escolhe o caminho. Este arquivo coordena a criação da nova história.**

Se o usuário quer continuar uma obra existente, usar `11-CONTINUAR-HISTORIA-COM-IA.md`.

---

# Condição de entrada

Antes de usar este arquivo, uma destas condições precisa ser verdadeira:

```text
usuário disse que quer criar uma história nova
OU
pedido já deixa isso inequivocamente claro
```

Se a operação ainda estiver aberta, voltar ao BOOT e perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

Não pedir premissa, estilo, fichas ou nome antes dessa bifurcação estar resolvida.

---

# Processo por etapas

A criação não acontece em uma única resposta.

O W4D separa decisões autorais importantes para que o Diretor possa construir, revisar e corrigir a obra sem a IA preencher silenciosamente tudo de uma vez.

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
```

Depois de Personagens Centrais aprovadas, a próxima etapa é **FICHAS**.

As etapas seguintes completam Direção, autoridades, políticas, mundo necessário, Estado inicial, Auditoria de preparação e START.

> **Não pular uma etapa autoral separada apenas porque a IA consegue inventar uma solução plausível.**

---

# Etapa 1 — Premissa

Carregar:

```text
12-CRIACAO-PREMISSA.md
```

A Premissa responde:

> **Que história estamos tentando construir?**

Se o Diretor já trouxe uma ideia suficiente, sintetizar e devolver para revisão.

Se trouxe apenas uma intenção vaga, fazer uma pergunta autoral de alto valor por vez ou oferecer poucas alternativas realmente distintas.

Quando aprovada:

```text
PREMISSA: APROVADA
→ carregar 13-CRIACAO-ESTILO-E-TOM.md
```

---

# Etapa 2 — Estilo / Tom

Carregar:

```text
13-CRIACAO-ESTILO-E-TOM.md
```

Esta etapa responde:

> **Como queremos experimentar e apresentar esta história?**

Pode definir, quando relevante:

```text
gênero ou mistura de gêneros
tom predominante
ritmo
escala
proximidade emocional
peso de diálogo e descrição
perspectiva narrativa
limites persistentes de apresentação
```

Informação já dada pelo Diretor deve ser organizada, não perguntada novamente.

Quando aprovada:

```text
ESTILO / TOM: APROVADO
→ carregar 14-CRIACAO-NOME-E-DESTINO.md
```

---

# Etapa 3 — Nome / Destino Canônico

Carregar:

```text
14-CRIACAO-NOME-E-DESTINO.md
```

Esta etapa responde:

> **Como esta obra será identificada e onde sua preparação persistente viverá?**

Definir:

```text
NOME DA OBRA
→ identidade humana.

SLUG
→ identidade técnica estável.

DESTINO
→ campanhas/<slug>/
```

Antes de criar, verificar se o slug já existe.

No nascimento do workspace, registrar somente o que já foi aprovado:

```text
# NOME

STATUS
→ EM PREPARAÇÃO

## Proposta curta
[Premissa aprovada]

## Estilo / Tom
[Resumo aprovado]
```

Quando concluído:

```text
NOME / DESTINO
→ CONCLUÍDO
→ carregar 15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

---

# Etapa 4 — Personagens Centrais

Carregar:

```text
15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

Esta etapa responde:

> **Quem precisa existir no centro desta obra para que a Premissa possa funcionar?**

Definir apenas o núcleo inicial suficiente:

```text
nome ou identificação provisória
papel estrutural na Premissa
relação mínima necessária
origem externa, quando houver
Personagem do Diretor, se isso já for relevante e estiver claro
```

Não criar personalidade completa, histórico, poderes ou ficha por hábito.

```text
PERSONAGEM CENTRAL
≠ FICHA CONCLUÍDA
```

Quando o núcleo for aprovado:

```text
PERSONAGENS CENTRAIS: APROVADAS
→ registrar bloco curto no README.md da obra
→ seguir para FICHAS
```

---

# Destino canônico e persistência progressiva

Antes da etapa de Nome/Destino:

```text
PREMISSA e ESTILO/TOM
→ podem existir apenas na conversa de criação.
```

Depois que o workspace nasce:

```text
campanhas/<slug>/README.md
→ âncora persistente da obra.
```

As próximas decisões aprovadas devem ser registradas progressivamente na fonte correta.

Exemplos:

```text
Personagens centrais aprovadas
→ README.md

ficha aprovada
→ personagens/<nome>.md

Direção construída
→ direcao.md

ponto inicial definido
→ estado.md

fato externo estável necessário
→ mundo/
```

Não criar arquivos vazios ou conteúdo inventado apenas para completar uma árvore ideal.

> **Persistir o que foi decidido. Não antecipar o que ainda está aberto.**

---

# Objetivo da IA na criação

A IA não deve começar inventando uma trama inteira sozinha nem transformar preparação em interrogatório.

Ela deve construir a obra por etapas, preservando as decisões autorais do Diretor.

Como regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

Isso significa sintetizar quando já existe material e perguntar somente quando falta algo que muda materialmente a etapa atual.

---

# Autoridades

Durante a criação, identificar quando necessário:

```text
DIRETOR
NARRADOR / JUIZ
PERSONAGEM DO DIRETOR, se houver
CADEIRAS
EXECUTORES
POLÍTICA DE MESA
```

Na configuração mais comum com IA:

```text
DIRETOR
→ humano.

NARRADOR / JUIZ
→ IA.

CADEIRAS SECUNDÁRIAS OU CO-PROTAGONISTAS
→ IA, salvo indicação diferente.
```

Não é necessário resolver todas essas configurações durante as primeiras etapas se ainda não forem materialmente relevantes.

A etapa de Personagens Centrais é normalmente o primeiro ponto em que pode fazer sentido esclarecer se alguma personagem pertence diretamente ao Diretor.

---

# Política de Mesa

Usar `00-ARQUITETURA-E-MESA.md` quando a política precisar ser definida ou quando o Diretor abrir consulta.

Opções:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Padrão quando nada for definido:

```text
MESA: SOB DEMANDA
```

---

# Fichas

Depois de Personagens Centrais aprovadas, construir fichas somente para quem precisa persistir.

Seguir:

```text
04-FICHA.md
modelos/FICHA.md
```

A ficha registra **quem a pessoa é**, não apenas sua função narrativa.

```text
PERSONAGENS CENTRAIS
→ quem sustenta a obra.

FICHAS
→ quem cada pessoa é.
```

Personagens secundárias podem receber ficha depois, quando adquirirem função persistente.

---

# Direção

A Direção inicial será construída a partir das decisões de criação aprovadas.

Ela deve dizer que história está sendo conduzida sem antecipar toda a trama.

Seguir:

```text
01-AUTORIDADE-E-DIRECAO.md
modelos/DIRECAO.md
```

Hipótese ainda em discussão não entra em `direcao.md` como decisão fechada.

---

# Mesa durante a criação

A criação também pode usar Mesa de Autoria quando já houver Cadeiras ou informação suficiente para consulta significativa.

```text
Diretor propõe
→ Cadeiras pertinentes opinam
→ Narrador emite PARECER
→ Diretor ajusta, cancela ou confirma
```

Antes de existirem fichas suficientes, a IA não deve fingir que uma Cadeira já possui personalidade detalhada que ainda não foi construída.

---

# Estado inicial e START

Antes do START, `estado.md` deve indicar exatamente onde a Ficção começa.

Não colocar no Estado acontecimentos que o Diretor apenas pretende produzir mais tarde.

Quando a preparação estiver suficiente:

```text
STATUS
→ PRONTA
```

Então:

```text
START
→ assumir Narrador/Juiz
→ reconstruir pacotes separados das Cadeiras
→ identificar o primeiro ponto aberto
→ começar a camada correta
```

> **Não fabricar conflito apenas porque a história está começando.**

---

# Não perguntar demais

Perguntar somente quando a escolha:

```text
é autoralmente importante para a etapa atual
muda materialmente o que está sendo definido
não pode ser inferida sem tomar decisão que pertence ao Diretor
```

Não pedir detalhes irrelevantes apenas para preencher formulários.

Ao mesmo tempo, não usar `Base suficiente → propor` como desculpa para pular Premissa, Estilo/Tom, Nome/Destino, Personagens Centrais ou outra etapa definida separadamente.

---

# Protocolo atual do ramo

```text
BOOT
↓
NOVA HISTÓRIA
↓
PREMISSA
→ 12-CRIACAO-PREMISSA.md
↓
ESTILO / TOM
→ 13-CRIACAO-ESTILO-E-TOM.md
↓
NOME / DESTINO
→ 14-CRIACAO-NOME-E-DESTINO.md
↓
criar campanhas/<slug>/README.md
↓
PERSONAGENS CENTRAIS
→ 15-CRIACAO-PERSONAGENS-CENTRAIS.md
↓
FICHAS
↓
DIREÇÃO / AUTORIDADES / POLÍTICAS / MUNDO NECESSÁRIO
↓
ESTADO INICIAL
↓
AUDITORIA DE PREPARAÇÃO
↓
START
```

As etapas posteriores podem receber arquivos próprios conforme forem refinadas.

---

# Regra final

> **Depois que NOVA HISTÓRIA foi escolhida, a IA passa por Premissa, Estilo/Tom, Nome/Destino e Personagens Centrais como decisões autorais separadas. O workspace nasce somente depois do nome e do slug; o elenco central é aprovado antes das fichas; e a Ficção só começa depois da preparação necessária e do START.**