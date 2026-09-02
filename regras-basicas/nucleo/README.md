# Núcleo

Status: REFORMULAÇÃO ATIVA

O Núcleo define como as cadeiras compartilham autoria, como o tempo avança e como o Narrador julga a ficção.

> **A literatura não substitui julgamento; o julgamento também não precisa virar matemática quando a ficção já responde.**

## Fluxo atual

```text
DECLARAÇÃO
→ separar intenção de resultado presumido
→ identificar autoridades afetadas
→ consultar ficha, estado e continuidade
→ permitir objeção factual quando necessária
→ Narrador / Juiz julga
→ abrir Mesa somente se houver dúvida ou discordância real
→ narrar
→ parar na primeira nova escolha voluntária humana
```

## Arquivos canônicos da reformulação

```text
0.0-autoria-narrativa.md
→ filosofia central: vários autores, soberania das cadeiras e acaso opcional.

0.1-resolucao.md
→ ficção primeiro; comparação e julgamento sem rolagem obrigatória.

0.8-tempo-e-acoes.md
→ tempo contínuo, intenções persistentes, autonomia das cadeiras e parada na nova escolha humana.

1.0-tribunal.md
→ autoridade das cadeiras e modo Diretor por [ ].

1.0.1-auditoria-das-cadeiras.md
→ Mesa sob demanda, somente com autoridades afetadas.

1.1-narrador.md
→ Narrador como Juiz.

1.2-jogador-humano.md
→ autoridade da personagem humana.

1.3-jogador-ia.md
→ autonomia da personagem IA.

1.4-jogador-ia-eventual.md
→ agência eventual com conhecimento separado.

1.5-opositor.md
→ oposição legítima, objeção factual curta e precedência de cadeira própria sobre função adversarial.

1.6-execucao-por-uma-unica-ia.md
→ separação técnica entre várias cadeiras executadas pela mesma IA.

1.7-criacao-emergente.md
→ Narrador completa mundo neutro e consequências óbvias; fatos pessoais novos pertencem à cadeira da personagem.

1.8-origem-de-conflitos.md
→ oposição da Diretriz Fechada e conflitos derivados por causalidade; o Opositor joga o tabuleiro, não o reconstrói.
```

## Arquivos do motor anterior

Os arquivos abaixo foram reduzidos a **marcadores de legado**. Eles não contêm regra ativa e não devem ser usados para reconstruir o motor antigo:

```text
0.2-rolagens.md
0.3-consequencias.md
0.4-disputas-simultaneas.md
0.5-combate.md
0.6-dano-e-ferimentos.md
0.7-iniciativa.md
0.9-alcance-e-movimento.md
0.10-mana.md
0.11-vida-e-mente.md
0.12-ataques-mentais.md
0.13-cura-e-recuperacao.md
0.14-potencia-de-efeito.md
```

O conteúdo histórico dessas mecânicas permanece recuperável pelo histórico do Git.

```text
LEGADO
→ referência histórica.

LEGADO
≠ regra pendente que pode ser aplicada enquanto ninguém olha.
```

Nenhuma reancoragem, julgamento, combate, investigação ou registro deve consultar esses arquivos como autoridade mecânica.

## Princípios atuais

```text
FICÇÃO JÁ RESPONDE
→ seguir a ficção.

INCERTEZA
→ não obriga RNG.

DISPUTA
→ não obriga RNG.

COMPARAÇÃO DIRETA
→ usar fatos e graduações pertinentes.

TEMPO
→ continuidade compartilhada, não fila fixa de turnos.

MUNDO NEUTRO INDEFINIDO
→ Narrador pode completar quando coerente e não consequencial.

FATO PESSOAL NOVO
→ pertence à cadeira da personagem.

CADEIRA PRÓPRIA
→ prevalece sobre função adversarial.
→ ser antagonista não transfere autoria ao Opositor.

OPOSIÇÃO ESTRUTURAL
→ precisa pertencer à Diretriz Fechada antes do START.

CONFLITO DERIVADO
→ pode nascer causalmente de fatos realmente ocorridos.

OPOSITOR
→ pode jogar para vencer.
→ não pode reconstruir o tabuleiro para vencer.
→ controla apenas forças adversariais sem cadeira própria.

OBJEÇÃO SIMPLES
→ resposta simples.

DÚVIDA OU DISCORDÂNCIA REAL
→ abrir Mesa.

DIREÇÃO HUMANA EM [ ]
→ modo Diretor, fora da ficção.

NOVA ESCOLHA HUMANA
→ parar e devolver controle.
```

## Combate no núcleo atual

Combate não ativa o motor legado.

```text
COMBATE
→ mesma estrutura de autoria
→ posição, intenção, Habilidades, Poderes, Traços, Estado, ambiente e oposição em primeiro plano
→ Narrador julga o encontro
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

## Exemplo curto

```text
Corvin
→ vai para cima do Rei para mostrar quem manda.

CADEIRA DO REI
→ decide como o Rei reage.

Opositor
→ apresenta que o Rei é mais forte e está em melhores condições.

Narrador
→ julga o encontro entre as duas intenções.

→ nenhuma rolagem é criada apenas para fingir que a diferença factual desapareceu.
```

## Regra estrutural

```text
JOGADORES
→ escrevem suas próprias peças.
→ mantêm essa autoria mesmo quando suas personagens se tornam antagonistas.

OPOSITOR
→ representa resistência e fatos adversariais legítimos.
→ movimenta oposição existente sem cadeira própria e consequências derivadas.
→ não amplia retroativamente a Diretriz Fechada.
→ não assume personagem que já possua cadeira própria.

NARRADOR
→ julga coerência e causalidade.
→ pode completar mundo neutro sem invadir autoria pessoal.

MESA
→ alinha autoridades quando necessário.

FICHA
→ estabelece fatos, capacidades, conhecimentos e comparações.

TEMPO
→ permite que todas as cadeiras continuem vivendo sem sincronização artificial.
```

## Regra final

> **O Núcleo não existe para perguntar aos dados o que autores e ficção já conseguem determinar. Ele existe para preservar autoria, estabelecer limites, organizar o tempo, resolver conflitos de autoridade e manter a história coerente enquanto várias cadeiras a escrevem juntas. Arquivos legados não possuem autoridade sobre a reformulação atual; oposição estrutural pertence ao tabuleiro preparado, conflitos novos só surgem legitimamente quando a própria ficção os produz por causalidade e uma personagem nunca perde sua cadeira apenas por se tornar antagonista.**
