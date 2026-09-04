# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico atual do espaço persistente de uma obra.

Ela pode ser:

```text
RPG narrativo
fanfic
romance seriado
aventura colaborativa
história conduzida por Diretor com Cadeiras IA
qualquer outra ficção compatível com a arquitetura
```

Este arquivo define **como materializar e completar o workspace persistente** de uma nova história.

Para uma IA começando do zero, ele não substitui o processo autoral de `10-INICIAR-HISTORIA-COM-IA.md`.

> **Primeiro construir a identidade da obra. Depois criar seu destino. Só então completar suas fontes persistentes.**

---

# Condição para criar a pasta

No ramo `NOVA HISTÓRIA`, a pasta não nasce no BOOT, na Premissa ou durante Estilo/Tom.

Antes de criar:

```text
PREMISSA
→ APROVADA

ESTILO / TOM
→ APROVADO

NOME
→ APROVADO ou provisório autorizado para persistência

SLUG
→ definido e sem conflito
```

Seguir:

```text
14-CRIACAO-NOME-E-DESTINO.md
```

Só então criar:

```text
campanhas/<slug>/README.md
```

Em GitHub e outros sistemas semelhantes, o arquivo materializa a pasta; diretórios vazios não precisam ser criados.

---

# Passo 0 — README âncora

No nascimento do workspace, criar primeiro:

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

Registrar somente decisões já aprovadas.

Não preencher antecipadamente como fatos:

```text
Personagens centrais ainda não aprovadas
Cadeiras ainda não definidas
Personagem do Diretor ainda não escolhido
módulos ainda não discutidos
Estado inicial ainda não construído
mundo ainda aberto
```

> **O README nasce como âncora; ele cresce conforme a preparação produz decisões legítimas.**

Modelo completo para quando a configuração avançar:

```text
modelos/README-CAMPANHA.md
```

---

# Persistência progressiva

Depois que o workspace existe:

```text
material aprovado
→ deve preferencialmente ser salvo na fonte canônica correta.
```

Exemplos:

```text
Personagens centrais aprovadas
→ bloco curto no README.md

ficha aprovada
→ personagens/<nome>.md

Direção construída
→ direcao.md

ponto inicial definido
→ estado.md

fato externo estável necessário
→ mundo/

Mesa/Auditoria/criação pendente que precisa sobreviver
→ operacao.md
```

Não criar arquivo vazio ou inventado apenas para completar uma árvore ideal.

```text
DESTINO CRIADO
≠ PREPARAÇÃO CONCLUÍDA
≠ START
```

---

# Estrutura esperada quando necessária

Ao longo da preparação, a obra pode chegar a:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
├── personagens/
├── operacao.md             # somente quando houver operação transitória real
├── mundo/                  # somente quando necessário
├── arco.md                 # somente com Arco Preparado ativo
├── oposicao.md             # somente com Opositor ativo
└── livro/                  # somente com Livro ativo
```

A ausência de uma fonte opcional não é erro.

A ausência de uma fonte necessária no momento do START é problema de preparação.

---

# Passo 1 — Personagens centrais

Depois que Nome/Destino estiver concluído, o processo autoral deve definir primeiro **quem sustenta a Premissa no início**.

Seguir:

```text
15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

Quando o núcleo for aprovado, registrar no `README.md` apenas uma identificação curta:

```text
## Personagens centrais

- Nome — papel estrutural curto.
- Nome — papel estrutural curto.
```

Não transformar essa seção em ficha resumida.

```text
README
→ quem está no centro da obra.

FICHA
→ quem cada pessoa é.
```

---

# Passo 2 — Fichas

Somente depois que as personagens centrais necessárias estiverem aprovadas, construir suas fichas.

Seguir:

```text
16-CRIACAO-FICHAS.md
04-FICHA.md
modelos/FICHA.md
```

O padrão é construir **uma personagem por vez**:

```text
reunir o que já sabemos
→ identificar lacunas realmente importantes
→ propor a pessoa
→ consolidar em ficha
→ Diretor corrige ou aprova
→ salvar a ficha aprovada
→ próxima personagem
```

Destino:

```text
campanhas/<slug>/personagens/<slug-da-personagem>.md
```

Uma ficha deve permitir que outro executor reconstrua a mesma pessoa sem depender da conversa original.

```text
FICHA SUFICIENTE
≠ FICHA EXAUSTIVA
```

Não criar trauma, segredo, fraqueza, romance passado, poder, equipamento ou outro conteúdo importante apenas para completar o modelo.

Personagens secundárias podem receber ficha depois, quando adquirirem relevância persistente.

Não criar ficha apenas porque uma pessoa foi mencionada na Premissa ou pode aparecer futuramente.

Se a criação de uma ficha ainda não aprovada precisar sobreviver a perda de contexto:

```text
operacao.md
→ preserva a etapa pendente.
```

Não transformar rascunho em ficha canônica apenas para persistir trabalho.

---

# Passo 3 — Direção

Criar `direcao.md` quando já existir material autoral suficiente para distinguir:

```text
que história está sendo conduzida
o que recebe foco recorrente
quais premissas estão fechadas
quais trajetórias ou limites persistentes existem
que espaço continua deliberadamente aberto
```

Usar:

```text
modelos/DIRECAO.md
```

A Direção não precisa antecipar a trama inteira.

Não registrar como Direção uma hipótese ainda em consulta.

---

# Passo 4 — Autoridades e políticas

À medida que forem definidas, registrar no `README.md`:

```text
DIRETOR
NARRADOR / JUIZ
CADEIRAS INICIAIS
EXECUTOR DE CADA AUTORIDADE
PERSONAGEM DO DIRETOR, quando houver
POLÍTICA DE MESA
POLÍTICA DE INDICADOR OPERACIONAL
MÓDULOS ATIVOS
```

Uma mesma IA pode executar várias funções.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
```

A configuração definitiva da Cadeira deve preservar a pessoa já construída.

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

Executor não pertence à ficha.

## Política de Mesa

Escolher conforme `00-ARQUITETURA-E-MESA.md`:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Padrão:

```text
MESA: SOB DEMANDA
```

## Indicador operacional

Escolher:

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

Padrão do Story Engine:

```text
INDICADOR OPERACIONAL: SILENCIOSO
```

---

# Passo 5 — Mesa inicial, quando necessária

Durante a preparação, a Mesa pode ser usada quando já houver informação suficiente para uma consulta significativa.

```text
DIRETOR PROPÕE
→ CADEIRAS ENVOLVIDAS OPINAM
→ NARRADOR EMITE PARECER
→ DIRETOR AJUSTA, CANCELA OU CONFIRMA
```

Nada discutido vira Ficção apenas porque houve concordância.

Se a operação precisar sobreviver a uma pausa ou perda de contexto:

```text
operacao.md
→ usar modelos/OPERACAO.md
```

---

# Passo 6 — Estado inicial

Criar `estado.md` apenas quando o ponto inicial da Ficção já estiver definido.

Usar:

```text
modelos/ESTADO.md
```

Ele deve indicar, quando pertinente:

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

Antes do início, o último fato pode ser simplesmente:

```text
história ainda não iniciada.
```

Não colocar hipótese de Mesa no Estado.

---

# Passo 7 — Mundo necessário

Criar `mundo/` somente quando a proposta depender de fatos externos estáveis que precisam persistir.

Não construir enciclopédia por obrigação.

Detalhes neutros podem surgir posteriormente por criação emergente conforme `02-RESOLUCAO.md`.

---

# Passo 8 — Módulos opcionais

Ativar somente o que a obra realmente usa:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

Módulo inativo não produz arquivo nem comportamento por hábito.

---

# Passo 9 — Auditoria de início

Antes de começar a Ficção, confirmar:

```text
[ ] nome e slug definidos;
[ ] README.md existe e STATUS = EM PREPARAÇÃO ou equivalente;
[ ] Premissa e Estilo/Tom aprovados estão preservados;
[ ] Personagens centrais necessárias estão aprovadas e identificadas;
[ ] Diretor e Narrador/Juiz estão definidos;
[ ] Cadeiras iniciais e executores necessários estão definidos;
[ ] Personagem do Diretor está corretamente atribuído, se houver;
[ ] política de Mesa está definida ou usa SOB DEMANDA;
[ ] indicador está definido ou usa SILENCIOSO;
[ ] direcao.md é suficiente para a condução inicial;
[ ] fichas necessárias são suficientes para reconstrução;
[ ] estado.md possui último fato e primeiro ponto aberto;
[ ] hipóteses não foram registradas como fatos;
[ ] operacao.md existe somente se houver operação real pendente;
[ ] módulos ativos possuem função real;
[ ] fatos secretos necessários possuem fonte legítima;
```

Quando suficiente:

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
→ iniciar a camada correta
```

O Diretor não precisa escrever toda a primeira cena.

Uma Cadeira IA disponível pode tomar a primeira iniciativa se a situação e o espaço aberto permitirem.

Não existe obrigação de começar por ação, conflito ou perigo.

---

# Regra final

> **A pasta nasce quando Nome e Destino estão definidos. Depois, o W4D identifica quem está no centro da obra, constrói cada pessoa antes de configurar sua Cadeira, salva somente fichas aprovadas e completa progressivamente Direção, autoridades, Estado e demais fontes. A existência do workspace não significa que a história já começou; apenas START transforma a preparação em Ficção executável.**