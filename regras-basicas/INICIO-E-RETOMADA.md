# Início e Retomada

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define como iniciar ou retomar uma campanha usando `regras-basicas/` sem reativar o motor anterior.

> **Carregar somente o necessário para reconstruir as cadeiras, a realidade presente, a Direção da Campanha e o primeiro ponto ainda aberto.**

## Entrada

No primeiro contato:

```text
ler regras-basicas/README.md
→ compreender Núcleo, Jogador, Mestre, Opositor e Registro
→ Nova campanha ou Continuar?
```

Não reler todos os arquivos em toda resposta. Durante o jogo, consultar somente a fonte específica que realmente se tornou necessária.

## Nova campanha

Seguir:

```text
CRIACAO-DE-CAMPANHA.md
```

A criação universal exige:

```text
PASSO 01 — Direção da Campanha
PASSO 02 — Configuração das Cadeiras
PASSO 03 — Fichas Iniciais
PASSO 04 — Estado Inicial
```

Depois disso, quando desejado:

```text
ESTRUTURA OPCIONAL
→ Temporada / Arco Preparado
→ Diretriz Fechada somente quando esse arco realmente precisar
→ seguir CRIACAO-DE-TEMPORADA.md
```

A ficção começa somente depois do START.

> **Temporada não é requisito universal de início. Direção da Campanha é. Diretriz Fechada também não é requisito universal de uma Temporada.**

## Continuar campanha

Abrir primeiro:

```text
campanhas/<nome>/README.md
```

Depois carregar, por padrão:

```text
mestre/narrativa.md
+
estado/atual.md
+
fichas das personagens atualmente relevantes
```

Carregar também:

```text
mestre/roteiro.md
```

**somente quando houver uma Temporada / Arco Preparado ativo**.

Dentro do Roteiro, carregar Diretriz Fechada somente quando ela estiver explicitamente ativa para aquele arco.

Essas fontes têm funções diferentes:

```text
DIREÇÃO DA CAMPANHA / NARRATIVA
→ identidade, foco e limites narrativos persistentes.

ROTEIRO DA TEMPORADA
→ preparação concreta de um Arco Preparado ativo, quando existir.

DIRETRIZ FECHADA
→ subconjunto opcional do Roteiro que protege verdades estruturais previamente fixadas.

FICHA
→ quem a personagem é, o que sabe, consegue fazer e possui legitimamente.

ESTADO DA CAMPANHA
→ realidade global presente necessária para continuar.

LIVRO / MUNDO / OPOSITOR / OUTRAS FONTES
→ contexto consultado somente quando necessário.
```

O `README.md` da campanha também preserva, quando aplicável, a **Configuração das Cadeiras**: quais autoridades existem e quem as executa.

Não pedir novamente informação já registrada em fonte canônica.

## Campanha com ou sem Arco Preparado

Antes da retomada, identificar qual estrutura está ativa.

```text
SEM ARCO PREPARADO ATIVO
→ Direção da Campanha continua sendo a referência estrutural persistente.
→ não inventar um roteiro ausente.
→ continuar a partir do Estado e das decisões das cadeiras.

COM ARCO PREPARADO ATIVO
→ carregar também o Roteiro.
→ se houver Diretriz Fechada ativa, carregar e respeitar somente as verdades que ela fechou.
→ se não houver, não inventar uma Diretriz Fechada retroativamente.
```

A ausência de Temporada não significa ausência de direção.

A ausência de Diretriz Fechada também não significa ausência de cânone ou continuidade.

```text
SEM TEMPORADA
≠
SEM DIREÇÃO

SEM DIRETRIZ FECHADA
≠
SEM LIMITES
```

## Reancoragem

Antes de voltar à ficção depois de perda importante de contexto, novo chat, checkpoint ou retomada de campanha pronta, executar:

```text
registro/reancoragem-operacional.md
```

Fluxo:

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR
→ reconstruir Configuração das Cadeiras e autoridades
→ reconstruir a Direção da Campanha
→ reconstruir a realidade presente
→ carregar Arco Preparado somente se estiver ativo
→ carregar Diretriz Fechada somente se existir nesse arco
→ separar pacotes das cadeiras
→ restaurar intenções e processos ainda vivos
→ identificar o primeiro ponto aberto
→ SÓ ENTÃO CONTINUAR A FICÇÃO
```

Reancoragem não significa recitar regras ao usuário.

## O Estado Atual na retomada

`campanhas/<nome>/estado/atual.md` é a fonte canônica global do presente.

Na retomada ele deve permitir responder rapidamente:

```text
quando estamos?
onde estamos?
quem está presente?
onde estão as peças relevantes?
que condições temporárias importam?
que efeitos ou transformações continuam ativos?
que Equipamentos ou Recursos estão indisponíveis?
que intenções persistem?
que processos ou prazos estão prestes a interferir?
qual foi o último fato estabelecido?
qual é a primeira decisão ainda aberta?
a qual cadeira essa decisão pertence?
```

Não presumir campos universais de `Vida`, `Mente` ou `Mana`.

```text
CONDIÇÃO / RECURSO / CUSTO ESPECÍFICO EXISTE
→ acompanhar conforme a fonte que o definiu.

NÃO EXISTE FONTE QUE O DEFINA
→ não recriar o mecanismo por hábito.
```

O bloco `Estado Atual` dentro de cada ficha é apenas o recorte pessoal relevante para aquela cadeira.

```text
ESTADO GLOBAL
→ Narrador pode consultar para reconstruir a realidade.

