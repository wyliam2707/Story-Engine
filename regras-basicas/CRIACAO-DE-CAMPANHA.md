# Criação de Campanha

Status: REFORMULAÇÃO ATIVA

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **Cada passo usa o anterior como base: primeiro definir a narrativa, depois criar e fechar estruturalmente a temporada, depois construir fichas persistentes para essa campanha.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
PASSO 01 — CAMPANHA
→ definir a identidade narrativa persistente.

PASSO 02 — TEMPORADA
→ receber a direção do Jogador.
→ criar o problema da temporada.
→ listar o que precisa ser resolvido.
→ responder previamente as questões estruturais.
→ registrar a Diretriz Fechada.

PASSO 03 — FICHAS
→ identificar o elenco inicial.
→ construir as personagens através da lente da campanha.
→ usar a primeira temporada apenas como contexto inicial.

DEPOIS
→ pareamento mínimo
→ situação inicial
→ Configuração das Cadeiras
→ START
```

Não pedir novamente informação já fornecida.

## 1 — Estrutura da campanha

Depois que o nome for aprovado, materializar:

```text
campanhas/<nome>/
├── README.md
├── personagens/
├── estado/
│   └── atual.md
├── mundo/
├── mestre/
│   ├── narrativa.md
│   ├── roteiro.md
│   └── temporadas/
├── opositor/
└── livro/
```

O `README.md` da campanha começa com:

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: PASSO 01 — CAMPANHA
```

## PASSO 01 — Narrativa da Campanha

O primeiro passo define **que tipo de história esta campanha quer acompanhar ao longo das temporadas**.

Perguntar somente o necessário:

```text
foco principal
gênero e tom
experiência desejada
temas e relações que devem receber espaço
tipos de conflito compatíveis
o que não deve dominar
premissas gerais já válidas
```

Registrar em:

```text
campanhas/<nome>/mestre/narrativa.md
```

A Narrativa da Campanha é persistente entre temporadas.

```text
NARRATIVA
→ identidade da campanha.

TEMPORADA
→ arco atual.
```

Uma trama secundária interessante não reescreve automaticamente a identidade da campanha.

## PASSO 02 — Criar a Temporada

Depois da Narrativa, seguir `CRIACAO-DE-TEMPORADA.md`.

Fluxo:

```text
DIREÇÃO DO JOGADOR
↓
PROBLEMA DA TEMPORADA
↓
LISTA DO QUE PRECISA SER RESOLVIDO
↓
RESPOSTAS CANÔNICAS NECESSÁRIAS
↓
DIRETRIZ FECHADA
```

O roteiro ativo fica em:

```text
campanhas/<nome>/mestre/roteiro.md
```

O roteiro estabelece o tabuleiro estrutural, não cenas futuras nem decisões voluntárias das personagens.

Quando a temporada termina:

```text
resolver o arco
→ escrever epílogo
→ consolidar mudanças
→ arquivar roteiro
→ perguntar “E agora?”
```

## PASSO 03 — Criar as Fichas

Somente depois de existir Narrativa da Campanha e roteiro inicial, construir o elenco que já precisa de agência.

Para cada personagem, começar com:

```text
Nome
IMPORTÂNCIA NARRATIVA
CONTROLE
Conceito, quando já conhecido
ESTADO DA FICHA: EM CRIAÇÃO
```

### Importância Narrativa

```text
PROTAGONISTA
RECORRENTE
EVENTUAL
INCIDENTAL
```

Importância Narrativa indica quanto desenvolvimento e continuidade precisam ser preservados.

```text
IMPORTÂNCIA NARRATIVA
→ quanto preservar.

CONTROLE
→ quem decide.

FICHA
→ quem é e o que consegue fazer.
```

Ela não mede poder, não concede bônus e não altera autoridade.

`Patamar` pertence ao motor anterior e não faz parte da criação ativa.

Depois do elenco, seguir:

```text
jogador/1.3-criacao-da-ficha.md
```

A ficha é persistente além da temporada que ajudou a contextualizar sua criação.

## 4 — Pareamento mínimo

Antes do START, comparar somente personagens cujas fichas possuam fatos cruzados relevantes.

Verificar quando necessário:

