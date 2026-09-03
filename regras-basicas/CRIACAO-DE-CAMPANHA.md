# Criação de Campanha

Status: REFORMULAÇÃO ATIVA

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **Toda campanha precisa de uma Direção antes do START. A Direção define que tipo de história estamos tentando escrever; ela não precisa definir antecipadamente uma trama.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
PASSO 01 — DIREÇÃO DA CAMPANHA
→ definir a identidade narrativa persistente.
→ definir o foco inicial suficiente para começar.

PASSO 02 — CONFIGURAÇÃO DAS CADEIRAS
→ identificar quais autoridades precisam existir.
→ registrar quem executa cada uma.

PASSO 03 — FICHAS INICIAIS
→ criar somente as personagens que precisam existir no começo.

PASSO 04 — ESTADO INICIAL
→ registrar a situação concreta de abertura.

ESTRUTURA OPCIONAL
→ Temporada / Arco Preparado / Diretriz Fechada, quando a campanha se beneficiar disso.

DEPOIS
→ pareamento mínimo, quando necessário
→ conferir condições de início
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

A presença dessas pastas não obriga o uso de todas as estruturas narrativas possíveis. Um arquivo de roteiro, por exemplo, só recebe autoridade quando existir um arco preparado ativo.

O `README.md` da campanha começa com:

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: PASSO 01 — DIREÇÃO DA CAMPANHA
```

## PASSO 01 — Direção da Campanha

A Direção da Campanha define **que tipo de história esta campanha pretende acompanhar**.

Ela é o mínimo narrativo obrigatório antes do START.

Perguntar somente o necessário para compreender, quando relevante:

```text
que tipo de história queremos acompanhar?
qual é o foco inicial?
qual gênero e tom interessam?
que experiência queremos produzir?
que temas e relações devem receber espaço?
que tipos de conflito são compatíveis?
o que não deve dominar?
onde ou em que situação começamos?
que premissas gerais já são válidas?
```

Nem toda campanha precisa responder formalmente a todos esses itens. A Direção está suficiente quando permite ao Narrador distinguir desenvolvimento coerente de desvio arbitrário.

Registrar em:

```text
campanhas/<nome>/mestre/narrativa.md
```

Esse arquivo funciona como registro persistente da **Direção da Campanha**.

```text
DIREÇÃO DA CAMPANHA
→ identidade, foco e limites narrativos persistentes.

TRAMA PREPARADA
→ opcional.

TEMPORADA
→ opcional.
```

Uma trama secundária interessante não reescreve automaticamente a Direção da Campanha.

> **Direção não é roteiro. Ela informa para onde a história quer olhar sem decidir antecipadamente o que acontecerá.**

## PASSO 02 — Configuração das Cadeiras

Registrar no `README.md` da campanha quais autoridades existem e quem executa cada uma.

A Configuração das Cadeiras responde a duas perguntas diferentes:

```text
CADEIRA / FUNÇÃO
→ qual autoridade existe?

EXECUTOR
→ quem ou o que opera essa autoridade nesta campanha?
```

> **Cadeira define autoridade. Executor define quem a opera.**

Ela é um registro persistente de composição da campanha. Não é uma Mesa aberta nem um procedimento de auditoria.

Exemplo:

```text
## Configuração das Cadeiras

CADEIRA DE PERSONAGEM A
→ PERSONAGEM: <nome>
→ EXECUTOR: HUMANO

CADEIRA DE PERSONAGEM B
→ PERSONAGEM: <nome>
→ EXECUTOR: IA

CADEIRAS EVENTUAIS
→ EXECUTOR COMPARTILHADO: IA, quando necessário

OPOSITOR
→ EXECUTOR: IA

NARRADOR / JUIZ
→ EXECUTOR: IA
```

A configuração poderia igualmente usar outros arranjos:

```text
várias cadeiras executadas por humanos
uma pessoa executando mais de uma cadeira
uma IA executando várias cadeiras
Narrador humano
Narrador IA
outro participante executando uma função
```

Nenhuma dessas escolhas altera a autoridade definida pelo Tribunal.

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

Cada personagem com cadeira própria mantém conhecimento, intenção e soberania separados mesmo quando o mesmo executor opera várias cadeiras.

A palavra `Mesa` fica reservada ao procedimento temporário de alinhamento definido pelo Núcleo:

```text
DÚVIDA / DISCORDÂNCIA / CONFLITO REAL
→ abrir Mesa.

