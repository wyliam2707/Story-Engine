# Criação de Campanha

Status: REFORMULAÇÃO ATIVA

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **Toda campanha precisa de uma Direção antes do START. A Direção define que tipo de história estamos tentando escrever; o Diretor pode depois deixar a ficção emergir ou fechar trajetórias e resultados quando decidir fazê-lo.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
PASSO 01 — DIREÇÃO DA CAMPANHA
→ definir identidade narrativa persistente.
→ definir foco inicial suficiente para começar.

PASSO 02 — CONFIGURAÇÃO DAS AUTORIDADES
→ identificar Diretor, Cadeiras, Narrador e funções opcionais.
→ registrar quem executa cada uma.

PASSO 03 — FICHAS INICIAIS
→ criar somente as personagens que precisam existir no começo.

PASSO 04 — ESTADO INICIAL
→ registrar a situação concreta de abertura.

ESTRUTURA OPCIONAL
→ Arco Preparado / Temporada, quando útil.
→ Diretriz Fechada somente quando esse arco possuir verdades estruturais que precisam existir antes de serem descobertas ou testadas.
→ Opositor somente quando forças adversariais persistentes sem cadeira própria precisarem de autoridade estratégica.

DEPOIS
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
→ criar somente se OPOSITOR estiver ativo
  e existir informação adversarial persistente que precise de registro próprio.
```

## PASSO 01 — Direção da Campanha

A Direção da Campanha define **que tipo de história esta campanha pretende acompanhar persistentemente**.

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

Nem toda campanha precisa responder formalmente a todos esses itens.

Registrar em:

```text
campanhas/<nome>/mestre/narrativa.md
```

```text
DIREÇÃO DA CAMPANHA
→ identidade, foco e limites narrativos persistentes.

DIREÇÃO DO DIRETOR DURANTE O JOGO
→ pode orientar ou fechar trajetórias, condições e resultados específicos.

TRAMA PREPARADA / TEMPORADA
→ opcional.

DIRETRIZ FECHADA
→ opcional dentro de um Arco Preparado.
```

A Direção da Campanha não precisa predeterminar uma trama para existir.

Isso não significa proibir o Diretor de determinar algo posteriormente.

```text
DIREÇÃO DA CAMPANHA
→ referência persistente ampla.

DIREÇÃO VINCULANTE DO DIRETOR
→ intervenção autoral específica quando ele decidir exercê-la.
```

> **A campanha pode permanecer emergente sem tornar o Diretor incapaz de dirigir.**

### Atenção não redefine a Direção

A atenção dada a um elemento durante a sessão pode justificar mais detalhe, compreensão, relação ou exploração, mas não muda automaticamente sua importância estrutural.

```text
ATENÇÃO EM CENA
→ pode aprofundar o que já está ali.

ATENÇÃO EM CENA
≠ mudança automática da Direção da Campanha.
```

Se o interesse revelar vontade real de mudar o foco persistente, o Diretor pode deliberadamente alterar a Direção da Campanha.

## PASSO 02 — Configuração das Autoridades

Registrar no `README.md` da campanha quais autoridades existem e quem executa cada uma.

```text
AUTORIDADE / FUNÇÃO
→ o que pode decidir.

EXECUTOR
→ quem ou o que opera essa autoridade nesta campanha.
```

Exemplo:

```text
DIRETOR
→ EXECUTOR: HUMANO

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

O mesmo humano pode executar o Diretor e uma Cadeira de Personagem sem fundir as funções.

```text
DIRETOR
≠
CADEIRA DA PERSONAGEM DO DIRETOR
```

Da mesma forma:

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

Uma campanha pode usar outros arranjos:

```text
várias cadeiras executadas por humanos
uma pessoa executando mais de uma cadeira
uma IA executando várias cadeiras
Narrador humano
Narrador IA
outro participante executando função
campanha sem Opositor
campanha que ativa Opositor depois
```

Nenhuma dessas escolhas altera a autoridade definida pelo Tribunal.

