# Início e Retomada

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define como iniciar ou retomar uma campanha usando `regras-basicas/` sem reativar o motor anterior.

> **Carregar somente o necessário para reconstruir o Diretor, as cadeiras, a realidade presente, a Direção da Campanha e o primeiro ponto ainda aberto.**

## Entrada

No primeiro contato:

```text
ler regras-basicas/README.md
→ compreender Diretor, Núcleo, Jogador, Mestre, Opositor e Registro
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
PASSO 02 — Configuração das Autoridades
PASSO 03 — Fichas Iniciais
PASSO 04 — Estado Inicial
```

Depois disso, quando desejado:

```text
ESTRUTURA OPCIONAL
→ Temporada / Arco Preparado
→ Diretriz Fechada somente quando o arco precisar
→ seguir CRIACAO-DE-TEMPORADA.md
```

A ficção começa somente depois do START.

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

somente quando houver Temporada / Arco Preparado ativo.

Dentro do Roteiro, carregar Diretriz Fechada somente quando estiver explicitamente ativa.

Essas fontes têm funções diferentes:

```text
DIREÇÃO DA CAMPANHA / NARRATIVA
→ identidade, foco e limites narrativos persistentes.

DIREÇÃO DO DIRETOR
→ intervenção autoral atual quando houver.

ROTEIRO DA TEMPORADA
→ preparação concreta do Arco Preparado ativo.

DIRETRIZ FECHADA
→ subconjunto opcional do Roteiro que protege verdades estruturais.

FICHA
→ quem a personagem é, o que sabe, consegue fazer e possui legitimamente.

ESTADO DA CAMPANHA
→ realidade global presente necessária para continuar.

LIVRO / MUNDO / OPOSITOR / OUTRAS FONTES
→ contexto consultado somente quando necessário.
```

O `README.md` da campanha preserva a Configuração das Autoridades: Diretor, cadeiras, Narrador, Opositor quando ativo e executores.

Não pedir novamente informação já registrada em fonte canônica.

## Campanha com ou sem Arco Preparado

```text
SEM ARCO PREPARADO ATIVO
→ Direção da Campanha continua sendo referência estrutural.
→ não inventar Roteiro ausente.
→ continuar a partir do Estado, das cadeiras e das Direções atuais do Diretor.

COM ARCO PREPARADO ATIVO
→ carregar também o Roteiro.
→ se houver Diretriz Fechada, respeitar as verdades que ela protege.
→ não inventar Diretriz Fechada retroativamente.
```

A ausência de Temporada não significa ausência de direção.

A ausência de Diretriz Fechada não significa ausência de cânone.

## Reancoragem

Antes de voltar à ficção depois de perda importante de contexto, novo chat, checkpoint ou retomada:

```text
registro/reancoragem-operacional.md
```

Fluxo:

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR DIRETOR E CONFIGURAÇÃO DAS AUTORIDADES
→ reconstruir Direção da Campanha
→ reconstruir realidade presente
→ carregar Arco Preparado somente se ativo
→ separar pacotes das cadeiras
→ restaurar intenções e processos vivos
→ identificar Direção autoral pendente, se houver
→ identificar primeiro ponto aberto
→ SÓ ENTÃO CONTINUAR A FICÇÃO
```

Reancoragem não significa recitar regras ao usuário.

## O Estado Atual na retomada

`campanhas/<nome>/estado/atual.md` é a fonte canônica global do presente.

Na retomada ele deve permitir responder:

```text
quando estamos?
onde estamos?
quem está presente?
onde estão as peças relevantes?
que condições temporárias importam?
que efeitos ou transformações continuam ativos?
que equipamentos ou recursos estão indisponíveis?
que intenções persistem?
que processos ou prazos estão prestes a interferir?
qual foi o último fato estabelecido?
qual é a primeira decisão ainda aberta?
a qual cadeira essa decisão pertence?
```

Não presumir `Vida`, `Mente` ou `Mana` universais.

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

Isso inclui Direção do Diretor.

```text
EXECUTOR CONHECE RESULTADO FECHADO
≠
PERSONAGEM CONHECE SEU DESTINO
```

## Diretor na retomada

Reconstruir também:

```text
quem exerce a função de Diretor
que Direções persistentes continuam válidas
que determinações específicas ainda limitam a cena, se houver
que pedidos de auditoria ou análise ficaram pendentes
```

Uma Direção vinculante não deve ser esquecida durante a retomada.

Ao mesmo tempo, não ampliar seu escopo além do que foi efetivamente determinado.

> **Reancorar a Direção significa preservar o que foi fechado sem inventar fechamento novo.**

## Configuração das Autoridades e Mesa

Não confundir composição persistente com procedimento temporário.

```text
CONFIGURAÇÃO DAS AUTORIDADES
→ Diretor, cadeiras, funções e executores.

TRIBUNAL
→ define os limites dessas autoridades.

MESA
→ só abre quando existe dúvida, objeção, análise ou conflito real.
```

Mesa não é etapa permanente da retomada.

## Campanha em criação

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar do ponto registrado
→ não iniciar ficção.
```

## Entre Arcos Preparados

Se uma Temporada terminou e não existe novo Roteiro ativo:

```text
→ consultar epílogo e fontes consolidadas quando relevantes
→ manter Direção da Campanha
→ aguardar ou aplicar a Direção atual do Diretor
→ escolher entre continuidade emergente ou novo Arco Preparado
→ não criar automaticamente nova Temporada
```

## Durante a sessão

Fluxo normal:

```text
DIRETOR PODE ORIENTAR OU DEIXAR ABERTO
→ CADEIRAS DECIDEM
→ fatos relevantes são identificados
→ perguntar se os fatos determinam
→ reconhecer somente decisões realmente disponíveis
→ Opositor apresenta resistência legítima quando pertinente
→ Narrador / Juiz julga
→ Mesa somente se houver dúvida, auditoria ou conflito real
→ narrar
→ devolver nova decisão à cadeira correta
```

Se o executor dessa cadeira depende de entrada externa:

```text
apresentar situação
→ aguardar entrada
```

O Narrador não escolhe a decisão apenas para evitar interrupção operacional.

## Pedido do Diretor durante a retomada

Texto em `[ ]` pertence à camada autoral.

```text
[confira nos livros]
→ auditar antes de continuar.

[justifique essa decisão]
→ analisar antes de continuar.

[quero que a cena siga para X]
→ aplicar Direção vinculante no escopo determinado.
```

Não tratar todo `[ ]` como simples sugestão.

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
→ reconstruir Diretor, autoridades e realidade presente.

CONTINUAR
→ a partir do Estado consolidado.
```

## O que não reativar

Retomar campanha antiga não torna ativos:

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

> **Antigo registro não é autorização para reconstruir o motor antigo.**

## Regra final

> **Para começar ou retomar uma campanha, reconstruir primeiro Diretor, Direção, Configuração das Autoridades, fichas, Estado global, conhecimentos, intenções e processos. Temporada e Diretriz Fechada só entram quando ativas. Direções vinculantes continuam válidas no escopo em que foram determinadas; pedidos de auditoria precisam ser resolvidos antes de a ficção avançar; e toda nova decisão voluntária retorna à cadeira que realmente possui oportunidade de decidir.**