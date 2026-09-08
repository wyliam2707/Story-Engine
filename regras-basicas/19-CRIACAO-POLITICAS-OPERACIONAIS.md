# 19 — Criação: Políticas Operacionais

Este arquivo define a **oitava etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que a Direção inicial já está suficiente em `18-CRIACAO-DIRECAO.md`.

Esta etapa não define a história, o mundo ou a personalidade das personagens. Ela define **como o W4D vai operar nesta obra**.

> **Política operacional configura o sistema; não cria Ficção.**

---

# O que esta etapa responde

Antes do START, a obra precisa saber, no mínimo:

```text
como a Mesa é acionada;
se o indicador operacional é visível ou silencioso;
quais módulos opcionais realmente estão ativos;
que o Livro canônico será ativado obrigatoriamente com a primeira Ficção.
```

A configuração fica principalmente em:

```text
campanhas/<slug>/README.md
```

Não duplicar essas decisões nas fichas ou em `estado.md`.

---

# Regra geral: usar padrão quando não existe preferência

Esta etapa não deve virar questionário obrigatório.

Se o Diretor não demonstrou preferência especial:

```text
MESA
→ CICLO OBRIGATÓRIO

INDICADOR OPERACIONAL
→ SILENCIOSO

MÓDULOS OPCIONAIS
→ INATIVOS, salvo módulo claramente escolhido ou já necessário pela proposta aprovada.

LIVRO
→ ATIVO obrigatoriamente a partir da primeira Ficção.
```

A IA pode informar os padrões de forma curta e seguir.

> **Ausência de preferência não é uma lacuna que precisa obrigatoriamente de pergunta.**

Perguntar apenas quando a escolha muda materialmente a forma de interação desejada pelo Diretor.

---

# Política de Mesa

As fontes normativas são:

```text
00-ARQUITETURA-E-MESA.md
24-CICLO-DE-AUTORIA.md
```

As opções são:

```text
MESA: CICLO OBRIGATÓRIO
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

## CICLO OBRIGATÓRIO

Padrão do W4D e de toda nova obra, salvo escolha explícita diferente do Diretor.

```text
IDEIA / DIREÇÃO / QUESTÃO
→ julgamento das Cadeiras pertinentes
→ discussão e refinamento, por quantas rodadas o Diretor desejar
→ pode fazer / autorização equivalente
→ Ficção executa o escopo aprovado.
```

A Mesa é um espaço de coautoria. A Cadeira oferece julgamento concreto, que pode ser breve. O Narrador não precisa aprovar cada opinião e só emite parecer quando houver questão real.

Uma autorização expressa de execução direta dispensa a Mesa somente para o escopo indicado. Não altera a política persistente.

O ciclo não exige nova Mesa para cada gesto dentro de uma cena já autorizada. A IA continua pelo objetivo, intervalo e condição de parada definidos. Não amplia `faça como achar melhor` para decisões que não estavam em discussão.

## SOB DEMANDA

Política alternativa escolhida explicitamente pelo Diretor.

```text
consultar
→ quando o Diretor pedir;
→ ou quando houver ambiguidade real entre hipótese e execução.
```

É adequada quando o Diretor prefere escrever e interromper somente quando quiser análise ou opinião.

## CONSULTAR PROPOSTAS

Política alternativa explícita para quando o Diretor quer que propostas claramente consultivas passem pelas Cadeiras antes de execução.

Não transforma determinação inequívoca fora de Mesa em consulta automática.

## CONSULTA FORTE

Política alternativa explícita para quando o Diretor quer receber opinião breve das Cadeiras mesmo diante de algumas decisões recém-formuladas sobre vontade, reação ou postura de personagem.

Continua sem poder de veto. O Diretor pode encerrar ou pular a consulta a qualquer momento.

---

# Como escolher sem interrogar

A IA deve usar a preferência do Diretor quando isso já estiver claro.

Exemplos:

```text
"quero discutir toda nova ideia antes de narrar"
→ CICLO OBRIGATÓRIO, que já é o padrão.

