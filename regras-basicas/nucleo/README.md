# Núcleo

Status: REFORMULAÇÃO ATIVA

O Núcleo define como as cadeiras compartilham autoria, como o tempo avança e como o Narrador julga a ficção.

> **A literatura não substitui julgamento; o julgamento também não precisa virar matemática quando a ficção já responde.**

## Terminologia estrutural

Usar estes termos com funções diferentes:

```text
CADEIRA
→ unidade de autoria.
→ define quem pode decidir dentro de determinada autoridade.

EXECUTOR
→ pessoa, IA ou outro meio que opera uma cadeira ou função.
→ não altera a autoridade daquela cadeira.

CONFIGURAÇÃO DAS CADEIRAS
→ registro persistente das autoridades existentes na campanha e de quem as executa.

TRIBUNAL
→ estrutura de autoridade do sistema.
→ define soberania, limites, conflito de autoridade e função do Narrador/Juiz.

MESA
→ procedimento temporário de alinhamento.
→ abre somente quando existe dúvida, discordância, direção compartilhada ou conflito real que precise ser resolvido.
```

> **Cadeira define autoridade. Executor define quem a opera. A Configuração registra ambos. O Tribunal define os limites. A Mesa só abre quando essas autoridades precisam conversar.**

Não usar `HUMANO`, `IA` ou `IA EVENTUAL` como espécies diferentes de soberania narrativa.

## Funções estruturais

```text
CADEIRA DE PERSONAGEM
→ decide voluntariamente por uma personagem.

OPOSITOR — OPCIONAL
→ representa forças adversariais persistentes sem cadeira própria quando a campanha se beneficia de uma autoridade estratégica dedicada.

NARRADOR / JUIZ
→ julga o encontro entre fatos e autoridades.

DIREÇÃO AUTORAL
→ camada fora da ficção para intenção, trajetória, tom ou limite narrativo.
```

A forma concreta de execução é configurada por campanha.

```text
CADEIRA DE PERSONAGEM A
→ EXECUTOR: HUMANO.

CADEIRA DE PERSONAGEM B
→ EXECUTOR: IA.

NARRADOR / JUIZ
→ EXECUTOR: IA.

OPOSITOR
→ ATIVO: NÃO, salvo quando a campanha realmente precisar dessa função.
```

Mudar o executor não muda a natureza da cadeira.
Ativar ou não o Opositor não altera as regras de autoria das demais cadeiras.

## Fluxo atual

```text
DECLARAÇÃO
→ separar intenção de resultado presumido
→ identificar autoridades afetadas
→ consultar ficha, Estado e continuidade
→ permitir objeção factual quando necessária
→ Narrador / Juiz julga
→ abrir Mesa somente se houver dúvida ou discordância real
→ narrar
→ devolver toda nova decisão voluntária à cadeira correta
```

Quando determinada cadeira depende de entrada externa de seu executor, a execução aguarda essa entrada em vez de inventar a decisão.

## Arquivos canônicos da reformulação

```text
0.0-autoria-narrativa.md
→ filosofia central: vários autores, soberania das cadeiras e acaso opcional.

0.1-resolucao.md
→ ficção primeiro; comparação e julgamento sem rolagem obrigatória.

0.8-tempo-e-acoes.md
→ tempo contínuo e intenções persistentes.

1.0-tribunal.md
→ autoridade universal das cadeiras, separação entre Cadeira e Executor e Direção Autoral.

1.0.1-auditoria-das-cadeiras.md
→ Mesa sob demanda, somente com autoridades afetadas.

1.1-narrador.md
→ Narrador como Juiz.

1.2-jogador-humano.md
→ perfil de execução humana de uma Cadeira de Personagem; não cria autoridade diferente.

1.3-jogador-ia.md
→ perfil de execução por IA dedicada; não cria autoridade diferente.

1.4-jogador-ia-eventual.md
→ perfil de execução compartilhada por IA para cadeiras distintas.

1.5-opositor.md
→ função opcional para oposição persistente sem cadeira própria, objeção factual curta e precedência de cadeira própria sobre função adversarial.

1.6-execucao-por-uma-unica-ia.md
→ separação técnica entre várias cadeiras executadas pela mesma IA.

1.7-criacao-emergente.md
→ Narrador completa mundo neutro e consequências óbvias; fatos pessoais novos pertencem à cadeira da personagem.

1.8-origem-de-conflitos.md
→ fontes legítimas de oposição, conflitos derivados por causalidade e limites contra reconstrução retroativa; Opositor e Diretriz Fechada só restringem quando estiverem ativos.
```