A palavra `Mesa` fica reservada ao procedimento temporário de auditoria e alinhamento.

### Opositor é opcional

A existência de conflito, dificuldade ou antagonismo não exige `OPOSITOR` ativo.

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

Ativar Opositor prospectivamente.

```text
ATIVAR AGORA
≠ inventar que planos ou recursos sempre existiram.
```

## PASSO 03 — Criar as Fichas Iniciais

Depois que Direção e autoridades necessárias estiverem claras, construir somente o elenco que já precisa de agência no início.

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
→ definido na Configuração das Autoridades.

FICHA
→ quem é e o que consegue fazer.
```

`CONTROLE` não deve ser preenchido com `HUMANO` ou `IA`.

Exemplo:

```text
CONTROLE: CADEIRA DE PERSONAGEM A
```

Importância Narrativa não mede poder, não concede bônus e não altera autoridade.

`Patamar` pertence ao motor anterior.

Depois do elenco, seguir:

```text
jogador/1.3-criacao-da-ficha.md
```

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

Se uma lacuna puder surgir naturalmente em cena sem contradição, não preenchê-la antes por obrigação.

## PASSO 04 — Estado Inicial

Registrar em:

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

O Estado Inicial registra o presente operacional, não um roteiro do futuro.

## Estrutura opcional — Temporada / Arco Preparado

Depois que existe Direção da Campanha, pode-se preparar um arco antes do START ou posteriormente.

```text
QUEREMOS UM ARCO PREPARADO?

SIM
→ seguir CRIACAO-DE-TEMPORADA.md.
→ registrar somente a preparação necessária.
→ criar Diretriz Fechada apenas se houver verdades que precisem existir antes de serem descobertas ou testadas.

NÃO
→ começar a partir de Direção + Fichas + Estado.
→ a campanha pode crescer emergentemente.
```

Temporada e Diretriz Fechada são ferramentas de estrutura, não limites à autoridade autoral do Diretor.

```text
ROTEIRO
→ não predetermina sozinho decisões das personagens.

DIRETOR
→ pode deliberadamente fechar uma trajetória ou resultado durante a condução da obra.
```

## START

Antes da primeira cena, conferir somente se a campanha consegue funcionar:

```text
estrutura existe?
Direção da Campanha foi aprovada?
Diretor está identificado?
Configuração das autoridades está clara?
elenco inicial necessário foi confirmado?
fichas necessárias estão aprovadas?
Estado inicial está definido?
se OPOSITOR estiver ativo, Executor e Escopo estão claros?
se um Arco Preparado foi escolhido, sua preparação necessária está concluída?
```

Não exigir por padrão:

```text
Opositor ativo
Temporada ativa
Diretriz Fechada
problema central
condição de encerramento de arco
```

Se faltar algo essencial:

```text
CRIAÇÃO: EM ANDAMENTO
→ registrar etapa
→ não iniciar ficção.
```

Se estiver pronto:

```text
CRIAÇÃO: CONCLUÍDA
→ seguir INICIO-E-RETOMADA.md
→ abrir a primeira cena.
```

## Criação emergente depois do START

Lacunas menores podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`.

Sempre vale para autoridades inferiores:

```text
não fabricar vantagem ou obstáculo retroativamente
não mudar invisivelmente a Direção da Campanha
não contradizer fatos estabelecidos por conveniência
```

O Diretor pode conscientemente alterar a direção ou um fato mediante determinação/correção explícita. O sistema pode apontar as consequências, mas não existe para impedi-lo de dirigir a própria obra.

## Regra final

> **Nova campanha exige Direção da Campanha, Diretor identificado, autoridades necessárias, fichas suficientes e Estado Inicial concreto. A história pode crescer de forma emergente porque qualquer cadeira pode iniciar ideias dentro de sua autoridade, mas o Diretor continua podendo orientar ou fechar trajetórias e resultados. Opositor, Temporadas e Diretrizes Fechadas permanecem estruturas opcionais.**