# Regras Básicas

Status: REFORMULAÇÃO ATIVA / BASE EXPERIMENTAL

Esta pasta está sendo convertida para um **RPG de autoria narrativa compartilhada**.

O objetivo do sistema não é produzir cenas por RNG. O objetivo é permitir que várias cadeiras escrevam a mesma história sem que uma delas tome para si a autoridade das outras.

> **As cadeiras escrevem. A ficha estabelece fatos. O Narrador julga. A ficção continua.**

## Princípio central

A ficha não existe principalmente para calcular chance de sucesso.

Ela existe para registrar:

```text
quem a personagem é
→ identidade, natureza, relações e estado persistente

o que ela sabe
→ conhecimentos e especialidades legítimos

o que ela pode fazer
→ Poderes, Traços, Recursos e capacidades

como ela se compara
→ graduações usadas somente quando uma comparação realmente importa
```

Quando a ficção já fornece uma resposta coerente, não se cria uma rolagem apenas para introduzir acaso.

```text
FATOS SUFICIENTES
→ julgar pela ficção

DÚVIDA OU DISCORDÂNCIA ENTRE AUTORIDADES
→ abrir Mesa somente com as partes afetadas

ACASO
→ só entra se uma regra futura ou a própria Mesa decidir entregar deliberadamente aquela parte da autoria ao acaso
```

## Autoria, cadeiras e executores

O motor separa **autoridade narrativa** de **forma de execução**.

```text
CADEIRA DE PERSONAGEM
→ decide voluntariamente por uma personagem.

OPOSITOR — OPCIONAL
→ representa forças adversariais persistentes sem cadeira própria quando a campanha se beneficia de uma autoridade estratégica dedicada.

NARRADOR / JUIZ
→ julga o encontro entre decisões e realidade estabelecida.

DIREÇÃO AUTORAL
→ camada fora da ficção para intenção, trajetória, tom ou limite narrativo.
```

Separadamente:

```text
EXECUTOR
→ pessoa, IA ou outro meio que opera uma cadeira ou função.
```

Portanto:

```text
CADEIRA
→ define autoridade.

EXECUTOR
→ define quem a opera.
```

Uma Cadeira de Personagem pode ser executada por humano, IA ou outro participante sem mudar sua soberania.

Uma mesma pessoa ou IA pode executar várias cadeiras, mas isso não mistura conhecimento, intenção ou autoridade.

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

Na execução textual adotada pelo sistema, colchetes sinalizam **Direção Autoral**:

```text
[quero que esta luta deixe claro que a Personagem A está em desvantagem]
```

Isso não é fala, pensamento ou conhecimento da personagem.

## Entrada

```text
Nova campanha
→ CRIACAO-DE-CAMPANHA.md

Novo Arco Preparado / Temporada
→ CRIACAO-DE-TEMPORADA.md

Começar ou continuar campanha
→ INICIO-E-RETOMADA.md
```

A Direção da Campanha é obrigatória para o START. Arco Preparado, Diretriz Fechada e Opositor são estruturas opcionais usadas somente quando a campanha realmente precisa delas.

## Estrutura

```text
regras-basicas/
├── CRIACAO-DE-CAMPANHA.md
├── CRIACAO-DE-TEMPORADA.md
├── INICIO-E-RETOMADA.md
├── nucleo/
├── jogador/
├── mestre/
├── opositor/
└── registro/
```

## Núcleo

O Núcleo define autoria, julgamento, comparação e continuidade.

Arquivos centrais ativos:

```text
nucleo/0.0-autoria-narrativa.md
→ filosofia e autoridade do sistema.

nucleo/0.1-resolucao.md
→ como a ficção resolve ações e conflitos sem exigir RNG.

nucleo/0.8-tempo-e-acoes.md
→ continuidade temporal, intenções persistentes e devolução de novas decisões à cadeira correta.

nucleo/1.0-tribunal.md
→ soberania das cadeiras, separação entre Cadeira e Executor e Direção Autoral.

nucleo/1.0.1-auditoria-das-cadeiras.md
→ quando abrir Mesa e quem realmente precisa participar.

nucleo/1.1-narrador.md
→ função do Narrador como Juiz.

nucleo/1.5-opositor.md
→ função opcional para oposição persistente sem cadeira própria.

nucleo/1.6-execucao-por-uma-unica-ia.md
→ como uma mesma IA pode executar várias autoridades sem fundi-las.

nucleo/1.7-criacao-emergente.md
→ criação de mundo neutro, autoria pessoal e preenchimento epistêmico.

nucleo/1.8-origem-de-conflitos.md
→ fontes legítimas de oposição e limites contra reconstrução retroativa.
```

