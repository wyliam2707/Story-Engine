# W4D — Story Engine

## O que o W4D é hoje

**W4D é uma arquitetura de autoria narrativa distribuída.**

Ele não depende de dados, combate, vitória, personagem-jogador ou estrutura de jogo para funcionar.

> **O Diretor conduz. As Cadeiras decidem as personagens. A Mesa alinha o que precisa ser fechado. O Narrador apresenta a Ficção. O Registro preserva.**

O W4D atual não possui `Juiz` permanente.

```text
SEM RNG UNIVERSAL
SEM TESTE UNIVERSAL
SEM DIFICULDADE UNIVERSAL
SEM SENTENÇA OCULTA DO NARRADOR
```

---

# Se você é uma IA: BOOT primeiro

Comece em:

```text
09-BOOT-E-ESCOLHA-DE-OPERACAO.md
```

Leia o núcleo nesta ordem pedagógica:

```text
README.md
↓
00-ARQUITETURA-E-MESA.md
↓
01-AUTORIDADE-E-DIRECAO.md
↓
03-CADEIRAS-E-EXECUTORES.md
↓
02-RESOLUCAO.md
↓
04-FICHA.md
↓
05-NARRADOR.md
↓
08-PLAUSIBILIDADE-E-RITMO.md
↓
06-REGISTRO-E-RETOMADA.md
↓
24-CICLO-DE-AUTORIA.md
```

O arquivo 24 é parte obrigatória do núcleo, não um módulo opcional. Ele consolida o ciclo de Mesa, a delegação delimitada e as agendas independentes. Quando um resumo antigo divergir sobre esses pontos, aplicar a especificação vigente do arquivo 24.

Depois do núcleo, se a operação ainda não estiver clara:

> **Você quer criar uma história nova ou continuar uma história existente?**

```text
NOVA HISTÓRIA
→ 10-INICIAR-HISTORIA-COM-IA.md
→ 07-CRIAR-CAMPANHA.md
→ 23-START.md quando a preparação estiver pronta e houver autorização para começar

CONTINUAR HISTÓRIA EXISTENTE
→ 11-CONTINUAR-HISTORIA-COM-IA.md
→ 06-REGISTRO-E-RETOMADA.md
```

---

# As três camadas

## MESA

Espaço autoral fora da Ficção.

```text
1. IDEIA / DIREÇÃO / QUESTÃO
→ 2. JULGAMENTO DAS CADEIRAS PERTINENTES
→ 3. DISCUSSÃO E REFINAMENTO, SEM LIMITE FIXO DE RODADAS
→ 4. PODE FAZER / AUTORIZAÇÃO EQUIVALENTE
```

O padrão é `MESA: CICLO OBRIGATÓRIO`. Toda nova proposta autoral passa pela Mesa, salvo execução direta expressamente autorizada. O Diretor pode discutir por quantas mensagens desejar. A Cadeira oferece avaliação própria, concreta e tão breve quanto a questão permitir. Não é necessário um parecer do Narrador para aprovar cada opinião.

Nada disso acontece ficcionalmente até autorização.

## FICÇÃO

```text
Direção preserva pontos fechados
→ Cadeiras decidem o espaço aberto
→ consequências evidentes podem seguir diretamente
→ Narrador apresenta a continuidade
```

A execução respeita objetivo, escopo e condição de parada. Não exigir nova Mesa para cada gesto dentro de uma cena autorizada. Não ampliar uma delegação limitada para decidir o restante do dia.

Se um resultado materialmente importante continua realmente aberto, o Narrador não cria um vencedor escondido. A questão pode voltar à Mesa.

## REGISTRO

```text
Ficção estabelecida
→ Registro preserva
```

> **Registrar preserva. Não cria.**

---

# Vocabulário mínimo

```text
MESA
Cadeira  → JULGAMENTO / OPINIÃO AUTORAL
Narrador → PARECER, quando útil
Diretor  → DECISÃO AUTORAL

FICÇÃO
Cadeira  → INTENÇÃO / DECISÃO DA PERSONAGEM NO ESPAÇO ABERTO
Direção  → PONTOS FECHADOS
Narrador → APRESENTAÇÃO / CONTINUIDADE

REGISTRO
→ PRESERVAÇÃO
```