QUESTÃO RESOLVIDA
→ encerrar Mesa e voltar à ficção.
```

## PASSO 03 — Criar as Fichas Iniciais

Depois que a Direção e as autoridades necessárias estiverem claras, construir somente o elenco que já precisa de agência no início.

Não é necessário criar antecipadamente todas as pessoas que poderão existir na campanha.

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
→ qual Cadeira de Personagem possui autoridade sobre essa peça.

EXECUTOR
→ definido na Configuração das Cadeiras; indica quem ou o que opera essa autoridade.

FICHA
→ quem é e o que consegue fazer.
```

`CONTROLE` não deve ser preenchido com `HUMANO` ou `IA` como se fossem tipos de autoridade.

Exemplo:

```text
CONTROLE: CADEIRA DE PERSONAGEM A
```

Importância Narrativa não mede poder, não concede bônus e não altera autoridade.

`Patamar` pertence ao motor anterior e não faz parte da criação ativa.

Depois do elenco, seguir:

```text
jogador/1.3-criacao-da-ficha.md
```

A ficha é persistente e não depende da existência de uma temporada.

## Pareamento mínimo

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

## PASSO 04 — Estado Inicial

Depois das fichas necessárias e do pareamento relevante, registrar em:

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

O Estado Inicial é o primeiro Estado Atual da campanha. Ele registra o presente operacional, não um roteiro do futuro.

## Estrutura opcional — Temporada / Arco Preparado

Depois que existe uma Direção da Campanha, pode-se escolher preparar um arco antes do START ou em qualquer momento posterior.

```text
QUEREMOS UM ARCO PREPARADO?

SIM
→ seguir CRIACAO-DE-TEMPORADA.md.
→ registrar roteiro e Diretriz Fechada conforme esse módulo exigir.

NÃO
→ nenhuma Temporada é exigida.
→ começar a partir da Direção da Campanha + Fichas + Estado Inicial.
→ a campanha pode crescer de forma emergente.
```

Temporada e Diretriz Fechada são ferramentas de estrutura, não requisitos universais do motor.

```text
DIREÇÃO DA CAMPANHA
→ obrigatória.

TEMPORADA / ARCO PREPARADO
→ opcional.

DIRETRIZ FECHADA
→ existe quando a estrutura escolhida a exigir.
```

Quando uma Temporada estiver ativa, seu roteiro estabelece o tabuleiro estrutural daquele arco, não cenas futuras nem decisões voluntárias das personagens.

Quando não houver Temporada ativa, a Direção da Campanha continua sendo a referência para impedir crescimento arbitrário ou mudança invisível de proposta.

## START

Antes da primeira cena, conferir somente se a campanha consegue funcionar:

```text
estrutura existe?
Direção da Campanha foi aprovada?
elenco inicial necessário foi confirmado?
fichas necessárias estão aprovadas?
pareamento essencial foi resolvido, quando necessário?
Estado inicial está definido?
CONTROLE das peças está claro?
Configuração das Cadeiras registra os Executores?
se um Arco Preparado foi escolhido, sua preparação necessária está concluída?
```

Não exigir por padrão:

```text
Temporada ativa
problema de temporada
Diretriz Fechada
condição de encerramento de arco
```

Esses elementos só são requisitos quando a campanha escolheu usar a estrutura correspondente.

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

## Ciclos e arcos posteriores

A campanha e as fichas continuam existindo independentemente de temporadas.

```text
CAMPANHA
→ persistente.

DIREÇÃO DA CAMPANHA
→ persistente até mudança deliberada.

FICHAS
→ persistentes.

TEMPORADA / ARCO PREPARADO
→ opcional e renovável.
```

Quando um arco preparado termina:

```text
resolver o arco
→ escrever epílogo quando pertinente
→ consolidar mudanças
→ arquivar roteiro
→ perguntar “E agora?” quando isso fizer sentido para a execução
```

A campanha pode então criar outro arco preparado ou simplesmente continuar de modo emergente dentro de sua Direção.

## Criação emergente depois do START

Lacunas menores podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`.

Sempre vale:

```text
não fabricar vantagem ou obstáculo retroativamente para responder a uma ação já declarada
não mudar invisivelmente a Direção da Campanha
```

Quando houver uma Diretriz Fechada ativa, vale também:

```text
não alterar a Diretriz Fechada por improvisação
não introduzir retroativamente um novo problema estrutural que a torne falsa ou incompleta
```

## Regra final

> **Nova campanha exige Direção, autoridades necessárias, fichas iniciais suficientes e um Estado Inicial concreto. A Direção informa que história estamos tentando escrever sem precisar predeterminar uma trama. Temporadas, Arcos Preparados e Diretrizes Fechadas são estruturas opcionais: quando escolhidas, organizam um arco; quando ausentes, a campanha pode crescer emergentemente sem perder sua identidade narrativa.**
