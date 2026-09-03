# Regras Básicas

Status: REFORMULAÇÃO ATIVA / BASE EXPERIMENTAL

Esta pasta define um **RPG puramente narrativo de autoria distribuída**.

O motor não depende de dados para produzir a história. Ele organiza quem pode decidir cada parte da ficção, como fatos são preservados, como intenções independentes se encontram e como o Diretor conduz a obra sem precisar escrever tudo sozinho.

> **As cadeiras escrevem as personagens. A ficha estabelece fatos. O Narrador julga. O Diretor conduz.**

## Princípio central

A ficha não existe principalmente para calcular chance de sucesso.

Ela registra:

```text
quem a personagem é
→ identidade, natureza, relações e fatos persistentes

o que ela sabe
→ conhecimentos e especialidades legítimos

o que ela pode fazer
→ Poderes, Traços, Recursos e capacidades

como ela se compara
→ graduações usadas somente quando uma comparação realmente importa
```

Quando a ficção já fornece resposta suficiente, não se cria chance apenas para introduzir incerteza.

```text
FATOS DETERMINAM
→ Narrador sentencia.

DECISÃO REALMENTE DISPONÍVEL A OUTRA CADEIRA
→ a cadeira decide.

DÚVIDA OU OBJEÇÃO REAL
→ Mesa / Auditoria verifica.

DIRETOR FECHOU A QUESTÃO
→ executar dentro do escopo determinado.
```

## Estrutura de autoria

```text
DIRETOR
→ autoridade autoral máxima sobre a direção da ficção.
→ pode também executar uma Cadeira de Personagem.
→ pode consultar, orientar ou determinar.

CADEIRA DE PERSONAGEM
→ decide voluntariamente pela própria personagem dentro do espaço que permanece aberto.

NARRADOR / JUIZ
→ julga o encontro entre decisões, fatos e realidade estabelecida.

MESA / AUDITORIA
→ verifica fatos, coerência, limites e autoridade quando necessário.
→ informa e alinha; não governa o Diretor.

OPOSITOR — OPCIONAL
→ representa forças adversariais persistentes sem cadeira própria quando a campanha precisa de autoridade estratégica dedicada.

EXECUTOR
→ pessoa, IA ou outro meio que opera uma cadeira ou função.
```

```text
CADEIRA
→ define autoria da personagem.

EXECUTOR
→ define quem a opera.

MESMO EXECUTOR
≠
MESMA CADEIRA
```

## Diretor e espaço aberto

O Diretor não precisa decidir toda a história.

Qualquer cadeira pode iniciar uma conversa, plano, relação, conflito ou ideia dentro de sua autoridade.

O Narrador pode desenvolver mundo neutro e consequências legítimas.

O Opositor pode mover suas forças quando estiver ativo.

O Diretor intervém quando quiser orientar ou fechar algo.

```text
DIRETOR NÃO DETERMINOU
→ o espaço continua emergente.

DIRETOR DETERMINOU
→ o ponto determinado fica fechado.
→ o restante continua aberto.
```

> **A autoridade do Diretor é absoluta sobre aquilo que ele efetivamente determina, mas não se expande automaticamente para aquilo que deixou aberto.**

## Direção não vira conhecimento da personagem

Uma Direção do Diretor existe fora da ficção.

```text
DIRETOR SABE / DETERMINA
≠
PERSONAGEM SABE / QUER
```

Se o Diretor determina que uma personagem perderá um confronto, ela ainda pode sinceramente tentar vencer quando isso for coerente com sua ficha e conhecimento.

O executor preserva simultaneamente:

```text
intenção legítima da personagem
+
resultado fechado pelo Diretor
```

sem fazer a personagem se sabotar e sem usar sua autonomia para invalidar o que foi determinado.

## `[ ]` na execução textual

Na execução textual adotada pelo sistema:

```text
[texto]
→ comunicação do Diretor fora da ficção.
```

Os colchetes identificam a camada. O conteúdo define a operação.

```text
[quero que X provoque Y até chegar a Z]
→ Direção.

[acho que X foi incoerente; justifique]
→ Análise.

[confira nos livros se isso já estava estabelecido]
→ Auditoria.

[o que seria mais coerente?]
→ Consulta.

[isso está errado; corrija segundo o cânone]
→ Correção.
```

Quando o Diretor pede auditoria ou análise antes de continuar, a progressão pertinente fica suspensa até a verificação terminar.

## Ser afetado não cria reação automática

```text
SER AFETADO
≠
TER UMA DECISÃO DISPONÍVEL
```

Uma cadeira só recebe nova decisão quando a personagem realmente possui escolha naquele instante.

Podem importar:

```text
percepção
tempo
oportunidade
posição
capacidade
meio disponível
```

> **A existência de uma cadeira protege autoria, não garante oposição.**

## Entrada

```text
Nova campanha
→ CRIACAO-DE-CAMPANHA.md

Novo Arco Preparado / Temporada
→ CRIACAO-DE-TEMPORADA.md

Começar ou continuar campanha
→ INICIO-E-RETOMADA.md
```

A Direção da Campanha é obrigatória para o START.

Arco Preparado, Diretriz Fechada e Opositor são estruturas opcionais.

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

O Núcleo define autoria, julgamento, direção e continuidade.

Arquivos centrais:

```text
nucleo/0.0-autoria-narrativa.md
→ filosofia, Diretor, Direção e espaço aberto.

nucleo/0.1-resolucao.md
→ fatos determinam, decisão real disponível e Direção fechada.

nucleo/0.8-tempo-e-acoes.md
→ continuidade temporal e intenções persistentes.

nucleo/1.0-tribunal.md
→ estrutura de autoridade.

nucleo/1.0.1-auditoria-das-cadeiras.md
→ Mesa sob demanda e validação factual de objeções.

nucleo/1.1-narrador.md
→ Narrador como Juiz.

nucleo/1.2-jogador-humano.md
→ execução humana e separação entre Cadeira e Diretor.

nucleo/1.3-jogador-ia.md
→ IA dedicada preservando personagem e Direção.

nucleo/1.5-opositor.md
→ função adversarial opcional.

nucleo/1.6-execucao-por-uma-unica-ia.md
→ separação técnica entre várias autoridades executadas pela mesma IA.

nucleo/1.7-criacao-emergente.md
→ criação neutra e preenchimento epistêmico.

nucleo/1.8-origem-de-conflitos.md
→ fontes legítimas de oposição e proibição de reconstrução retroativa.
```

## Jogador e ficha

A ficha é fonte canônica da personagem.

Graduações `[1]–[3]` existem apenas para comparar intensidade de capacidades equivalentes quando isso realmente importa.

```text
[1] < [2] < [3]
```

Elas não são bônus de teste, dano ou dificuldade.

A cadeira usa apenas a própria ficha, Estado pessoal, conhecimento legítimo e cena perceptível.

## Regra de localização

```text
regras-basicas/
→ como o motor funciona.

campanhas/<nome>/
→ o que é verdade naquela campanha.
```

> **Regra fica aqui. Verdade concreta fica na campanha.**

## Fluxo de cena

```text
DECLARAÇÃO
→ identificar Direção pertinente
→ separar intenção de resultado presumido
→ conferir fatos
→ fatos determinam?
   SIM → sentenciar
   NÃO → continuar
→ existe decisão real disponível a outra cadeira?
   SIM → executar a cadeira
   NÃO → não criar reação
→ auditar objeção factual, quando houver
→ Narrador julga
→ narrar
→ devolver nova decisão realmente disponível à autoridade correta
```

A Mesa não é ritual obrigatório.

Ela abre quando existe algo real para verificar ou alinhar.

## Opositor

Opositor é opcional.

Ele não existe para garantir dificuldade.

```text
NÃO HÁ OPOSIÇÃO LEGÍTIMA
→ não fabricar.

HÁ OPOSIÇÃO LEGÍTIMA
→ usar somente fatos, meios, conhecimento e oportunidade realmente existentes.
```

## Registro

```text
DECLARAÇÃO
→ intenção.

JULGAMENTO
→ estabelece realidade.

NARRAÇÃO
→ apresenta realidade.

REGISTRO
→ preserva o que precisa continuar verdadeiro.
```

Salvar não cria nova ficção.

## Motor legado

Não reativar automaticamente:

```text
Atributo + Perícia
2d6 universal
Potência de Execução
Defesa / Resistência matemáticas
Vida universal
Mente universal
Mana universal
iniciativa numérica
rodadas fixas
```

O Git preserva o histórico. A árvore ativa deve representar apenas o motor atual.

## O sistema não governa o Diretor

O motor pode apontar brevemente uma contradição relevante e o Diretor pode pedir explicação ou alternativas.

Se, compreendendo a questão, o Diretor determinar:

```text
faça assim mesmo
```

a execução segue.

> **O sistema protege a obra contra violações acidentais de autoridade e coerência, não contra decisões conscientes de seu próprio Diretor.**

## Regra final

> **Este é um RPG puramente narrativo de autoria distribuída. As cadeiras escrevem personagens independentes; a ficha fornece fatos; o Narrador julga; a Mesa audita; o Opositor só entra quando necessário; e o Diretor conduz a obra, podendo deixar a história emergir ou fechar exatamente os pontos que decidir fechar.**