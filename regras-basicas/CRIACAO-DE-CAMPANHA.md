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
→ Arco Preparado / Temporada, quando a campanha se beneficiar disso.
→ Diretriz Fechada somente quando esse arco possuir verdades que realmente precisam ser fechadas antes do jogo.
→ Opositor somente quando houver forças adversariais persistentes sem cadeira própria que se beneficiem de estratégia autônoma.

DEPOIS
→ pareamento mínimo, quando necessário
→ conferir condições de início
→ START
```

Não pedir novamente informação já fornecida.

## 1 — Estrutura da campanha

Depois que o nome for aprovado, materializar somente a estrutura universal:

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
└── livro/
```

Estruturas adicionais são materializadas somente quando realmente usadas.

```text
campanhas/<nome>/opositor/
→ criar somente se a função OPOSITOR estiver ativa
  e existir informação adversarial persistente que precise de registro próprio.
```

A presença das pastas universais também não obriga o uso de todas as estruturas narrativas possíveis. Um arquivo de roteiro, por exemplo, só recebe autoridade quando existir um arco preparado ativo.

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

DIRETRIZ FECHADA
→ opcional inclusive dentro de uma Temporada.
```

Uma trama secundária interessante não reescreve automaticamente a Direção da Campanha.

> **Direção não é roteiro. Ela informa para onde a história quer olhar sem decidir antecipadamente o que acontecerá.**

### Atenção não redefine a Direção

A atenção dada a um elemento durante a sessão pode justificar mais detalhe, compreensão, relação ou exploração, mas não muda automaticamente sua importância estrutural.

```text
ATENÇÃO EM CENA
→ pode aprofundar o que já está ali.

ATENÇÃO EM CENA
≠ mudança automática da Direção da Campanha.
```

Uma personagem pode conversar longamente com um NPC, explorar um local secundário ou investigar um detalhe menor sem que isso obrigue o Narrador a transformá-lo em novo eixo da campanha.

Se o interesse das cadeiras revelar vontade real de mudar o foco persistente, essa mudança deve acontecer por **Direção Autoral deliberada**, não como escalada invisível da improvisação.

> **A atenção pode aprofundar um elemento; não concede, por si só, autoridade para ampliar sua importância estrutural.**

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
→ ATIVO: NÃO

NARRADOR / JUIZ
→ EXECUTOR: IA
```

Se a campanha realmente se beneficiar de uma função adversarial persistente:

```text
OPOSITOR
→ ATIVO: SIM
→ EXECUTOR: <humano, IA ou outro participante>
→ ESCOPO: <forças adversariais sem cadeira própria que representa>
```

A configuração poderia igualmente usar outros arranjos:

```text
várias cadeiras executadas por humanos
uma pessoa executando mais de uma cadeira
uma IA executando várias cadeiras
Narrador humano
Narrador IA
outro participante executando uma função
campanha sem Opositor
campanha que ativa Opositor somente depois que uma força adversarial persistente surge
```

Nenhuma dessas escolhas altera a autoridade definida pelo Tribunal.

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

Cada personagem com cadeira própria mantém conhecimento, intenção e soberania separados mesmo quando o mesmo executor opera várias cadeiras.

A palavra `Mesa` fica reservada ao procedimento temporário de alinhamento definido pelo Núcleo.

### Opositor é opcional

A existência de conflito, dificuldade ou antagonismo não exige uma função `OPOSITOR` ativa.

```text
CONFLITO ENTRE PERSONAGENS COM CADEIRA
→ cada cadeira continua decidindo sua própria personagem.

PERIGO AMBIENTAL OU PROCESSO IMPESSOAL
→ pertence ao mundo, Estado e julgamento causal.

NPC COM AGÊNCIA PRÓPRIA
→ pode receber cadeira própria ou eventual quando necessário.

FORÇA ADVERSARIAL PERSISTENTE SEM CADEIRA PRÓPRIA
→ pode justificar ativar OPOSITOR.
```

Ativar Opositor quando uma ou mais forças adversariais persistentes se beneficiarem de planejamento, recursos, objetivos e decisões estratégicas próprias sem que cada peça possua cadeira dedicada.

Não ativar apenas porque a história possui problemas.

> **Opositor organiza oposição persistente quando ela precisa de uma autoridade própria; não é a fonte obrigatória de todo problema da ficção.**

Se a necessidade surgir depois do START, a Configuração das Cadeiras pode ser atualizada prospectivamente e a função passa a existir a partir dali. Isso não autoriza inventar retroativamente preparação ou recursos adversariais.

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
→ registrar somente a preparação realmente necessária no Roteiro.
→ criar Diretriz Fechada apenas se houver verdades que precisem existir e permanecer fixas antes de serem descobertas, enfrentadas ou testadas.

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
→ opcional dentro do Arco Preparado.
```

Quando uma Temporada estiver ativa, seu Roteiro registra a preparação daquele arco, não cenas futuras nem decisões voluntárias das personagens.

Quando houver Diretriz Fechada, ela protege somente as verdades estruturais explicitamente fechadas.

Quando não houver Diretriz Fechada, o arco ainda respeita Direção, cânone, Estado e proibição de retroatividade oportunista.

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
se OPOSITOR estiver ativo, seu Executor e Escopo estão claros?
se um Arco Preparado foi escolhido, sua preparação necessária está concluída?
se esse arco realmente precisa de Diretriz Fechada, ela foi registrada?
```

Não exigir por padrão:

```text
Opositor ativo
pasta opositor/
Temporada ativa
problema de temporada
Diretriz Fechada
condição de encerramento de arco
```

Esses elementos só são requisitos quando a estrutura escolhida realmente os utiliza.

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

OPOSITOR
→ opcional e ativável quando surgir necessidade legítima.

TEMPORADA / ARCO PREPARADO
→ opcional e renovável.

DIRETRIZ FECHADA
→ existe somente enquanto alguma estrutura ativa precisar dela.
```

Quando um arco preparado termina, consolidar mudanças e decidir se haverá outro arco preparado ou continuidade emergente.

## Criação emergente depois do START

Lacunas menores podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`.

Sempre vale:

```text
não fabricar vantagem ou obstáculo retroativamente para responder a uma ação já declarada
não mudar invisivelmente a Direção da Campanha
não contradizer fatos já estabelecidos
```

Quando houver uma Diretriz Fechada ativa, vale também:

```text
não alterar por improvisação as verdades que foram fechadas
não introduzir retroativamente estrutura que torne essas verdades falsas ou incompletas
```

## Regra final

> **Nova campanha exige Direção, autoridades necessárias, fichas iniciais suficientes e um Estado Inicial concreto. A Direção informa que história estamos tentando escrever sem precisar predeterminar uma trama. Opositor, Temporadas e Diretrizes Fechadas são estruturas opcionais: o Opositor só é ativado quando forças adversariais persistentes sem cadeira própria realmente precisam de uma autoridade estratégica; Temporadas só existem quando se deseja um Arco Preparado; e a Diretriz Fechada só aparece quando certas verdades precisam ser fixadas antes de serem descobertas, enfrentadas ou testadas.**