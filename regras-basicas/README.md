# W4D — Story Engine

## O que o W4D é hoje

**W4D é uma arquitetura de autoria narrativa distribuída.**

Ele nasceu com linguagem de RPG, mas não depende de dados, combate, vitória, personagem-jogador ou estrutura de jogo para funcionar. Pode ser usado como:

```text
RPG narrativo
coautoria de ficção com IA
sala de roteiro distribuída
motor para histórias seriadas
fanfic assistida por IA
ferramenta de construção e continuidade narrativa
```

O objetivo central é permitir que uma pessoa conduza uma obra sem precisar escrever sozinha todas as personagens e, ao mesmo tempo, sem entregar a obra inteira a um único executor IA.

> **O Diretor conduz. As Cadeiras preservam as personagens. O Narrador emite parecer na Mesa e sentencia na Ficção. O Registro preserva.**

---

# Se você é uma IA: leia isto primeiro

Se recebeu somente esta pasta, ela deve ser suficiente para aprender a arquitetura.

Leia nesta ordem operacional:

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
07-CRIAR-CAMPANHA.md
↓
10-INICIAR-HISTORIA-COM-IA.md
```

Depois leia somente os módulos realmente ativados.

A numeração atual é histórica. Ela **não representa prioridade normativa**. A ordem acima é a ordem pedagógica recomendada até uma futura migração de nomes/numeração.

---

# As três camadas

O W4D separa três coisas que modelos de linguagem tendem a misturar.

## 1 — MESA

Espaço autoral fora da ficção.

```text
PROPOSTA OU DECISÃO EM EXAME
→ CADEIRAS ENVOLVIDAS OPINAM
→ NARRADOR EMITE PARECER
→ DIRETOR ALTERA, CANCELA OU AUTORIZA EXECUÇÃO
```

Nada disso é automaticamente ficção.

## 2 — FICÇÃO

Depois da autorização:

```text
CADEIRAS DECIDEM O QUE CONTINUA ABERTO
→ NARRADOR SENTENCIA CAUSALIDADE
→ PROSA APRESENTA O QUE ACONTECEU
```

## 3 — REGISTRO

Depois, quando houver salvamento, checkpoint ou fechamento de capítulo:

```text
FICÇÃO ESTABELECIDA
→ REGISTRO PRESERVA
```

> **Registrar preserva. Não cria.**

---

# Vocabulário mínimo

```text
MESA
Cadeira  → OPINIÃO
Narrador → PARECER
Diretor  → DECISÃO AUTORAL

FICÇÃO
Cadeira  → INTENÇÃO / DECISÃO DA PERSONAGEM
Narrador → SENTENÇA
Prosa    → APRESENTAÇÃO

REGISTRO
→ PRESERVAÇÃO
```

As distinções essenciais são:

```text
PROPOSTA
≠ CÂNONE

OPINIÃO CONSULTIVA
≠ DECISÃO FICCIONAL

PARECER
≠ SENTENÇA

DECISÃO AUTORAL
≠ ACONTECIMENTO JÁ EXECUTADO

EXECUÇÃO FICCIONAL
→ ESTABELECE O QUE ACONTECEU

REGISTRO
→ PRESERVA O QUE JÁ ACONTECEU
```

---

# Políticas de Mesa

Cada obra pode configurar uma política.

```text
MESA: SOB DEMANDA
→ consulta quando o Diretor pede.

MESA: CONSULTAR PROPOSTAS
→ propostas claramente consultivas passam pela Mesa antes de execução.

MESA: CONSULTA FORTE
→ até uma decisão recém-formulada pode receber opinião breve das Cadeiras antes de executar,
   salvo ordem do Diretor para seguir sem consulta.
