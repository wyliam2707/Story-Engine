# Núcleo

Status: REFORMULAÇÃO ATIVA

O Núcleo define como a autoria é distribuída, como o Diretor conduz a história, como o tempo avança e como o Narrador julga a ficção.

> **As cadeiras escrevem as personagens. O Narrador julga o encontro entre elas. O Diretor conduz a história.**

## Terminologia estrutural

```text
DIRETOR
→ autoridade autoral máxima sobre a direção da ficção.
→ pode também executar uma Cadeira de Personagem.
→ pode consultar, orientar ou determinar.

DIREÇÃO AUTORAL
→ conteúdo emitido pelo Diretor fora da ficção.
→ pode definir trajetória, tom, limite, condição, forma ou resultado.

CADEIRA
→ unidade de autoria de uma personagem.
→ decide voluntariamente dentro do espaço que permanece aberto.

EXECUTOR
→ pessoa, IA ou outro meio que opera uma cadeira ou função.
→ não altera a autoridade daquela cadeira.

CONFIGURAÇÃO DAS CADEIRAS
→ registro persistente das autoridades existentes e de quem as executa.

TRIBUNAL
→ estrutura que define autoridade, limites e julgamento.

MESA / AUDITORIA
→ procedimento temporário de verificação e alinhamento.
→ não é autoridade criativa acima do Diretor.

NARRADOR / JUIZ
→ julga fatos, causalidade e o encontro entre decisões.

OPOSITOR — OPCIONAL
→ representa forças adversariais persistentes sem cadeira própria dentro de escopo definido.
```

> **Cadeira define autoria da personagem. Executor define quem a opera. Narrador julga. Mesa audita. Diretor conduz.**

## Diretor e espaço aberto

O Diretor não precisa escrever tudo.

```text
DIRETOR NÃO DETERMINOU
→ cadeiras, Narrador, Opositor e criação emergente continuam produzindo ficção dentro de suas autoridades.

DIRETOR DETERMINOU
→ o ponto determinado fica fechado.
→ o restante continua aberto.
```

Exemplo:

```text
DIRETOR
→ A perde.

FECHADO
→ A perde.

ABERTO
→ como tenta vencer.
→ falas.
→ decisões intermediárias.
→ forma da derrota, se não especificada.
```

> **A autoridade do Diretor é absoluta sobre aquilo que ele efetivamente determina, mas não se expande automaticamente para aquilo que deixou aberto.**

## Direção não é conhecimento ficcional

```text
DIRETOR SABE / DETERMINA
≠
PERSONAGEM SABE / QUER
```

Uma determinação de derrota não faz a personagem desejar perder nem se sabotar.

O executor conhece a Direção e preserva o resultado fechado; a cadeira continua decidindo a partir do conhecimento e da personalidade da personagem.

## `[ ]` na execução textual

No modo textual adotado:

```text
[texto]
→ comunicação do Diretor fora da ficção.
```

Os colchetes identificam a camada. A intenção do texto define a operação.

```text
[quero X]
→ Direção.

[justifique X]
→ Análise.

[confira X nas fontes]
→ Auditoria.

[o que seria mais coerente?]
→ Consulta.

[corrija X]
→ Correção.
```

Pedido de auditoria ou análise suspende a progressão pertinente até ser respondido.

## Fluxo atual

```text
DECLARAÇÃO
→ identificar Direção pertinente
→ separar intenção de resultado presumido
→ consultar ficha, Estado e continuidade
→ perguntar se os fatos determinam
   → SIM: sentenciar
   → NÃO: continuar
→ perguntar se existe decisão voluntária realmente disponível a outra cadeira
   → SIM: executar essa cadeira
   → NÃO: não criar reação
→ auditar objeções factuais quando existirem
→ Narrador / Juiz cruza decisões e julga
→ Mesa somente se houver dúvida real
→ narrar
→ devolver toda nova decisão realmente disponível à cadeira correta
```

## Ser afetado não cria oposição

```text
SER AFETADO
≠
TER UMA DECISÃO DISPONÍVEL
```

