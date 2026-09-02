# Estado Atual

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define a função de:

```text
campanhas/<nome>/estado/atual.md
```

`estado/atual.md` é a **fonte canônica global da realidade presente da campanha**.

Ele responde:

> **Se a campanha continuar agora, o que precisa estar imediatamente verdadeiro para que a próxima janela comece no lugar correto?**

## Princípio central

A campanha possui um único presente compartilhado.

```text
campanhas/<nome>/estado/atual.md
→ verdade canônica global do presente.

Ficha da personagem / bloco Estado Atual
→ recorte pessoal e operacional daquela personagem.
```

Os dois registros não competem pela mesma autoridade.

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
equipamentos ou recursos atualmente indisponíveis
intenções persistentes
ações interrompidas
processos em andamento
prazos próximos
consequências recentes que ainda alteram a situação
```

Nem todo campo precisa existir sempre.

```text
ACONTECEU E AINDA MUDA O PRESENTE
→ Estado Atual.

ACONTECEU MAS JÁ NÃO ALTERA O PRESENTE
→ Livro, Histórico ou outra fonte apropriada.
```

> **Entrar no Estado Atual exige utilidade para a continuação, não apenas ter acontecido.**

## Estado local da personagem

O bloco `Estado Atual` da ficha é um recorte pessoal do presente.

Ele pode registrar, quando relevante:

```text
ferida
exausta
abalada
transformada
sob efeito temporário
sem determinado equipamento
recurso temporariamente indisponível
localização atual quando necessária à cadeira
intenção pessoal ainda em curso
outra condição temporária que afete aquela personagem
```

Ele não deve copiar:

```text
todos os presentes da cena
processos secretos do mundo
estado de outras personagens
planos do Opositor
informação que a cadeira não conhece
roteiro da temporada
```

A finalidade é permitir que a cadeira recupere **como sua própria personagem está agora**, não entregar a ela a visão completa do Narrador.

## Uma realidade, duas leituras

Exemplo:

```text
ESTADO DA CAMPANHA
→ noite, biblioteca da mansão.
→ Corvin e Ravena estão presentes.
→ Corvin continua envenenado.
→ o veneno deve produzir novo efeito em aproximadamente uma hora.
→ Ravena está investigando a origem do veneno.

FICHA DE CORVIN — ESTADO ATUAL
→ Envenenado.
→ Está na biblioteca.

FICHA DE RAVENA — ESTADO ATUAL
→ Está na biblioteca.
→ Investigando a origem do veneno.
```

A ficha de Corvin não precisa receber automaticamente o que Ravena descobriu fora de sua percepção.

```text
REALIDADE GLOBAL EXISTE
≠
TODAS AS CADEIRAS CONHECEM TUDO SOBRE ELA
```

## Hierarquia quando houver divergência

Se o Estado da Campanha e o Estado local de uma ficha descreverem de forma diferente **a mesma condição presente**, não existem duas realidades paralelas.

```text
ESTADO DA CAMPANHA
→ fonte primária do presente.

ESTADO LOCAL DA FICHA
→ deve ser sincronizado com o recorte correspondente.
```

Exemplo:

```text
estado/atual.md
→ Ravena já se recuperou do ferimento.

ficha de Ravena
→ ainda diz “ferida no braço”.

RESULTADO
→ Ravena está recuperada.
→ corrigir o Estado Atual da ficha.
```

A divergência é erro de sincronização, não oportunidade para escolher a versão mais conveniente.

> **Para o presente, a realidade global prevalece; o recorte pessoal acompanha.**

## Ficha permanente não é sobrescrita pelo Estado

A primazia de `estado/atual.md` vale para **condições presentes e temporárias**, não para reescrever identidade permanente.

```text
FICHA
→ quem a personagem é, o que sabe, possui, consegue fazer e quais fatos permanentes a definem.

ESTADO DA CAMPANHA
→ como a realidade está agora.
```

Se o Estado Atual indicar uma mudança permanente já consolidada, a ficha deve ser atualizada no bloco adequado.

Até essa consolidação:

```text
MUDANÇA TEMPORÁRIA
→ permanece no Estado.

