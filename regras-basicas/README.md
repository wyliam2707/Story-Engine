# W4D — Regras Básicas

## O que o W4D se tornou

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

> **O Diretor conduz. As Cadeiras preservam as personagens. O Narrador julga. A ficção executa. O Registro preserva.**

---

# Se você é uma IA: leia isto primeiro

Se recebeu somente esta pasta, ela é suficiente para aprender a arquitetura.

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

A numeração histórica dos arquivos não é uma hierarquia de autoridade. A ordem acima foi escolhida para ensinar primeiro a arquitetura, depois as autoridades, depois a resolução e por fim criação e persistência.

---

# As três camadas

O W4D separa três coisas que modelos de linguagem tendem a misturar.

## 1 — MESA

Espaço autoral fora da ficção.

Aqui o Diretor pode propor uma ideia e ouvir as Cadeiras envolvidas antes de decidir.

```text
PROPOSTA
→ CADEIRAS OPINAM
→ NARRADOR ANALISA / JULGA
→ DIRETOR ALTERA, CANCELA OU CONFIRMA
```

Nada disso é automaticamente ficção.

## 2 — FICÇÃO

Quando o Diretor autoriza a execução, a ideia aprovada entra na cena segundo as autoridades do sistema.

```text
DIRETOR CONFIRMA
→ NARRADOR EXECUTA
→ A FICÇÃO ESTABELECE O QUE ACONTECEU
```

## 3 — REGISTRO

Depois, quando houver salvamento, checkpoint ou fechamento de capítulo, os fatos já estabelecidos são persistidos nas fontes corretas.

```text
FICÇÃO ESTABELECIDA
→ REGISTRO PRESERVA
```

> **Registrar preserva. Não cria.**

---

# Ciclo autoral completo

```text
IDEIA DO DIRETOR
↓
MESA DE AUTORIA, quando aberta
↓
CADEIRAS ENVOLVIDAS DÃO SUA LEITURA
↓
NARRADOR JULGA PLAUSIBILIDADE, FATOS E CAUSALIDADE
↓
DIRETOR DECIDE
├─ CANCELA → nada aconteceu
├─ ALTERA → nova consulta quando necessário
└─ CONFIRMA → executar
                ↓
              FICÇÃO
                ↓
              CONSEQUÊNCIAS
                ↓
              REGISTRO, quando solicitado
```

As distinções essenciais são:

```text
PROPOSTA
≠ CÂNONE

OPINIÃO DE CADEIRA
≠ DECISÃO CANÔNICA DA PERSONAGEM

JULGAMENTO DO NARRADOR NA MESA
≠ ACONTECIMENTO FICCIONAL

DIRETOR CONFIRMA
→ AUTORIZA EXECUÇÃO

EXECUÇÃO FICCIONAL
→ ESTABELECE O QUE ACONTECEU

REGISTRO
→ PRESERVA O QUE JÁ ACONTECEU
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

Uma única IA pode operar dez Cadeiras, mas deve fazê-lo em dez escopos distintos.

```text
MESMO EXECUTOR
≠
MESMA PERSONAGEM
```

Na Mesa, isso também permite que uma personagem diga ao Diretor:

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

Ele existe para:

```text
analisar
apontar contradições
consultar fatos
julgar causalidade
separar intenção de resultado
preservar consequências
transformar o que foi decidido em prosa clara
```

> **NARRADOR INFORMA ≠ NARRADOR VETA**

O Diretor pode mudar de ideia porque a objeção foi boa. Também pode manter conscientemente a escolha.

Depois que a escolha é confirmada, o Narrador executa sem ficar reabrindo a mesma discussão.

---

# Quando começar uma história do zero

Se não existe campanha/história pronta, use:

```text
10-INICIAR-HISTORIA-COM-IA.md
```

No W4D, `campanha` é apenas o nome técnico do espaço persistente da obra. A história pode ou não ser um RPG.

Modelos disponíveis:

```text
modelos/README-CAMPANHA.md
modelos/DIRECAO.md
modelos/ESTADO.md
modelos/FICHA.md
```

A IA deve perguntar somente o que realmente precisa ser decidido pelo Diretor. Quando houver base suficiente, deve **propor uma estrutura completa para revisão**, não transformar preparação em interrogatório.

---

# Quando retomar uma história existente

Use:

```text
06-REGISTRO-E-RETOMADA.md
```

Reconstrua:

```text
configuração da campanha
Direção
Estado
fichas relevantes
módulos ativos
pacotes separados das Cadeiras
primeiro ponto aberto
```

Não improvise continuidade se o contexto necessário estiver perdido.

---

# Regra de identidade

O nome `RPG` pode continuar sendo usado historicamente ou como modo de uso, mas a arquitetura não depende dele.

> **W4D é um sistema para construir ficção através de autoridade distribuída, consulta de personagens, julgamento causal e registro persistente. Jogar é uma forma de usá-lo; escrever uma história em conjunto é outra.**
