# Manual de Registro da Campanha

Status: CANÔNICO DA REFORMULAÇÃO

Esta pasta é o **manual de persistência da história**.

Ela explica como transformar fatos já estabelecidos em fontes permanentes dentro de:

```text
campanhas/<nome>/
```

> **O jogo acontece na mesa. O Registro preserva o que precisa continuar verdadeiro depois da resposta.**

## Função do Registro

O Registro responde:

```text
SOBRE O QUE A CAMPANHA É?
→ mestre/narrativa.md

QUAL É O ARCO ATIVO?
→ mestre/roteiro.md

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

JULGAMENTO
→ estabelece realidade.

NARRAÇÃO
→ apresenta a realidade.

REGISTRO
→ preserva o que precisa sobreviver.
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

Preserva identidade, capacidades, conhecimentos, Traços, Poderes, Equipamentos, Recursos, personalidade, relações e Histórico relevantes da personagem.

O bloco `Estado Atual` da ficha guarda somente o recorte pessoal temporário daquela personagem.

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
Equipamentos ou Recursos indisponíveis
intenções persistentes
processos e prazos
primeiro ponto ainda aberto
```

Não é histórico completo.

### Livro

Preserva o que realmente aconteceu.

Não registra como fato consumado:

```text
intenção ainda não executada
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

## Vida, Mente e Mana

Os antigos mecanismos universais de `Vida`, `Mente` e `Mana` pertencem ao motor legado.

Eles não são campos obrigatórios de ficha, Estado, capítulo, reancoragem ou fechamento.

```text
VIDA UNIVERSAL
MENTE UNIVERSAL
MANA UNIVERSAL
→ não registrar como pressupostos do sistema ativo.
```

Quando uma personagem, Poder, Equipamento, Traço ou campanha possuir **um recurso ou condição específica realmente definida**, registrar aquilo pelo nome e escopo próprios.

Exemplos:

```text
Condição: braço fraturado.

Transformação: forma espectral ativa.

Recurso específico: três cargas restantes do artefato.

Limitação: Poder indisponível até o amanhecer.
```

> **Registrar o fato que existe; não recriar uma barra genérica para representá-lo.**

## Conhecimento por personagem

Um fato pode ser verdadeiro sem ser conhecido por todas as cadeiras.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

Se uma informação precisa orientar decisões recorrentes de uma personagem, consolidá-la na ficha quando apropriado.

Não copiar conhecimento automaticamente para outras personagens.

## Processos e prazos

Processos continuam existindo fora da cena quando já foram legitimamente estabelecidos.

Exemplo:

```text
Processo: investigação de Dick
Estado: em andamento
Prazo: primeiras pistas em 10 dias
```

O Registro preserva o processo; não precisa reencená-lo a cada resposta.

## Duplicação legítima

Uma mesma realidade pode aparecer em duas fontes quando cada uma responde a uma pergunta diferente.

```text
LIVRO
→ registra que Corvin foi ferido.

ESTADO DA CAMPANHA
→ registra que o ferimento ainda existe agora.

FICHA / ESTADO ATUAL DA PERSONAGEM
→ pode carregar o recorte pessoal desse ferimento.
```

Isso não exige trilho numérico universal.

Outro exemplo:

```text
LIVRO
→ registra que Ravena aprendeu um fato.

FICHA DE RAVENA
→ preserva o conhecimento que ela precisa continuar levando consigo.
```

## Fechar capítulo

O comando `fechar o capítulo` segue `fechar-capitulo.md`:

```text
parar
→ consolidar capítulo
→ atualizar fontes afetadas
→ reset operacional
→ reancorar
→ continuar do Estado atual
```

O fechamento não fabrica clímax, passagem de tempo nem nova decisão.

## Fechar temporada

Quando a condição de encerramento for realmente alcançada:

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

A próxima temporada não nasce automaticamente de um problema aberto.

## Salvar não joga

Quando o pedido for apenas salvar ou registrar:

```text
SALVAR
→ preservar.

SALVAR
≠
continuar jogando.
```

Parar no último fato estabelecido e não decidir nada que ainda esteja aberto.

## Dados vivos ficam em `campanhas/`

Isso inclui, conforme a necessidade real:

```text
Narrativa da Campanha
Roteiro ativo
fichas
Estado global
relações e conhecimentos consolidados
condições e efeitos presentes
Equipamentos e Recursos relevantes
processos e prazos
mundo
planos do Opositor
capítulos, epílogos, resumos e mapas
```

Não criar campos mecânicos apenas porque existiam em versões anteriores.

## Regra final

> **Registro é a memória canônica da campanha. A ficha preserva a personagem, o Estado preserva o presente global, o Livro preserva o passado e as demais fontes preservam o contexto que lhes pertence. Vida, Mente e Mana não são estruturas universais do sistema ativo; registrar somente condições, custos e recursos que realmente existam em uma fonte canônica específica.**