Os nomes físicos `1.2-jogador-humano.md`, `1.3-jogador-ia.md` e `1.4-jogador-ia-eventual.md` são mantidos por compatibilidade documental. Conceitualmente, eles são **perfis de execução**, não tipos fundamentais de cadeira.

## Arquivos do motor anterior

Os arquivos abaixo são **marcadores de legado**. Eles não contêm regra ativa e não devem ser usados para reconstruir o motor antigo:

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

O conteúdo histórico permanece recuperável pelo histórico do Git.

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

MESMO EXECUTOR
→ pode operar várias cadeiras.
→ não mistura conhecimento, intenção ou autoridade.

OPOSIÇÃO ESTRUTURAL
→ precisa possuir fonte canônica legítima.
→ não pode nascer retroativamente apenas para responder a uma jogada.
→ quando houver Diretriz Fechada ativa, precisa respeitar as verdades que ela fechou.

DIRETRIZ FECHADA
→ ferramenta opcional de Arco Preparado.
→ fecha somente verdades que precisam existir antes de serem descobertas, enfrentadas ou testadas.
→ sua ausência não autoriza retroatividade.

CONFLITO DERIVADO
→ pode nascer causalmente de fatos realmente ocorridos.

OPOSITOR
→ função opcional.
→ quando ativo, pode jogar para vencer dentro de seu escopo.
→ não pode reconstruir o tabuleiro para vencer.
→ controla apenas forças adversariais sem cadeira própria incluídas em seu escopo.
→ sua ausência não elimina conflitos, perigos, processos ou consequências.

OBJEÇÃO SIMPLES
→ resposta simples.

DÚVIDA OU DISCORDÂNCIA REAL
→ abrir Mesa.

DIREÇÃO AUTORAL
→ conceito do sistema fora da ficção.

[ ]
→ convenção da execução textual para sinalizar Direção Autoral.
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
CADEIRA DE PERSONAGEM A
→ A tenta dominar B em força pura.

CADEIRA DE PERSONAGEM B
→ decide como B reage.

OPOSITOR, SE ATIVO E PERTINENTE
→ apresenta um fato adversarial dentro de seu escopo.

NARRADOR / JUIZ
→ julga o encontro entre intenções, fichas, Estado e demais fatos legítimos.
```

Se não houver Opositor ativo, nada falta ao julgamento: usar as cadeiras existentes, o mundo, o Estado, os processos e a causalidade já estabelecida.

Nenhuma rolagem é criada apenas para fingir que uma diferença factual desapareceu.

## Regra estrutural

```text
CADEIRAS DE PERSONAGEM
→ escrevem suas próprias peças.
→ mantêm essa autoria independentemente de quem as executa.

EXECUTORES
→ operam cadeiras ou funções.
→ podem ser humanos, IAs ou outros participantes.
→ não recebem autoridade extra por sua natureza técnica.

OPOSITOR, QUANDO ATIVO
→ representa resistência persistente e fatos adversariais legítimos dentro de seu escopo.
→ não assume personagem que já possua cadeira própria.

NARRADOR / JUIZ
→ julga coerência e causalidade.
→ pode completar mundo neutro sem invadir autoria pessoal.

CONFIGURAÇÃO DAS CADEIRAS
→ registra quais autoridades existem, quais funções opcionais estão ativas e quem as executa.

TRIBUNAL
→ define a estrutura de autoridade e julgamento.

MESA
→ alinha temporariamente autoridades quando necessário.

FICHA
→ estabelece fatos, capacidades, conhecimentos e comparações.

TEMPO
→ permite que todas as cadeiras continuem vivendo sem sincronização artificial.
```

## Regra final

> **O Núcleo organiza autoria, não tecnologia nem obrigação de antagonismo. Cadeira define autoridade; Executor define quem a opera. Humanos, IAs ou outros participantes podem executar cadeiras sem alterar sua soberania. O Narrador julga, a Mesa alinha quando necessário e nenhuma troca de executor transforma conhecimento técnico em conhecimento ficcional. Opositor, Temporada e Diretriz Fechada são estruturas opcionais: só entram quando a campanha realmente precisa delas.**