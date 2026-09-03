# Estado Atual

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define a função de:

```text
campanhas/<nome>/estado/atual.md
```

`estado/atual.md` é a **fonte canônica global da realidade presente da campanha** e pode preservar **Direções Autorais Ativas** que ainda limitam a continuação.

Ele responde:

> **Se a campanha continuar agora, o que precisa estar imediatamente verdadeiro — e que limite autoral ainda precisa ser respeitado — para a próxima janela começar no lugar correto?**

## Princípio central

A campanha possui um único presente compartilhado.

```text
campanhas/<nome>/estado/atual.md
→ verdade canônica global do presente.
→ limites autorais locais ainda ativos, quando houver.

Ficha da personagem / Estado Atual
→ recorte pessoal e operacional daquela personagem.
```

> **O Estado da Campanha define o presente. O Estado da ficha carrega somente a parte desse presente que precisa acompanhar aquela personagem.**

## Estado global da campanha

Registrar somente fatos atuais úteis para continuidade, como:

```text
momento ou data atual
local ou locais relevantes
quem está presente
posição importante das peças
condições temporárias relevantes
transformações em curso
efeitos ativos
equipamentos ou recursos indisponíveis
intenções persistentes
ações interrompidas
processos em andamento
prazos próximos
consequências recentes que ainda alteram a situação
primeiro ponto ainda aberto
```

Nem todo campo precisa existir sempre.

```text
ACONTECEU E AINDA MUDA O PRESENTE
→ Estado Atual.

ACONTECEU MAS JÁ NÃO ALTERA O PRESENTE
→ Livro, Histórico ou outra fonte.
```

## Direções Autorais Ativas

Uma Direção do Diretor entra no Estado somente quando **ainda precisa ser lembrada para a continuação**.

Exemplos:

```text
DIRETOR FECHOU RESULTADO DE CONFRONTO AINDA EM CURSO
→ registrar.

DIRETOR DEFINIU TRAJETÓRIA QUE AINDA NÃO TERMINOU
→ registrar.

DIREÇÃO JÁ FOI COMPLETAMENTE CONSUMADA
→ não manter como pendência.
```

Forma sugerida:

```text
## Direções Autorais Ativas

- Direção: A perde o confronto atual.
  Escopo fechado: resultado do confronto.
  Permanece aberto: ações intermediárias, falas e método específico da derrota.
```

Outro exemplo:

```text
- Direção: X provoca Y porque o considera indigno até a cena alcançar o confronto definido pelo Diretor.
  Escopo fechado: trajetória e motivação indicada para a provocação.
  Permanece aberto: formulação das falas, reação de Y, detalhes intermediários não determinados.
```

> **Registrar o escopo fechado e o espaço aberto evita que a reancoragem esqueça ou amplie a Direção.**

### Direção ativa não é fato consumado

```text
DIREÇÃO
→ limite autoral sobre o que ainda deve acontecer.

FATO PRESENTE
→ o que já aconteceu ou já é verdade agora.
```

Não escrever uma Direção futura no Livro como se já tivesse acontecido.

Quando a Direção for consumada:

```text
→ remover de Direções Autorais Ativas.
→ registrar o acontecimento real nas fontes normais.
```

### Direção não é conhecimento da personagem

O Estado global pode conter Direção Autoral Ativa sem transmiti-la às cadeiras.

```text
ESTADO / EXECUTOR SABE
≠
PERSONAGEM SABE
```

A cadeira recebe somente os fatos que pode conhecer e sua própria situação.

## Estado local da personagem

O bloco `Estado Atual` da ficha é recorte pessoal.

Pode registrar:

```text
ferida
exausta
abalada
transformada
sob efeito temporário
sem determinado equipamento
recurso temporariamente indisponível
localização quando necessária
intenção pessoal ainda em curso
outra condição temporária relevante
```

Não deve copiar:

```text
todos os presentes da cena
processos secretos
estado de outras personagens
planos do Opositor
Direções Autorais que a personagem não conhece
roteiro da temporada
```

## Uma realidade, leituras separadas

O Narrador pode conhecer o Estado global inteiro.

Cada cadeira recebe apenas:

```text
seu Estado pessoal
+
fatos perceptíveis
+
fatos aprendidos legitimamente
```

```text
REALIDADE GLOBAL EXISTE
≠
TODAS AS CADEIRAS CONHECEM TUDO SOBRE ELA
```

## Hierarquia quando houver divergência

Se Estado global e Estado local de uma ficha descrevem diferente **a mesma condição presente**:

```text
ESTADO DA CAMPANHA
→ fonte primária do presente.

ESTADO LOCAL DA FICHA
→ sincronizar.
```

A divergência é erro de sincronização, não duas realidades alternativas.

## Ficha permanente não é sobrescrita silenciosamente pelo Estado

```text
FICHA
→ quem a personagem é, o que sabe, possui e consegue fazer normalmente.

ESTADO
→ como a realidade está agora.
```

Se o Estado indicar mudança permanente legitimamente consolidada, atualizar a ficha no bloco adequado.

Uma Direção do Diretor que conscientemente altera fato permanente deve seguir também `canonizacao-e-correcoes.md`; não fingir que a mudança sempre existiu.

## O que não entra

Não usar `estado/atual.md` como depósito de:

```text
tudo que aconteceu
biografia completa
ficha inteira
mundo inteiro
conhecimentos completos
planos secretos integrais do Opositor
capítulos do Livro
fatos antigos sem efeito atual
Direções já consumadas
```

Também não manter mecanismos legados:

```text
Vida universal
Mente universal
Mana universal
```

## Entrar, mudar e sair

```text
ENTRA
→ quando algo passa a ser necessário para representar corretamente o presente ou uma Direção ainda ativa.

MUDA
→ quando realidade ou escopo autoral ativo mudam.

SAI
→ quando deixa de existir, deixa de importar ou a Direção é consumada.
```

## Processos longos

Quando processo existe em fonte própria, registrar somente o suficiente para sua interferência não ser esquecida.

Detalhes reservados do Opositor permanecem em `campanhas/<nome>/opositor/`.

## Salvar no meio de uma decisão

Se a campanha for interrompida antes de nova escolha, registrar o ponto sem decidir por ninguém.

Exemplo:

```text
A porta foi aberta.
B está do outro lado.
Nenhuma nova decisão de A foi declarada.
```

Se também houver Direção ativa:

```text
Direção Autoral Ativa: a conversa deve caminhar até X.
Escopo ainda aberto: como A e B chegam até esse ponto.
```

Não executar a Direção durante o salvamento apenas para removê-la da pendência.

## Regra de sincronização

Ao salvar, fechar capítulo ou reancorar:

```text
1. atualizar Estado global com realidade presente;
2. preservar Direções Autorais ainda ativas e seu escopo exato;
3. remover Direções já consumadas;
4. atualizar em cada ficha somente o recorte pessoal temporário pertinente;
5. remover condições encerradas;
6. consolidar mudanças permanentes na ficha quando apropriado;
7. não transmitir às cadeiras informação global ou autoral que elas não conhecem.
```

> **Sincronizar não significa copiar. Significa manter uma única realidade e preservar separação de conhecimento e autoridade.**

## Regra final

> **`estado/atual.md` é a fonte canônica global do presente e pode preservar Direções Autorais Ativas que ainda limitam a continuação. Essas Direções devem registrar claramente o que está fechado e o que permanece aberto, não são fatos já consumados e não entram no conhecimento das personagens. Quando forem cumpridas, saem do Estado e dão lugar ao acontecimento real nas fontes normais.**