Distinções essenciais:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO CONSULTIVA ≠ DECISÃO FICCIONAL
PARECER ≠ DECISÃO AUTORAL
DECISÃO AUTORAL ≠ ACONTECIMENTO JÁ EXECUTADO
APRESENTAÇÃO ≠ AUTORIA ESCONDIDA
```

---

# A Mesa resolve autoria, não probabilidade

A Mesa pode ser usada em qualquer domínio:

```text
romance
combate
investigação
perseguição
negociação
cotidiano
```

Ela pode encontrar uma versão executável:

```text
Diretor propõe X
→ Cadeira rejeita X nas condições atuais
→ outra versão Y é construída
→ Cadeira sustenta Y
→ Diretor fecha Y
→ Ficção executa Y
```

Depois:

```text
RESULTADO FECHADO
→ não reabrir.

CAMINHO ABERTO
→ Cadeiras continuam autoras.
```

> **A Mesa pode fechar o destino; as Cadeiras descobrem o caminho.**

Isso não significa usar Mesa para cada detalhe cotidiano durante uma execução já autorizada.

> **Mesa obrigatória para a nova proposta, não para cada gesto da Ficção.**

---

# Políticas de Mesa

```text
MESA: CICLO OBRIGATÓRIO
→ padrão de toda nova obra.

MESA: SOB DEMANDA
→ alternativa escolhida expressamente pelo Diretor.

MESA: CONSULTAR PROPOSTAS
→ alternativa escolhida expressamente pelo Diretor.

MESA: CONSULTA FORTE
→ alternativa escolhida expressamente pelo Diretor.
```

A fonte normativa é `00-ARQUITETURA-E-MESA.md`, complementada por `24-CICLO-DE-AUTORIA.md`. A autorização local de execução direta não altera a política persistente.

---

# Cadeiras

Uma Cadeira pergunta separadamente:

```text
quem é esta pessoa?
o que ela sabe?
o que ela quer?
como esta relação altera sua resposta?
que parte da autoria ainda está aberta?
```

Uma única IA pode operar várias Cadeiras, mas em escopos separados.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

Na Mesa, a Cadeira é a função autoral, não a personagem falando dentro da Ficção. Pode dizer `ela ainda não está pronta` ou `ela diria sim, mas prefere calma`. O julgamento não precisa ser longo; precisa ser próprio. A IA não deve concordar por conveniência nem criar resistência artificial.

A Cadeira pode discordar do Diretor. Essa resistência é informativa, não veto. Depois que o Diretor compreende a objeção e fecha conscientemente um resultado, a Cadeira muda de pergunta:

```text
antes
→ eu faria isso?

depois do fechamento
→ como faço isso dentro do espaço ainda aberto?
```

---

# Personagem do Diretor e delegação

A vontade da Personagem do Diretor permanece com ele. A IA pode executar a personagem com a mesma qualidade literária das demais, escolhendo como realizar o objetivo autorizado.

```text
VONTADE
→ DIRETOR.

EXECUÇÃO TEXTUAL
→ DIRETOR ou IA dentro da delegação.
```

O Diretor pode escolher uma alternativa ou dizer `faça como achar melhor`. Essa frase delega a escolha em discussão, não toda a agenda. Uma direção ampla pode autorizar um intervalo inteiro e estabelecer condições de parada. Não inventar o evento de parada nem ultrapassar o limite autorizado.

---

# Agendas e iniciativa própria

As Cadeiras conservam compromissos, intenções, relações e disponibilidade fora da presença do protagonista. Na Mesa, podem apresentar o que pretendem fazer durante o intervalo em discussão. O Diretor pode usar essas informações para alinhar cenas sem conceder conhecimento indevido às personagens.

```text
CADEIRA SABE COMO AUTORA
≠ PERSONAGEM SABE NA FICÇÃO
```

Uma visita proposta não é uma visita acontecida. Uma agenda não precisa preencher cada hora, nem se torna roteiro imutável. O Registro preserva compromissos e prazos reais, não possibilidades descartadas.

---

# Ruptura deliberada

Uma Cadeira pode dizer `isso não parece algo que eu faria`. O Diretor pode reconhecer que essa ruptura é deliberada e autorizar execução.

Nesse caso, a Cadeira não reabre a objeção, não inventa causa oculta, executa o caminho restante e preserva conhecimento legítimo.

```text
EXECUTOR SABE A CAUSA
≠ PERSONAGEM SABE A CAUSA
```

> **Coerência protege contra ruptura acidental; não governa uma ruptura conscientemente escolhida pelo Diretor.**

---

# Narrador

O Narrador não é Juiz nem supervisor das Cadeiras.

Na Mesa, pode emitir Parecer quando houver questão real. Na Ficção, preserva continuidade, apresenta decisões, aplica consequências ordinárias e evidentes e dá forma literária sem aumentar o tabuleiro.

Se um resultado material permanece realmente aberto, não escolhe secretamente. A questão pode ir à Mesa.

> **NARRADOR INFORMA ≠ NARRADOR VETA.**

O Narrador não precisa concordar com a escolha para executá-la bem.

---

# Quando continuar e quando parar

```text
CADEIRA IA disponível
→ trocar de escopo, decidir e continuar dentro da execução autorizada.

