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

OPOSITOR
→ representa fatos, recursos, intenções e resistência do lado adversarial dentro de sua autoridade.

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

Nova temporada
→ CRIACAO-DE-TEMPORADA.md

Começar ou continuar campanha
→ INICIO-E-RETOMADA.md
```

Esses arquivos ainda carregam partes do motor anterior e serão revisados gradualmente.

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

Os arquivos prioritários da reformulação são:

```text
nucleo/0.0-autoria-narrativa.md
→ filosofia e autoridade do sistema.

nucleo/0.1-resolucao.md
→ como a ficção resolve ações e conflitos sem exigir RNG.

nucleo/1.0-tribunal.md
→ soberania das cadeiras, separação entre Cadeira e Executor e Direção Autoral.

nucleo/1.0.1-auditoria-das-cadeiras.md
→ quando abrir Mesa e quem realmente precisa participar.

nucleo/1.1-narrador.md
→ função do Narrador como Juiz.

nucleo/1.5-opositor.md
→ função factual e adversarial do Opositor.

nucleo/1.6-execucao-por-uma-unica-ia.md
→ como uma mesma IA pode executar várias autoridades sem fundi-las.
```

Arquivos antigos de dado, Mana, Potência, dano, iniciativa e outros subsistemas permanecem temporariamente na árvore como material a revisar. Eles não devem ser usados para contradizer os princípios novos já consolidados nos arquivos acima.

## Jogador e ficha

A ficha passa a funcionar principalmente como **fonte de fatos narrativos e comparação**.

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

## Estado da migração

A reformulação começou pelo núcleo de autoria e resolução.

Ainda precisam de revisão conjunta, entre outros:

```text
criação completa da ficha
Patamares e orçamentos
Vida / Mente / Mana
combate e dano
iniciativa e tempo
Potência de Efeito
modelos de campanha e temporada que ainda citam o motor mecânico anterior
```

Até essa revisão terminar, preferir os princípios novos quando houver conflito conceitual e marcar inconsistências para correção em vez de inventar compatibilidade automática.

## Regra final

> **Este sistema é uma estrutura para vários autores contarem uma história juntos. Cadeiras definem autoridade; executores apenas as operam. Cada cadeira conserva sua soberania; a ficha fornece fatos, conhecimentos, capacidades e comparações; o Opositor apresenta resistência legítima; o Narrador julga coerência; e o acaso só recebe autoria quando a Mesa deliberadamente quiser entregá-la a ele.**