```

Definição normativa:

```text
00-ARQUITETURA-E-MESA.md
```

Padrão quando nada for definido:

```text
MESA: SOB DEMANDA
```

---

# Por que existem Cadeiras

Uma IA tende a homogeneizar personagens quando executa todas ao mesmo tempo.

A Cadeira obriga o executor a perguntar separadamente:

```text
quem é esta pessoa?
o que ela sabe?
o que ela quer?
o que ela considera plausível?
como esta relação específica altera sua resposta?
```

Uma única IA pode operar várias Cadeiras, mas deve fazê-lo em escopos distintos.

```text
MESMO EXECUTOR
≠
MESMA PERSONAGEM
```

Na Mesa, uma Cadeira pode dizer:

```text
"isso parece comigo"
"isso não parece comigo"
"eu faria, mas por outro motivo"
"isso seria possível apenas se X estivesse presente"
```

A opinião informa o Diretor. Não o governa.

---

# O papel do Narrador

O Narrador não existe para inventar drama nem para concordar com o Diretor.

Na Mesa:

```text
NARRADOR
→ analisa
→ aponta contradições
→ consulta fatos
→ prevê consequências
→ emite PARECER
```

Na Ficção:

```text
NARRADOR
→ separa intenção de resultado
→ cruza fatos, decisões e capacidades
→ SENTENCIA
→ apresenta em prosa clara
```

> **NARRADOR INFORMA ≠ NARRADOR VETA**

O Diretor pode mudar de ideia porque a objeção foi boa. Também pode manter conscientemente a escolha.

Depois que a escolha é confirmada, o Narrador executa sem ficar reabrindo a mesma discussão.

---

# Quando a Ficção precisa parar

Não interromper apenas porque surgiu nova decisão de uma Cadeira IA que o próprio executor já pode operar.

```text
CADEIRA IA DISPONÍVEL
→ trocar de escopo
→ decidir
→ continuar.
```

Parar quando a próxima autoria legítima depender de:

```text
Diretor
humano ou executor externo indisponível
Mesa aguardando decisão
Auditoria pendente
reancoragem necessária
```

> **Pare por indisponibilidade de autoria, não por existência de autoria.**

---

# Estado operacional

`estado.md` registra a realidade ficcional.

Uma Mesa ou Auditoria pendente não é realidade ficcional.

Quando uma operação transitória precisa sobreviver a perda de contexto, pode existir:

```text
operacao.md
```

Modelo:

```text
modelos/OPERACAO.md
```

```text
ESTADO
→ realidade da Ficção.

OPERAÇÃO
→ pergunta/processo fora da Ficção ainda pendente.
```

> **Operação preserva a pergunta. Não canoniza a resposta.**

---

# Modelos disponíveis

```text
modelos/README-CAMPANHA.md
modelos/DIRECAO.md
modelos/ESTADO.md
modelos/OPERACAO.md
modelos/FICHA.md
```

---

# Criar uma história do zero

Use:

```text
10-INICIAR-HISTORIA-COM-IA.md
```

A IA deve perguntar somente o que realmente precisa ser decidido pelo Diretor. Quando houver base suficiente, deve **propor uma estrutura para revisão**, não transformar preparação em interrogatório.

---

# Retomar uma história existente

Use:

```text
06-REGISTRO-E-RETOMADA.md
```

Reconstrua:

```text
configuração da obra
Direção
Estado
Operação, se houver
fichas relevantes
módulos ativos
pacotes separados das Cadeiras
primeiro ponto aberto ou decisão autoral pendente
```

Não improvise continuidade se o contexto necessário estiver perdido.

---

# Módulos opcionais

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

Módulo inativo não participa da obra.

---

# Princípio documental

> **Uma ideia, uma definição, uma fonte principal.**

Principais fontes normativas:

```text
Mesa e políticas de consulta
→ 00-ARQUITETURA-E-MESA.md

Autoridade e Direção
→ 01-AUTORIDADE-E-DIRECAO.md

Cadeiras e Executores
→ 03-CADEIRAS-E-EXECUTORES.md

Resolução da Ficção
→ 02-RESOLUCAO.md

Ficha
→ 04-FICHA.md

Narrador
→ 05-NARRADOR.md

Persistência e retomada
→ 06-REGISTRO-E-RETOMADA.md

Plausibilidade e ritmo
→ 08-PLAUSIBILIDADE-E-RITMO.md
```

Quando um resumo parecer competir com a fonte normativa, use a fonte normativa.

---

# Regra de identidade

O nome `RPG` pode continuar sendo usado historicamente ou como modo de uso, mas a arquitetura não depende dele.

> **W4D é um Story Engine para construir ficção através de autoridade distribuída, consulta de personagens, parecer autoral, sentença causal e registro persistente. Jogar é uma forma de usá-lo; escrever uma história em conjunto é outra.**