CONSEQUÊNCIA ORDINÁRIA / EVIDENTE
→ Narrador apresenta e continua.

RESULTADO MATERIAL IMPORTANTE AINDA ABERTO
→ Mesa, quando necessária.
```

Parar quando a próxima autoria depender do Diretor, de executor externo indisponível, de Mesa aguardando decisão, de Auditoria, de fonte indispensável, de reancoragem ou quando uma condição de parada ou limite do escopo for alcançado.

> **Pare por indisponibilidade de autoria, condição de parada ou limite do escopo, não pela mera existência de escolha.**

---

# Estado operacional

```text
estado.md
→ realidade da Ficção.

operacao.md
→ processo fora da Ficção ainda pendente.
```

> **Operação preserva a pergunta. Não canoniza a resposta.**

---

# Criar uma história do zero

Depois que `NOVA HISTÓRIA` foi escolhida:

```text
10-INICIAR-HISTORIA-COM-IA.md
```

A criação é progressiva e não exige planejamento completo do futuro.

A preparação termina em:

```text
AUDITORIA APROVADA
→ STATUS: PRONTA
```

A Ficção começa conforme:

```text
23-START.md
```

```text
PRONTA
≠ FICÇÃO JÁ INICIADA
```

---

# Continuar uma história existente

Depois que `CONTINUAR HISTÓRIA EXISTENTE` foi escolhida:

```text
11-CONTINUAR-HISTORIA-COM-IA.md
06-REGISTRO-E-RETOMADA.md
```

```text
RETOMAR ≠ RECRIAR
```

---

# Modelos

```text
modelos/README-CAMPANHA.md
modelos/DIRECAO.md
modelos/ESTADO.md
modelos/OPERACAO.md
modelos/FICHA.md
```

---

# Módulos

Módulos opcionais:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
```

Módulo obrigatório durante a Ficção:

```text
modulos/LIVRO.md
```

```text
OBRA EM PREPARAÇÃO
→ Livro pode estar apenas PREPARADO.

PRIMEIRA FICÇÃO EXECUTADA
→ Livro ATIVO obrigatoriamente.
```

Módulo opcional inativo não participa da obra. O Livro não pode permanecer inativo depois do START.

---

# Testes de conformidade

A pasta `testes/` inclui testes por etapa, testes gerais do engine, regressão sem Juiz e teste específico do START.

Em especial:

```text
testes/CENARIOS-DE-CONFORMIDADE.md
testes/MESA-SEM-JUIZ.md
testes/NOVA-HISTORIA-START.md
testes/CICLO-DE-AUTORIA.md
```

O novo teste cobre julgamento breve, Mesa aberta, delegação delimitada, condições de parada, agendas próprias e resultados autorais.

---

# Fontes normativas principais

```text
Mesa e alinhamento autoral
→ 00-ARQUITETURA-E-MESA.md

Autoridade e Direção
→ 01-AUTORIDADE-E-DIRECAO.md

Resolução autoral e execução
→ 02-RESOLUCAO.md

Cadeiras e Executores
→ 03-CADEIRAS-E-EXECUTORES.md

Ficha
→ 04-FICHA.md

Narrador
→ 05-NARRADOR.md

Registro e retomada
→ 06-REGISTRO-E-RETOMADA.md

Plausibilidade e ritmo
→ 08-PLAUSIBILIDADE-E-RITMO.md

BOOT
→ 09-BOOT-E-ESCOLHA-DE-OPERACAO.md

Criação de nova história
→ 10-INICIAR-HISTORIA-COM-IA.md

Retomada
→ 11-CONTINUAR-HISTORIA-COM-IA.md

START
→ 23-START.md

Ciclo obrigatório, delegação e agendas
→ 24-CICLO-DE-AUTORIA.md
```

---

# Regra de identidade

> **W4D é um Story Engine para construir ficção por autoridade distribuída. Ele não precisa de um Juiz para descobrir a história: Diretor e Cadeiras decidem o que importa, a Mesa constrói e fecha com autorização do Diretor, o Narrador apresenta e o Registro preserva.**
