# Fontes da Campanha

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define **onde salvar cada tipo de verdade** dentro de `campanhas/<nome>/`.

> **Cada verdade deve ter uma fonte principal. Direção persistente também precisa de uma fonte quando deve sobreviver ao contexto imediato.**

## Regra de roteamento

```text
QUEM É A PERSONAGEM E O QUE ELA PRECISA LEVAR CONSIGO?
→ personagens/<nome>.md

SOBRE O QUE A CAMPANHA É AO LONGO DOS ARCOS?
→ mestre/narrativa.md

QUAL É O ARCO PREPARADO ATIVO?
→ mestre/roteiro.md

QUE DIREÇÃO AUTORAL AINDA LIMITA O PONTO ATUAL?
→ estado/atual.md, quando for local/operacional.
→ mestre/narrativa.md, quando alterar a identidade persistente da campanha.
→ mestre/roteiro.md, quando for uma Direção persistente daquele arco.

COMO A CAMPANHA ESTÁ AGORA?
→ estado/atual.md

O QUE É VERDADE ESTÁVEL DO CENÁRIO?
→ mundo/

O QUE O LADO ADVERSARIAL ESTÁ FAZENDO?
→ opositor/

O QUE REALMENTE ACONTECEU?
→ livro/
```

## Direções do Diretor

Nem toda Direção precisa ser salva.

```text
DIREÇÃO JÁ CONSUMADA NA MESMA JANELA
→ não precisa de registro separado.
→ o resultado real entra nas fontes normais.

DIREÇÃO QUE AINDA LIMITA A CONTINUAÇÃO
→ precisa ser preservada antes de checkpoint, troca de chat ou perda de contexto.
```

Roteamento:

### Direção da Campanha

```text
campanhas/<nome>/mestre/narrativa.md
```

Guarda identidade, foco e limites persistentes.

### Direção de Arco

Quando houver Arco Preparado:

```text
campanhas/<nome>/mestre/roteiro.md
```

Pode guardar Direção do Arco e determinações persistentes próprias daquele arco quando realmente precisarem sobreviver entre cenas.

### Direção local / resultado ainda não consumado

Se o Diretor fechou algo que ainda precisa ser cumprido a partir do ponto atual:

```text
campanhas/<nome>/estado/atual.md
```

Pode registrar um bloco como:

```text
## Direções Autorais Ativas

- A deve perder o confronto atual.
  Escopo fechado: resultado do confronto.
  Permanece aberto: método, falas e decisões intermediárias não especificadas.
```

Esse bloco é operacional e temporário.

Quando a Direção for consumada:

```text
→ remover da lista de Direções Autorais Ativas.
→ registrar o que realmente aconteceu nas fontes normais.
```

> **Registrar uma Direção ativa significa preservar um limite autoral ainda não consumado; não significa transformar o conteúdo inteiro da Direção em fato já acontecido.**

## `personagens/`

Guarda as fichas reais.

A ficha pode conter:

```text
identidade
Descrição Física
Conceito
Habilidades e Conhecimentos
Traços e Poderes
Equipamentos e Recursos
Descrição Emocional / Personalidade
relações
Histórico
Estado Atual pessoal
```

O bloco `Estado Atual` da ficha é apenas recorte pessoal temporário.

## Conhecimento relevante

Quando esquecer uma informação provavelmente faria a personagem decidir de forma incoerente, consolidar esse conhecimento na ficha ou fonte apropriada.

```text
PERSONAGEM A SABE
≠
PERSONAGEM B SABE
```

Direção do Diretor nunca entra automaticamente como conhecimento de personagem.

## Relações e ponto de vista

Relações registradas na ficha pertencem ao ponto de vista daquela personagem.

```text
FICHA DE A
→ como A entende o vínculo.

FICHA DE B
→ como B entende o vínculo.
```

As leituras podem divergir.

## `estado/atual.md`

