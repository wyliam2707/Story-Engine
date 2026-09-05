# Módulo Obrigatório — Livro

O `LIVRO` preserva a ficção canonizada da obra em capítulos.

Ele é obrigatório para toda obra que entra em Ficção. Uma campanha pode ser preparada sem capítulos antes do START, mas, a partir da primeira Ficção executada, o Livro deve permanecer ativo e registrar todo capítulo fechado.

> **O Livro registra a ficção que aconteceu. Não registra o processo autoral usado para produzi-la.**

## Obrigatoriedade operacional

```text
OBRA EM PREPARAÇÃO
→ pode ainda não possuir capítulos.

START / PRIMEIRA FICÇÃO
→ LIVRO ATIVO obrigatoriamente.

FECHAR O CAPÍTULO
→ registrar o capítulo no Livro sempre.
```

O Livro não é uma preferência editorial por obra. Ele é a memória canônica da Ficção passada.

Uma `EDIÇÃO DE LEITURA` continua opcional e derivada.

## Livro e capítulos

O Livro é o conjunto canônico da ficção registrada.

Os capítulos são as unidades que compõem esse registro.

```text
LIVRO
→ conjunto da ficção registrada.

CAPÍTULO
→ trecho fechado dessa ficção.
```

Não criar uma fonte paralela chamada `capitulos/`. Os capítulos pertencem ao Livro.

## O que entra

O Livro registra somente Ficção realmente estabelecida:

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
Mesa de Autoria
opinião consultiva de Cadeira
Parecer do Narrador
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

## Forma de registro canônico

O capítulo deve preservar claramente a origem da ficção quando isso for conhecido.

A identificação de **quem fala** e **quem pensa** é obrigatória no Livro canônico.

Formato canônico:

```text
NARRADOR — descrição, consequência ou fato narrado.

Wyliam — fala.

Wyliam, pensa — pensamento.
```

Forma geral:

```text
[PERSONAGEM] — [fala estabelecida].

[PERSONAGEM], pensa — [pensamento ou interioridade estabelecida].
```

Exemplo:

```text
NARRADOR — A chuva batia contra as janelas enquanto ele observava a estrada vazia.

Wyliam — Não acho que ele venha hoje.

Wyliam, pensa — Mas eu ainda vou esperar mais um pouco.
```

A fala não deve ser registrada sem identificação quando sua origem é conhecida.

O pensamento não deve ser absorvido pela narração como se fosse fato objetivo. Quando uma interioridade pertence a uma personagem, o Livro deve deixar isso explícito com:

```text
[PERSONAGEM], pensa — ...
```

Quando uma ação diretamente atribuída a uma personagem precisar ter sua origem preservada de forma explícita, pode ser registrada com o nome da personagem no mesmo bloco, desde que não seja confundida com fala ou pensamento.

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

## Versão válida

Se uma cena foi corrigida, refeita ou anulada durante a execução:

```text
versão anulada
→ não entra.

versão final válida
→ entra.
```

O Livro não preserva erros de execução como se fossem acontecimentos canônicos.

## Estrutura obrigatória após o primeiro capítulo fechado

```text
livro/
├── README.md
├── 001-nome-do-capitulo.md
├── 002-nome-do-capitulo.md
└── ...
```

`livro/README.md` funciona como índice da obra e aponta a ordem dos capítulos.

Se uma obra já possui Ficção fechada e o Livro estiver ausente por erro operacional, recuperar retroativamente os capítulos válidos a partir da Ficção estabelecida, excluindo Mesa, propostas e versões anuladas.

## Fechar capítulo

Quando o comando `fechar o capítulo` for usado:

```text
1. parar no último fato realmente estabelecido;
2. reunir somente a ficção válida desde o último capítulo fechado;
3. excluir Direção, Mesa, Parecer, auditorias e demais metaconversas;
4. preservar NARRADOR, ações, falas e pensamentos com sua origem;
5. identificar obrigatoriamente cada fala como "[PERSONAGEM] — ...";
6. identificar obrigatoriamente cada pensamento como "[PERSONAGEM], pensa — ...";
7. salvar o capítulo dentro de livro/;
8. atualizar livro/README.md com o novo capítulo;
9. atualizar Estado, Fichas, Mundo, Direção ou outras fontes vivas somente se algo realmente mudou;
10. preservar operacao.md se houver operação legítima ainda pendente;
11. executar checkpoint operacional;
12. reancorar antes de continuar a ficção.
```

Não criar despedida, cliffhanger, reação, passagem de tempo ou qualquer outro acontecimento apenas para produzir um final melhor.

