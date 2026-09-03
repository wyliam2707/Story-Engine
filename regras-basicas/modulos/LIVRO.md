# Módulo Opcional — Livro

O `LIVRO` preserva a ficção canonizada da campanha em capítulos.

Ele é opcional. A campanha pode funcionar somente com Direção, Estado, Fichas e demais fontes necessárias.

> **O Livro registra a ficção que aconteceu. Não registra a direção usada para produzi-la.**

## Livro e capítulos

O Livro é a obra completa da campanha.

Os capítulos são as unidades que compõem essa obra.

```text
LIVRO
→ conjunto da ficção registrada.

CAPÍTULO
→ trecho fechado dessa ficção.
```

Não criar uma fonte paralela chamada `capitulos/` quando o módulo Livro estiver ativo. Os capítulos pertencem ao Livro.

## O que entra

O Livro registra somente ficção realmente estabelecida:

```text
narração válida
ações realizadas
decisões exercidas
falas
pensamentos e interioridade explicitamente estabelecidos
descobertas
consequências
mudanças de relação
mudanças de situação
passagem de tempo realmente ocorrida
causalidade necessária já consumada
```

Não entram no Livro:

```text
Direção
Consulta
Auditoria
Análise
Correção como metaconversa
instruções de cena
intenção não executada
Direção futura ainda não consumada
hipótese
plano futuro
resultado ainda aberto
versão anulada por correção ou refação
```

> **Direção consumida pode produzir ficção. A Direção em si não entra no Livro.**

## Forma de registro

O capítulo deve preservar claramente a origem da ficção quando isso for conhecido.

Formato recomendado:

```text
NARRADOR:
Descrição, consequência ou fato narrado.

KARA:
— Fala ou ação estabelecida para Kara.

KARA — pensamento:
*Interioridade estabelecida de Kara.*

DANIEL:
— Fala ou ação estabelecida para Daniel.

DANIEL — pensamento:
*Interioridade estabelecida de Daniel.*
```

Aplicar o mesmo padrão a outras personagens quando necessário.

Esses marcadores ajudam a preservar:

```text
quem falou
quem agiu
quem pensou
que informação pertence ao leitor
que informação pertence somente a uma personagem
```

O Livro pode melhorar apenas apresentação mínima — ortografia, pontuação, divisão de parágrafos e transições que não criem conteúdo novo.

Não deve converter automaticamente o registro em romance tradicional nem apagar marcadores de autoria/interioridade.

Uma adaptação literária diferente pode ser produzida posteriormente como material derivado, se o Diretor desejar.

## Versão válida

Se uma cena foi corrigida, refeita ou anulada durante o jogo:

```text
versão anulada
→ não entra.

versão final válida
→ entra.
```

O Livro não preserva erros de execução como se fossem acontecimentos canônicos.

## Estrutura sugerida

```text
livro/
├── README.md
├── 001-nome-do-capitulo.md
├── 002-nome-do-capitulo.md
└── ...
```

`livro/README.md` funciona como índice da obra e aponta a ordem dos capítulos.

Exemplo:

```text
# Nome da Campanha

## Capítulos

001 — Primeiro capítulo
002 — Segundo capítulo
```

Se a campanha usa Arcos Preparados, capítulos podem ser agrupados editorialmente mais tarde. Essa organização não altera o cânone.

## Fechar capítulo

Quando o comando `fechar o capítulo` for usado com este módulo ativo:

```text
1. parar no último fato realmente estabelecido;
2. reunir somente a ficção válida desde o último capítulo fechado;
3. excluir Direção, consultas, auditorias, instruções de cena e demais metaconversas;
4. preservar NARRADOR, falas, ações e pensamentos com sua origem quando conhecida;
5. salvar o capítulo dentro de livro/;
6. atualizar livro/README.md com o novo capítulo;
7. atualizar Estado, Fichas, Mundo, Direção ou outras fontes vivas somente se algo realmente mudou;
8. executar checkpoint operacional;
9. reancorar antes de continuar a ficção.
```

Não criar despedida, cliffhanger, reação, passagem de tempo ou qualquer outro acontecimento apenas para produzir um final melhor.

> **Fechar capítulo registra o ponto em que a ficção parou; não joga uma cena de encerramento.**

## Conhecimento e interioridade

O Livro pode conter conhecimento que não pertence a todas as personagens.

```text
LEITOR SABE
≠ PERSONAGEM SABE
```

Um pensamento de Kara registrado no capítulo não se torna conhecimento de Daniel.

Uma narração externa também não concede automaticamente esse conteúdo a qualquer Cadeira.

A retomada deve reconstruir conhecimento a partir das fontes corretas, não a partir de tudo que o leitor do Livro pode ver.

## Resumo e índice

Quando útil, um arco concluído pode receber:

```text
resumo.md
→ contexto condensado para consulta.

mapa-de-eventos.md
→ índice cronológico e causal.
```

Esses arquivos são derivados. Se contradisserem Ficha, Estado, Direção ou capítulo canônico, corrigir o resumo/índice.

> **O Livro preserva o passado ficcional em capítulos. Nunca recebe autoridade para jogar o futuro.**