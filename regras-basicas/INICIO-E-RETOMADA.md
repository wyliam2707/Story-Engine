# Início e Retomada

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define como iniciar ou retomar uma campanha usando `regras-basicas/` sem reativar o motor anterior.

> **Carregar somente o necessário para reconstruir a mesa, a realidade presente e o primeiro ponto ainda aberto.**

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

A criação segue:

```text
PASSO 01 — Narrativa da Campanha
PASSO 02 — Temporada
PASSO 03 — Fichas
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
mestre/roteiro.md
+
estado/atual.md
+
fichas das personagens atualmente relevantes
```

Essas fontes têm funções diferentes:

```text
NARRATIVA DA CAMPANHA
→ identidade persistente.

ROTEIRO DA TEMPORADA
→ tabuleiro estrutural do arco ativo.

FICHA
→ quem a personagem é, o que sabe, consegue fazer e possui legitimamente.

ESTADO DA CAMPANHA
→ realidade global presente necessária para continuar.

LIVRO / MUNDO / OPOSITOR / OUTRAS FONTES
→ contexto consultado somente quando necessário.
```

Não pedir novamente informação já registrada em fonte canônica.

## Reancoragem

Antes de voltar à ficção depois de perda importante de contexto, novo chat, checkpoint ou retomada de campanha pronta, executar:

```text
registro/reancoragem-operacional.md
```

Fluxo:

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR
→ reconstruir autoridades e realidade presente
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
qual é a primeira decisão humana ainda aberta?
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

Uma única IA técnica pode executar várias cadeiras, mas cada uma opera somente com:

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
IA TÉCNICA SABE
≠
PERSONAGEM SABE
```

Comparações técnicas pertencem ao Narrador/Juiz e, quando pertinente, ao Opositor.

## Campanha em criação

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar do ponto registrado
→ não iniciar ficção.
```

## Entre temporadas

Se a temporada anterior terminou e ainda não existe um novo roteiro ativo:

```text
→ consultar epílogo e fontes consolidadas
→ retomar ou fazer a pergunta “E agora?”
→ não escolher a próxima temporada automaticamente
```

Um problema ainda aberto não obriga que o próximo arco seja sobre ele.

## Campanha pronta

```text
CRIAÇÃO: CONCLUÍDA
→ carregar fontes mínimas
→ reconstruir cadeiras necessárias
→ carregar Narrativa
→ carregar Roteiro ativo
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
→ parar na primeira nova escolha voluntária humana
```

Uma intenção longa não congela as outras cadeiras nem os processos já estabelecidos.

Uma cena de combate, investigação, romance, exploração ou cotidiano continua usando a mesma estrutura de autoria. Nenhuma lente ativa automaticamente um motor mecânico legado.

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
→ reconstruir a mesa funcional.

CONTINUAR
→ a partir do Estado consolidado.
```

Se a temporada também terminou, o fechamento de temporada substitui a continuação normal e termina em **“E agora?”**.

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

> **Para começar ou retomar uma campanha pronta, reconstruir autoridades, fichas, Estado global, conhecimento por cadeira, intenções e processos antes da nova ficção. Vida, Mente e Mana não são campos universais de retomada; somente condições, recursos e custos definidos por fontes canônicas específicas continuam sendo acompanhados.**