```text
se já se conhecem
natureza atual da relação
fatos compartilhados importantes
conhecimento legítimo de uma sobre a outra
obrigações, acessos ou vínculos recorrentes
```

Se uma lacuna puder surgir naturalmente em cena sem contradição, não é preciso preenchê-la antes.

## 5 — Situação inicial

Depois das fichas e do pareamento, registrar em:

```text
campanhas/<nome>/estado/atual.md
```

somente o presente necessário para abrir a primeira cena.

Quando relevante:

```text
momento ou período
local
personagens presentes
posições relevantes
situação imediata
condições ou efeitos temporários ativos
transformações em curso
equipamentos ou recursos temporariamente indisponíveis
intenções persistentes
processos ou prazos já em andamento
primeiro ponto ainda aberto
```

Não criar campos universais de `Vida`, `Mente` ou `Mana`.

```text
RECURSO / CUSTO / CONDIÇÃO ESPECÍFICA
→ só acompanhar se existir legitimamente na ficha, Poder, Equipamento, Traço, regra canônica ou Estado da campanha.
```

O Estado Atual é presente operacional, não histórico.

## 6 — Configuração das Cadeiras

Registrar no `README.md` da campanha quem ocupa cada cadeira necessária e qual função de autoridade está ativa.

A Configuração das Cadeiras responde:

> **Quem está sentado e qual autoridade cada cadeira possui nesta campanha?**

Ela é um registro persistente de composição da campanha. Não é uma Mesa aberta nem um procedimento de auditoria.

Exemplo:

```text
## Configuração das Cadeiras

JOGADOR HUMANO → <personagem>
JOGADOR IA — <personagem> → <personagem>
JOGADOR IA EVENTUAL → ATIVO, quando necessário
OPOSITOR → ATIVO
NARRADOR / JUIZ → ATIVO
```

Cada personagem com cadeira própria mantém sua própria autoridade mesmo quando uma única IA técnica executa várias cadeiras.

A palavra `Mesa` fica reservada ao procedimento temporário de alinhamento definido pelo Núcleo:

```text
DÚVIDA / DISCORDÂNCIA / CONFLITO REAL
→ abrir Mesa.

QUESTÃO RESOLVIDA
→ encerrar Mesa e voltar à ficção.
```

## 7 — START

Antes da primeira cena, conferir somente se a campanha consegue funcionar:

```text
estrutura existe?
Narrativa da Campanha foi aprovada?
Direção da temporada está clara?
problema da temporada existe?
Diretriz Fechada está registrada?
condição de encerramento existe?
elenco inicial foi confirmado?
fichas necessárias estão aprovadas?
pareamento essencial foi resolvido?
Estado inicial está definido?
CONTROLE das peças está claro?
Configuração das Cadeiras está registrada?
```

Se faltar algo essencial:

```text
CRIAÇÃO: EM ANDAMENTO
→ registrar a etapa
→ não iniciar ficção.
```

Se estiver pronto:

```text
CRIAÇÃO: CONCLUÍDA
→ seguir INICIO-E-RETOMADA.md
→ abrir a primeira cena.
```

START é somente a passagem da criação para o jogo.

## Ciclo entre temporadas

Depois da primeira temporada, a campanha e as fichas continuam existindo.

```text
CAMPANHA
→ persistente.

FICHAS
→ persistentes.

TEMPORADA
→ renovável.
```

Uma nova temporada pode exigir complementar uma ficha quando uma lacuna tiver alta chance de causar interpretação incoerente. Isso não significa revisar todas as fichas automaticamente.

## Criação emergente depois do START

Lacunas menores podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`.

A criação emergente não pode:

```text
alterar a Diretriz Fechada
introduzir retroativamente um novo problema estrutural
fabricar vantagem ou obstáculo para responder a uma ação já declarada
```

## Regra final

> **Nova campanha segue três passos dependentes: Narrativa, Temporada e Fichas. Depois disso, a Configuração das Cadeiras registra quem ocupa cada autoridade persistente; Mesa é reservada ao alinhamento temporário que só abre diante de dúvida, discordância ou conflito real. A situação inicial registra fatos atuais concretos, não trilhos universais herdados do motor anterior. Vida, Mente e Mana não são pressupostos da campanha nova; qualquer condição, custo ou recurso só existe quando uma fonte canônica específica realmente o estabelece.**