Os antigos marcadores de rolagens, Mana, Vida/Mente, Potência, dano, iniciativa e outros subsistemas do motor anterior foram removidos da árvore ativa.

```text
HISTÓRICO DO GIT
→ preserva as versões antigas quando for necessário consultar a evolução do sistema.

ÁRVORE ATIVA
→ contém somente documentos que ainda cumprem função no motor atual ou estão em revisão real para essa função.
```

> **Legado histórico não precisa permanecer como arquivo ativo para continuar recuperável.**

## Jogador e ficha

A ficha funciona principalmente como **fonte de fatos narrativos e comparação**.

Exemplos:

```text
Personagem A
→ Especialista em Ocultismo.

Personagem B
→ conhece política, protocolo e costumes de sua cultura de origem.

Personagem C
→ Força Sobre-Humana [1].

Personagem D
→ Força Sobre-Humana [2].
```

`[2]` não significa bônus de +2 em uma rolagem. Significa que, quando ambas as capacidades forem diretamente comparáveis e os demais fatos não alterarem a situação, `[2]` é superior a `[1]`.

A ficha continua sendo a fonte canônica primária da personagem conforme `jogador/1.5-autoridade-da-ficha.md`.

## Regra de localização

`regras-basicas/` contém somente regras, procedimentos e modelos.

```text
regras-basicas/
→ como o sistema funciona.

campanhas/<nome>/
→ o que é verdade naquela campanha.
```

> **Regra fica aqui. Verdade concreta fica na campanha.**

## Fluxo de cena

Por padrão:

```text
DECLARAÇÃO
→ identificar o que pertence à própria cadeira
→ conferir fatos relevantes
→ verificar se outra autoridade é afetada
→ permitir objeção factual quando necessária
→ Narrador julga
→ narrar
→ devolver toda nova decisão voluntária à cadeira responsável
```

Não existe obrigação de abrir uma auditoria formal para cada frase.

A Mesa abre somente quando existe:

```text
dúvida real
discordância
conflito de autoridade
direção autoral que afeta outra cadeira
necessidade de esclarecer fatos antes da prosa
```

Se ninguém afetado discorda e os fatos estão claros, a história continua.

## Trava operacional

Narrar não significa decidir arbitrariamente.

O Narrador deve primeiro saber quais fatos e autoridades sustentam a continuação da cena.

```text
FATOS + AUTORIDADES
→ JULGAMENTO
→ SENTENÇA NARRATIVA
→ PROSA
```

A diferença para o motor anterior é importante:

```text
INCERTEZA
≠ rolagem obrigatória

DISPUTA
≠ rolagem obrigatória

FICÇÃO JÁ RESPONDE
→ seguir a ficção
```

## Estado atual da reformulação

A árvore ativa já não preserva subsistemas mortos apenas como aviso de que não devem ser usados.

Um arquivo pode continuar marcado como `REFORMULAÇÃO` quando ainda precisa de revisão real, mas sua permanência deve responder a uma função atual do sistema.

```text
FUNÇÃO ATUAL EXISTE
→ preservar e revisar.

SÓ EXPLICA MECÂNICA MORTA
→ remover; o Git já preserva o histórico.
```

Esse critério vale para futuras varreduras de limpeza.

## Regra final

> **Este sistema é uma estrutura para vários autores contarem uma história juntos. Cadeiras definem autoridade; executores apenas as operam. Cada cadeira conserva sua soberania; a ficha fornece fatos, conhecimentos, capacidades e comparações; o Opositor só entra quando uma campanha precisa dessa função; o Narrador julga coerência; e o acaso só recebe autoria quando deliberadamente escolhido.**