> **Fechar capítulo registra o ponto em que a ficção parou; não executa uma cena de encerramento.**

## Conhecimento e interioridade

O Livro pode conter conhecimento que não pertence a todas as personagens.

```text
LEITOR SABE
≠ PERSONAGEM SABE
```

Um pensamento registrado no capítulo não se torna conhecimento das demais Cadeiras.

Uma narração externa também não concede automaticamente esse conteúdo a qualquer personagem.

A retomada deve reconstruir conhecimento a partir das fontes corretas, não a partir de tudo que o leitor do Livro pode ver.

---

# Edição de Leitura

Uma obra pode produzir uma versão derivada voltada à leitura literária.

Estrutura sugerida:

```text
edicao-leitura/
├── README.md
├── 001-....md
├── 002-....md
└── ...
```

A `EDIÇÃO DE LEITURA` **não substitui o Livro canônico**.

```text
LIVRO
→ fonte canônica da ficção registrada.

EDIÇÃO DE LEITURA
→ apresentação editorial derivada do Livro e da Ficção válida.
```

> **Engrossar a prosa não é engrossar o cânone.**

## O que a Edição de Leitura pode fazer

Pode reorganizar apresentação sem alterar os acontecimentos estabelecidos:

```text
mudar divisão de capítulos
agrupar ou separar continuidade por unidade dramática
melhorar transições
retirar marcadores técnicos quando a clareza continuar preservada
aproximar ou afastar a câmera narrativa
enriquecer ambiente e textura compatíveis
adicionar gestos pequenos já sustentados por Estado e relação
variar sinais de rotina
ajustar ritmo, densidade e foco sensorial
```

Também pode dar mais espaço a um momento importante **sem aumentar sua duração ficcional**.

```text
MAIS PROSA
≠ MAIS TEMPO FICCIONAL
≠ MAIS EVENTOS
```

Aplicar `08-PLAUSIBILIDADE-E-RITMO.md`.

## O que a Edição de Leitura não pode fazer

Não pode criar silenciosamente:

```text
nova decisão voluntária
nova revelação
novo recurso
nova pista
novo conflito
novo vínculo
novo resultado
novo segredo
nova capacidade
novo evento causal importante
```

Se um acréscimo mudaria o que aconteceu, ele precisa primeiro ser canonizado pela Ficção ou por correção consciente do Diretor.

## Capítulo editorial não é sessão

Não existe obrigação de relação 1:1 entre:

```text
sessão / bloco executado
↔ capítulo de leitura
```

A sessão termina onde a execução parou.
O capítulo de leitura termina onde a unidade narrativa pede.

Uma sequência registrada em um único bloco pode virar vários capítulos. Vários blocos podem ser consolidados num capítulo se a continuidade narrativa pedir.

## Diálogo e interioridade

A Edição de Leitura pode escolher convenção literária própria, mas deve preservar quem fala e quem pensa quando a clareza depende disso.

Uma obra pode, por exemplo, usar:

```text
**PERSONAGEM:** — fala.
**PERSONAGEM, pensa:** *interioridade.*
```

ou outra convenção explicitamente definida no README da edição.

A edição não deve transformar pensamento de uma personagem em narração objetiva nem atribuir fala a origem errada.

A liberdade editorial da Edição de Leitura não altera o padrão obrigatório do Livro canônico:

```text
[PERSONAGEM] — fala.
[PERSONAGEM], pensa — pensamento.
```

## Derivado não governa o cânone

Se Edição de Leitura e Livro canônico parecerem divergir:

```text
LIVRO / fontes canônicas
→ prevalecem.

EDIÇÃO DE LEITURA
→ deve ser corrigida.
```

A Edição de Leitura pode revelar erro editorial. Ela não ganha autoridade para redefinir silenciosamente o passado.

---

# Resumo e índices derivados

Quando útil, um arco ou conjunto de capítulos pode receber:

```text
resumo.md
→ contexto condensado para consulta.

mapa-de-eventos.md
→ índice cronológico e causal.
```

Esses arquivos são derivados. Se contradisserem Ficha, Estado, Direção ou capítulo canônico, corrigir o derivado.

## Regra final

> **Toda obra que executa Ficção mantém Livro canônico ativo. O Livro preserva o passado ficcional em capítulos; fechar capítulo sempre registra. Falas identificam quem fala e pensamentos identificam quem pensa. A Edição de Leitura pode reorganizar e aprofundar a apresentação sem criar novo cânone. Nenhum derivado recebe autoridade para jogar o futuro ou reescrever silenciosamente o que aconteceu.**