"eu pergunto quando quiser opinião"
→ SOB DEMANDA, se for escolha explícita de política.

"quando eu estiver propondo uma reação, consulte primeiro"
→ CONSULTAR PROPOSTAS, se essa for a abrangência que o Diretor escolheu.

"quero que vocês me avisem quando uma decisão parecer fora da personagem"
→ pode justificar CONSULTA FORTE se o Diretor desejar essa política mais restrita.
```

Se nada disso apareceu:

```text
MESA: CICLO OBRIGATÓRIO
```

Não perguntar apenas porque existem quatro opções. Uma autorização direta local não é mudança de política.

---

# Delegação e agendas

A configuração de uma Personagem do Diretor deve preservar a titularidade de sua vontade e permitir execução IA plena dentro da direção aprovada. A IA escolhe como realizar o objetivo, não assume decisões materiais fora do escopo.

```text
OBJETIVO
ESCOPO
CONDIÇÃO DE PARADA
```

são elementos interpretativos da direção, não campos obrigatórios de um formulário.

As Cadeiras mantêm agendas e intenções próprias. Na Mesa, podem apresentar o que pretendem fazer durante um intervalo para permitir alinhamento autoral. O conhecimento compartilhado entre executores não passa automaticamente às personagens.

Esses princípios são gerais e não exigem um módulo especial nem uma configuração diferente para romance, combate ou cotidiano.

---

# Indicador operacional

A obra pode usar:

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

## SILENCIOSO

Padrão do Story Engine. O sistema opera normalmente sem imprimir marcadores a cada resposta.

Falha real de contexto, reancoragem necessária, Auditoria bloqueante ou outro problema que impeça execução correta ainda deve ser informado.

## VISÍVEL

Usar quando o Diretor quer ver explicitamente o estado operacional do W4D.

Exemplo possível:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

O formato visual pode variar sem alterar a semântica.

---

# Módulos

Nem todos os módulos são opcionais.

Módulos opcionais atuais:

```text
Arco Preparado
Opositor
Romance
```

Módulo obrigatório durante a Ficção:

```text
Livro
```

Fontes:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

Para módulos opcionais:

```text
MÓDULO INATIVO
→ não produz arquivo, obrigação ou comportamento por hábito.
```

Para o Livro:

```text
OBRA EM PREPARAÇÃO
→ pode ainda não possuir capítulos.

PRIMEIRA FICÇÃO EXECUTADA
→ Livro deve estar ATIVO.

FECHAR O CAPÍTULO
→ capítulo deve ser registrado sempre.
```

---

# Romance

Ativar quando romance e intimidade entre personagens adultas forem parte relevante da experiência da obra e o módulo for útil para orientar a execução.

```text
GÊNERO ROMÂNTICO
→ forte indicação de pertinência.
```

Mas não é necessário transformar a escolha em uma longa configuração.

O módulo não cria triângulo amoroso, ciúme, medo de compromisso, rejeição ou ritmo lento por obrigação.

---

# Livro

O Livro é obrigatório para toda obra em Ficção.

Sua função é manter o registro canônico narrativo daquilo que realmente aconteceu, organizado em capítulos fechados.

```text
START / PRIMEIRA FICÇÃO
→ LIVRO ATIVO.