É a fonte canônica global da realidade presente e do limite autoral operacional ainda ativo.

Pode registrar:

```text
momento e local
quem está presente
posição das peças
condições temporárias
efeitos ativos
transformações em curso
equipamentos ou recursos indisponíveis
intenções persistentes
ações interrompidas
processos e prazos próximos
fatos recentes que ainda alteram a situação
Direções Autorais Ativas ainda não consumadas
primeiro ponto ainda aberto
```

Não registrar `Vida`, `Mente` ou `Mana` universais.

## `mundo/`

Guarda verdades estáveis externas às personagens.

Exemplos:

```text
localização de cidade
regra política estabelecida
organização existente
característica permanente de local
evento que alterou duradouramente o cenário
```

## `mestre/`

### `mestre/narrativa.md`

Fonte da identidade persistente:

```text
foco
gênero e tom
experiência desejada
temas e conflitos recorrentes
o que não deve dominar
premissas gerais
mudanças persistentes de Direção determinadas pelo Diretor
```

### `mestre/roteiro.md`

Fonte do Arco Preparado ativo:

```text
Direção do Arco
problema estrutural, quando houver
Diretriz Fechada
processos preparados
limites do arco
condição de encerramento
Direções persistentes específicas do arco, quando realmente necessárias
```

O Roteiro não decide sozinho pelas personagens. Uma Direção registrada ali precisa vir da autoridade legítima do Diretor ou da preparação já aprovada.

### `mestre/temporadas/`

Guarda roteiros de temporadas encerradas.

## `opositor/`

Guarda oposição sem cadeira própria e processos adversariais legitimamente existentes.

Pode conter:

```text
objetivos
planos
preparação
prazos
conhecimento adversarial
recursos disponíveis
processos em andamento
```

Plano não é acontecimento.

## `livro/`

Guarda o histórico canônico do que efetivamente aconteceu.

Não registrar como acontecimento:

```text
intenção ainda não executada
Direção ainda não consumada
hipótese
plano futuro
metaconversa
resultado ainda aberto
```

Quando uma Direção finalmente se realiza, o Livro registra **o acontecimento**, não a ordem autoral que existia antes dele.

## Duplicação legítima

Uma realidade pode aparecer em mais de uma fonte quando cada ocorrência possui função diferente.

```text
LIVRO
→ registra que A foi ferida.

ESTADO DA CAMPANHA
→ registra que o ferimento continua presente.

FICHA / ESTADO PESSOAL
→ carrega o recorte necessário para A.
```

Outro exemplo:

```text
ESTADO
→ registra que “A perde este confronto” ainda é uma Direção ativa.

LIVRO
→ depois registra como a derrota realmente aconteceu.

ESTADO
→ remove a Direção já consumada.
```

Duplicação funcional não significa autoridade concorrente.

## Vida, Mente, Mana e mecanismos antigos

Não tratar como padrão:

```text
Vida universal
Mente universal
Mana universal
```

Se campanha ou personagem possuir condição, reserva, carga, transformação ou custo particular realmente estabelecido, registrar o elemento específico em sua fonte correta.

## Evitar cópia sem função

Não repetir por padrão:

```text
cena inteira no Estado
ficha inteira no README
segredos em vários arquivos
todo o Livro na ficha
toda a lore em cada personagem
todo plano do Opositor no Estado
Narrativa inteira dentro do Roteiro
Direção já consumada como se ainda estivesse pendente
```

## Regra final

> **Escolha a fonte pela função da verdade. Ficha guarda a personagem; Narrativa guarda identidade persistente; Roteiro guarda preparação e Direções de arco quando pertinentes; Estado guarda o presente e Direções Autorais Ativas ainda não consumadas; Mundo guarda contexto estável; Opositor guarda oposição legítima; Livro guarda o que aconteceu. Uma Direção ativa é limite autoral, não acontecimento consumado nem conhecimento da personagem.**