Uma cadeira só é convocada quando os fatos deixam escolha real.

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

## Objeção factual

Uma objeção precisa apontar fundamento:

```text
fato
capacidade
Traço
posição
percepção
oportunidade
meio
conhecimento
limite de autoridade
```

Objeção sem fundamento não cria veto.

```text
AUDITORIA
→ verifica validade.
→ não fabrica reação.
```

## Arquivos canônicos principais

```text
0.0-autoria-narrativa.md
→ filosofia central, Diretor, espaço aberto e Direção Autoral.

0.1-resolucao.md
→ ficção primeiro, fatos determinam, decisão real disponível e Direção fechada.

0.8-tempo-e-acoes.md
→ tempo contínuo e intenções persistentes.

1.0-tribunal.md
→ estrutura de autoridade.

1.0.1-auditoria-das-cadeiras.md
→ Mesa sob demanda e validação factual de objeções.

1.1-narrador.md
→ Narrador como Juiz.

1.2-jogador-humano.md
→ execução humana e separação entre Cadeira e Diretor.

1.3-jogador-ia.md
→ IA dedicada preservando personagem e Direção sem misturá-las.

1.4-jogador-ia-eventual.md
→ execução compartilhada de cadeiras eventuais.

1.5-opositor.md
→ função adversarial opcional.

1.6-execucao-por-uma-unica-ia.md
→ separação de escopos quando uma IA executa várias funções.

1.7-criacao-emergente.md
→ criação neutra, autoridade epistêmica e proibição de retroatividade oportunista.

1.8-origem-de-conflitos.md
→ fontes legítimas de oposição e conflitos derivados.
```

## Princípios atuais

```text
FICÇÃO JÁ RESPONDE
→ seguir a ficção.

DIRETOR FECHOU ALGO
→ respeitar exatamente o escopo fechado.

DIRETOR PEDIU AUDITORIA
→ verificar antes de continuar.

INCERTEZA
→ não obriga RNG.

DISPUTA
→ não obriga RNG.

COMPARAÇÃO DIRETA
→ usar fatos e graduações pertinentes.

TEMPO
→ continuidade compartilhada, não fila fixa.

CADEIRA PRÓPRIA
→ decide voluntariamente a própria personagem quando existe decisão real disponível.

MESMO EXECUTOR
→ pode operar várias cadeiras sem misturar conhecimento.

OPOSIÇÃO
→ precisa possuir origem legítima.
→ não pode ser fabricada retroativamente.

OPOSITOR
→ opcional.
→ pode jogar para vencer dentro do escopo real.
→ não reconstrói o tabuleiro depois da jogada.

MESA
→ verifica e alinha.
→ não governa o Diretor.

REGISTRO
→ preserva; não cria.
```

## Combate no núcleo atual

Combate não ativa subsistema mecânico separado.

```text
COMBATE
→ mesma estrutura de autoria
→ posição, intenção, Habilidades, Poderes, Traços, Estado, ambiente e oposição
→ Narrador julga
```

Não usar automaticamente:

```text
Ataque + Defesa
2d6
Potência
Resistência
Vida numérica
Mana
iniciativa matemática
```

## O motor não protege a obra do próprio Diretor

As regras existem para impedir violações acidentais de autoridade, metaconhecimento, retroatividade e incoerências não percebidas.

Elas não existem para impedir uma decisão consciente do Diretor depois que ele compreende a consequência.

```text
SISTEMA
→ pode avisar brevemente sobre contradição relevante.

DIRETOR
→ pode pedir explicação ou alternativa.

DIRETOR
→ pode manter a decisão.

DEPOIS DE MANTER
→ executar.
```

> **Auditoria informa o Diretor; não governa o Diretor.**

## Regra final

> **O Núcleo organiza um RPG puramente narrativo de autoria distribuída. Cadeiras escrevem personagens independentes; o Narrador julga; o Diretor conduz e pode fechar o que decidir fechar; a Mesa audita sem virar veto; e uma personagem só recebe nova decisão quando a ficção realmente deixa uma escolha disponível. Opositor, Temporada e Diretriz Fechada continuam opcionais.**