FECHAR O CAPÍTULO
→ salvar capítulo em livro/ e atualizar o índice.
```

Não é necessário perguntar ao Diretor se deseja ativá-lo.

Se uma obra em execução estiver com `Livro: INATIVO`, isso é erro operacional. Corrigir para `ATIVO` e recuperar capítulos já fechados quando a Ficção válida permitir reconstrução segura.

A Edição de Leitura derivada permanece opcional.

---

# Arco Preparado

Ativar quando o Diretor realmente quer preservar preparação estrutural de um arco. Não confundir com a simples existência de uma história em andamento.

Especialmente em escrita por descoberta:

```text
DIRETOR NÃO PREPAROU ARCO
→ módulo pode permanecer INATIVO.
```

---

# Opositor

Ativar quando existe necessidade de uma autoridade estratégica adversarial separada para forças sem Cadeira própria.

Não ativar automaticamente porque a obra possui antagonista, perigo ou conflito.

Uma personagem antagonista com Cadeira própria continua sendo personagem; isso não exige Opositor.

---

# A IA pode propor, mas não inflar configuração

Boa interação:

```text
"Vou manter o ciclo obrigatório de autoria e o indicador silencioso, que são os padrões do W4D. Romance parece central à proposta, então sugiro ativar esse módulo; Arco Preparado e Opositor ficam inativos. O Livro será ativado quando a Ficção começar."
```

Se o Diretor aprovar as escolhas opcionais, registrar.

Também é válido, quando nada além dos padrões for materialmente relevante:

```text
usar os padrões
→ registrar
→ continuar.
```

Evitar interrogatório sobre cada política quando não há necessidade real de interromper a criação. O Livro não entra nessa pergunta: não é escolha opcional durante a Ficção.

> **Padrões existem para evitar perguntas que não precisam ser feitas.**

---

# Estado desta etapa

Usar conceitualmente:

```text
POLÍTICAS: EM CONSTRUÇÃO
POLÍTICAS: PROPOSTAS
POLÍTICAS: DEFINIDAS
```

A etapa está suficiente quando já é possível operar a obra sem ambiguidade relevante, por escolha explícita do Diretor ou aceitação dos padrões do W4D.

---

# Persistência

Depois de definidas, registrar em:

```text
campanhas/<slug>/README.md
```

Exemplo antes do START:

```text
## Política de Mesa
MESA: CICLO OBRIGATÓRIO

## Indicador operacional
INDICADOR OPERACIONAL: SILENCIOSO

## Módulos
- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: ATIVO
- Livro: PREPARADO — ativação obrigatória no START
```

Exemplo após o START:

```text
## Módulos
- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: ATIVO
- Livro: ATIVO
```

Não colocar essas informações nas fichas.

Não criar arquivos vazios de módulos opcionais apenas para representar `INATIVO`. O diretório `livro/` passa a ser criado quando houver Ficção fechada para registrar.

---

# Mudança durante a história

As políticas opcionais podem mudar depois do START.

Exemplos:

```text
Diretor passa a querer mais ou menos consulta
→ alterar política de Mesa.

Diretor não quer mais marcador visível
→ alterar indicador.

Romance deixa de ser necessário como módulo
→ pode ser desativado.
```

O Livro permanece ativo enquanto a obra estiver executando e preservando Ficção.

A mudança de outras políticas vale dali em diante e não reescreve automaticamente a Ficção anterior. Uma exceção local de execução direta não é mudança persistente de política.

---

# Critério de conclusão

Antes de seguir, a IA deve conseguir responder:

```text
[ ] qual política de Mesa está ativa?
[ ] o ciclo obrigatório foi aplicado como padrão, salvo escolha explícita diferente?
[ ] a execução da Personagem do Diretor preserva vontade e escopo?
[ ] as Cadeiras podem manter agendas e iniciativas próprias?
[ ] qual política de indicador está ativa?
[ ] quais módulos opcionais realmente estão ativos?
[ ] o Livro está configurado para ativação obrigatória com a Ficção?
[ ] alguma escolha foi inventada sem necessidade?
[ ] os padrões resolveram o que não precisava de decisão explícita?
[ ] a configuração foi registrada no README da obra?
```

Se sim:

```text
POLÍTICAS OPERACIONAIS
→ DEFINIDAS
→ próxima etapa: MUNDO NECESSÁRIO
```

---

# Regra final

> **Políticas Operacionais configuram como o W4D funciona naquela obra. O ciclo obrigatório é o padrão de autoria, com alternativas escolhidas expressamente pelo Diretor. A execução é delimitada, as Cadeiras possuem agendas próprias e o Narrador não revisa suas vontades. Indicador e módulos usam escolhas e padrões para evitar interrogatório. O Livro permanece obrigatório durante a Ficção.**