CADEIRA
→ recebe somente seu recorte legítimo e fatos que pode conhecer.
```

## Separação das cadeiras

Um mesmo executor pode operar várias cadeiras, mas cada uma funciona somente com:

```text
sua própria ficha
+
seu recorte pessoal do Estado
+
seu conhecimento legítimo
+
fatos da cena que pode perceber ou conhecer
+
sua intenção atual, quando houver
```

```text
EXECUTOR SABE
≠
PERSONAGEM SABE
```

Comparações técnicas pertencem ao Narrador/Juiz e, quando pertinente, ao Opositor.

## Configuração das Cadeiras e Mesa

Não confundir composição persistente com procedimento temporário.

```text
CONFIGURAÇÃO DAS CADEIRAS
→ quais autoridades existem na campanha e quem as executa.
→ deve ser reconstruída na retomada.

TRIBUNAL
→ estrutura que define essas autoridades e seus limites.

MESA
→ só abre quando existe dúvida, discordância, direção compartilhada ou conflito real.
→ não é uma etapa permanente da retomada.
```

Se não houver questão pendente, nenhuma Mesa precisa ser aberta para continuar.

## Campanha em criação

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar do ponto registrado
→ não iniciar ficção.
```

## Entre Arcos Preparados

Se uma Temporada anterior terminou e ainda não existe novo roteiro ativo:

```text
→ consultar epílogo e fontes consolidadas quando relevantes
→ manter a Direção da Campanha
→ escolher entre continuidade emergente ou novo Arco Preparado
→ não criar automaticamente uma nova Temporada
```

Um problema ainda aberto não obriga que o próximo arco seja sobre ele.

## Campanha pronta

```text
CRIAÇÃO: CONCLUÍDA
→ carregar fontes mínimas
→ reconstruir Configuração das Cadeiras e autoridades necessárias
→ carregar Direção da Campanha
→ carregar Roteiro somente se existir Arco Preparado ativo
→ carregar Diretriz Fechada somente se existir nesse Roteiro
→ carregar Estado da Campanha
→ carregar fichas relevantes
→ restaurar intenções e processos pertinentes
→ reancorar
→ identificar o primeiro ponto aberto
→ continuar exatamente dali
```

## Durante a sessão

O fluxo normal não muda porque a campanha foi retomada:

```text
CADEIRAS DECIDEM
→ fatos relevantes são identificados
→ autoridades afetadas são reconhecidas
→ Opositor apresenta resistência legítima quando pertinente
→ Narrador/Juiz julga
→ Mesa somente se houver dúvida ou conflito real
→ narrar
→ quando surgir nova decisão voluntária, devolvê-la à cadeira correta
```

A forma de continuidade depende do executor dessa cadeira:

```text
EXECUTOR PODE DECIDIR NO MESMO FLUXO
→ executar a cadeira separadamente e continuar.

EXECUTOR DEPENDE DE ENTRADA EXTERNA
→ apresentar a situação e aguardar essa entrada.
```

O Narrador não escolhe a decisão apenas para evitar uma interrupção operacional.

Uma intenção longa não congela as outras cadeiras nem os processos já estabelecidos.

Uma cena de combate, investigação, romance, exploração ou cotidiano continua usando a mesma estrutura de autoria. Nenhuma lente ativa automaticamente um motor mecânico legado.

## Direção durante o jogo

A Direção da Campanha continua válida mesmo quando não existe Roteiro ativo.

Ela serve para julgar se um desenvolvimento é compatível com a história que a campanha pretende acompanhar.

```text
CURIOSIDADE DE CENA
≠ autorização automática para mudar a identidade da campanha.

AUSÊNCIA DE ROTEIRO
≠ permissão para criar qualquer trama.

AUSÊNCIA DE DIRETRIZ FECHADA
≠ permissão para alterar retroativamente a realidade.
```

Quando houver Direção Autoral nova que realmente altere a identidade da campanha, consolidar a mudança deliberadamente em `mestre/narrativa.md`.

Quando a intenção for apenas preparar um arco específico sem mudar a identidade persistente, usar `CRIACAO-DE-TEMPORADA.md`.

## Fechar capítulo

O comando:

```text
fechar o capítulo
```

segue `registro/fechar-capitulo.md`.

Ele funciona como checkpoint:

```text
SALVAR
→ capítulo no Livro.

ATUALIZAR
→ Estado e fontes afetadas.

RESET OPERACIONAL
→ ruído transitório deixa de ser base principal.

RECARREGAR
→ fontes essenciais.

REANCORAR
→ reconstruir Configuração das Cadeiras, autoridades e realidade presente.

CONTINUAR
→ a partir do Estado consolidado.
```

Se um Arco Preparado também terminou, aplicar seu encerramento antes de decidir como a campanha continuará.

## O que não reativar na retomada

Retomar uma campanha antiga não torna ativos por compatibilidade:

```text
Atributo + Perícia
2d6 universal
Potência de Execução
Defesa ou Resistência matemáticas
Vida universal
Mente universal
Mana universal
rodadas fixas
iniciativa numérica obrigatória
```

Se uma campanha histórica possui um recurso particular que continua canonicamente válido, ele deve ser reinterpretado e registrado explicitamente antes de ser usado como regra ativa.

> **Antigo registro não é autorização para reconstruir o motor antigo.**

## Regra final

> **Para começar ou retomar uma campanha, reconstruir primeiro sua Direção, Configuração das Cadeiras, fichas, Estado global, conhecimentos, intenções e processos. Temporada só entra quando existir um Arco Preparado ativo; Diretriz Fechada só entra quando esse arco possuir verdades que realmente precisem estar fixadas. Sua ausência não remove a Direção, o cânone nem a proibição de retroatividade. Toda nova decisão voluntária retorna à cadeira correta.**