MUDANÇA PERMANENTE CONFIRMADA
→ atualizar ficha + remover redundância temporária quando apropriado.
```

## Separação de conhecimento por cadeira

O Narrador/Juiz pode carregar `estado/atual.md` inteiro para reconstruir a realidade.

Uma cadeira de personagem recebe somente:

```text
seu próprio Estado Atual relevante
+
fatos da cena que pode perceber
+
informações que aprendeu legitimamente
```

Portanto:

```text
NARRADOR CONHECE O ESTADO GLOBAL
≠
PERSONAGEM CONHECE O ESTADO GLOBAL
```

O arquivo global pode conter fatos necessários ao julgamento que não devem entrar na decisão de determinada personagem.

## O que não entra

Não usar `estado/atual.md` como depósito de:

```text
tudo que aconteceu no capítulo
biografia completa
ficha inteira
mundo inteiro
conhecimentos completos das personagens
planos secretos integrais do Opositor
capítulos do Livro
fatos antigos sem efeito atual
```

Também não manter sistemas mecânicos legados apenas porque apareciam em versões anteriores do Estado.

```text
Vida numérica ou trilhos universais
Mente numérica ou trilhos universais
Mana universal
```

não são campos obrigatórios da reformulação atual.

Uma personagem pode possuir recurso, condição ou limite específico desse tipo somente quando uma regra canônica, Traço, Poder, Equipamento ou outra fonte legítima realmente o definir.

## Entrar, mudar e sair

```text
ENTRA
→ quando algo passa a ser necessário para representar corretamente o presente.

MUDA
→ quando a realidade presente muda.

SAI
→ quando deixa de existir ou deixa de ser útil para continuidade imediata.
```

Exemplo:

```text
LIVRO
→ Corvin foi envenenado durante o jantar.

ESTADO ATUAL
→ Corvin continua envenenado agora.
```

Depois da cura:

```text
LIVRO
→ preserva o acontecimento quando relevante.

ESTADO ATUAL
→ remove a condição Envenenado.

ESTADO LOCAL DE CORVIN
→ também remove a condição.
```

## Processos longos

Nem todo processo precisa ser copiado integralmente para o Estado Atual.

Quando existir em fonte própria, registrar somente o suficiente para que sua interferência não seja esquecida.

Exemplo:

```text
## Processos relevantes
- investigação de Dick continua; consultar a fonte correspondente quando o prazo ou resultado se tornar relevante.
```

Detalhes reservados do Opositor permanecem em `campanhas/<nome>/opositor/`.

O Estado pode registrar que existe um processo ou prazo relevante sem revelar informação que uma cadeira não deveria conhecer.

## Salvar no meio de uma decisão

Se a campanha for interrompida exatamente antes de uma nova escolha, registrar o ponto sem decidir por ninguém.

Exemplo:

```text
A porta foi aberta.
Ravena está do outro lado.
Nenhuma nova decisão de Corvin foi declarada ainda.
```

Isso é suficiente.

Não completar:

```text
Corvin entra e começa a conversar.
```

se isso ainda não aconteceu.

## Regra de sincronização

Ao salvar, fechar capítulo ou reancorar:

```text
1. atualizar o Estado da Campanha com a realidade presente;
2. atualizar em cada ficha somente o recorte pessoal temporário que ainda importa;
3. remover dos recortes locais condições que já terminaram;
4. consolidar na ficha permanente mudanças que deixaram de ser temporárias;
5. não transmitir às cadeiras informação global que elas não conhecem legitimamente.
```

Não é necessário duplicar todo fato global em todas as fichas.

> **Sincronizar não significa copiar. Significa garantir que nenhum recorte pessoal contradiga a realidade compartilhada.**

## Regra final

> **`campanhas/<nome>/estado/atual.md` é a fonte canônica global do presente da campanha. O bloco Estado Atual de cada ficha é somente o recorte pessoal temporário necessário para aquela personagem. Quando ambos descrevem a mesma condição e divergem, o Estado da Campanha prevalece e a ficha deve ser sincronizada. O Narrador conhece o panorama global; cada cadeira recebe apenas aquilo que pertence legitimamente ao seu próprio estado, conhecimento e percepção.**