# Manual de Registro da Campanha

Status: CANÔNICO DA REFORMULAÇÃO

Esta pasta é o **manual de persistência da história**.

Ela explica como transformar fatos já estabelecidos e Direções ainda ativas em fontes permanentes dentro de:

```text
campanhas/<nome>/
```

> **O jogo acontece na mesa. O Registro preserva o que precisa continuar verdadeiro — e preserva como Direção, não como acontecimento, aquilo que o Diretor ainda determinou para o futuro imediato.**

## Função do Registro

O Registro responde:

```text
SOBRE O QUE A CAMPANHA É?
→ mestre/narrativa.md

QUAL É O ARCO PREPARADO ATIVO?
→ mestre/roteiro.md

QUE DIREÇÃO LOCAL AINDA LIMITA A CONTINUAÇÃO?
→ estado/atual.md / Direções Autorais Ativas

QUEM É A PERSONAGEM?
→ ficha

COMO A CAMPANHA ESTÁ AGORA?
→ estado/atual.md

O QUE ACONTECEU?
→ livro/

O QUE É VERDADE ESTÁVEL DO CENÁRIO?
→ mundo/

O QUE CONTINUA AGINDO FORA DA CENA?
→ processos, prazos, opositor/ e fontes apropriadas
```

Registrar não cria ficção.

```text
DECLARAÇÃO
→ intenção.

DIREÇÃO DO DIRETOR
→ limite autoral, quando houver.

JULGAMENTO
→ estabelece realidade.

NARRAÇÃO
→ apresenta realidade.

REGISTRO
→ preserva o que precisa sobreviver.
```

## Direção ativa não é acontecimento

Se o Diretor determinou algo que ainda não aconteceu:

```text
DIREÇÃO AINDA ATIVA
→ preservar como Direção.

LIVRO
→ ainda não registra como acontecimento.
```

Exemplo:

```text
Direção: A perde o confronto atual.
Escopo fechado: resultado do confronto.
Permanece aberto: método e decisões intermediárias.
```

Quando a derrota realmente acontecer:

```text
→ Livro pode registrar como aconteceu.
→ Estado remove a Direção já consumada.
```

## Arquivos do manual

```text
registro/
├── README.md
├── fontes-da-campanha.md
├── salvar-a-historia.md
├── fechar-capitulo.md
├── estado-atual.md
├── livro-e-capitulos.md
├── arquivo-de-temporada.md
├── canonizacao-e-correcoes.md
└── reancoragem-operacional.md
```

## Fontes principais

### Ficha

Preserva identidade, capacidades, conhecimentos, Traços, Poderes, Equipamentos, Recursos, personalidade, relações e Histórico.

### Estado da Campanha

`campanhas/<nome>/estado/atual.md` é a fonte canônica global do presente.

Pode guardar:

```text
momento
localização
presenças
posições relevantes
condições temporárias
efeitos ativos
transformações em curso
equipamentos ou recursos indisponíveis
intenções persistentes
processos e prazos
Direções Autorais Ativas
primeiro ponto ainda aberto
```

### Livro

Preserva o que realmente aconteceu.

Não registra como fato consumado:

```text
intenção ainda não executada
Direção ainda não consumada
hipótese
plano futuro
decisão ainda aberta
metaconversa
versão anulada
```

### Mundo

Preserva verdades externas estáveis.

### Opositor

Preserva planos, processos, recursos e conhecimentos adversariais legitimamente existentes.

Plano não é acontecimento até ocorrer.

## Conhecimento por personagem

Um fato pode ser verdadeiro sem ser conhecido por todas as cadeiras.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

O mesmo vale para Direção:

```text
DIRETOR / EXECUTOR SABE
≠
PERSONAGEM SABE
```

## Processos e prazos

Processos continuam existindo fora da cena quando legitimamente estabelecidos.

O Registro preserva o processo; não precisa reencená-lo a cada resposta.

## Duplicação legítima

Uma mesma realidade pode aparecer em duas fontes quando cada uma responde a pergunta diferente.

```text
LIVRO
→ registra que A foi ferida.

ESTADO
→ registra que o ferimento ainda existe agora.

FICHA / ESTADO PESSOAL
→ carrega o recorte necessário.
```

Direção pendente segue lógica diferente:

```text
ESTADO
→ preserva a Direção enquanto ainda está ativa.

LIVRO
→ registra apenas o acontecimento depois que ele ocorrer.
```

## Vida, Mente e Mana

Os antigos mecanismos universais pertencem ao motor legado.

```text
VIDA UNIVERSAL
MENTE UNIVERSAL
MANA UNIVERSAL
→ não registrar como pressupostos do sistema ativo.
```

Registrar somente condição, custo ou recurso específico realmente existente.

## Fechar capítulo

O comando `fechar o capítulo` segue `fechar-capitulo.md`:

```text
parar
→ consolidar capítulo
→ atualizar fontes afetadas
→ preservar Direções ainda ativas sem executá-las
→ reset operacional
→ reancorar Diretor, autoridades e realidade
→ continuar do Estado atual
```

## Fechar temporada

Quando o arco realmente termina:

```text
fechar último capítulo
→ escrever epílogo
→ consolidar fichas, Estado, mundo e processos
→ arquivar roteiro
→ organizar livro/temporada-[N]/
→ criar resumo e mapa de eventos
→ reancorar
→ perguntar “E agora?”
```

## Salvar não joga

```text
SALVAR
→ preservar.

SALVAR
≠
continuar jogando.
```

Isso inclui não consumir uma Direção pendente durante o salvamento.

## Dados vivos ficam em `campanhas/`

Conforme necessidade:

```text
Direção da Campanha
Direções Autorais Ativas
Roteiro ativo
fichas
Estado global
relações e conhecimentos consolidados
processos e prazos
mundo
planos do Opositor
capítulos, epílogos, resumos e mapas
```

## Regra final

> **Registro é a memória canônica da campanha. A ficha preserva a personagem, o Estado preserva o presente e Direções locais ainda ativas, o Livro preserva o passado e as demais fontes preservam seu próprio contexto. Direção pendente nunca vira acontecimento apenas porque foi salva, e conhecimento autoral nunca vira conhecimento da personagem.**