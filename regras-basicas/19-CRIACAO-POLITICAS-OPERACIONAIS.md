# 19 — Criação: Políticas Operacionais

Este arquivo define a **oitava etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que a Direção inicial já está suficiente em `18-CRIACAO-DIRECAO.md`.

Esta etapa não define a história, o mundo ou a personalidade das personagens.

Ela define **como o W4D vai operar nesta obra**.

> **Política operacional configura o sistema; não cria Ficção.**

---

# O que esta etapa responde

Antes do START, a obra precisa saber, no mínimo:

```text
como a Mesa é acionada;
se o indicador operacional é visível ou silencioso;
quais módulos opcionais realmente estão ativos.
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
→ SOB DEMANDA

INDICADOR OPERACIONAL
→ SILENCIOSO

MÓDULOS
→ INATIVOS, salvo módulo claramente escolhido ou já necessário pela proposta aprovada.
```

A IA pode informar os padrões de forma curta e seguir.

> **Ausência de preferência não é uma lacuna que precisa obrigatoriamente de pergunta.**

Perguntar apenas quando a escolha muda materialmente a forma de interação desejada pelo Diretor.

---

# Política de Mesa

A fonte normativa é:

```text
00-ARQUITETURA-E-MESA.md
```

As opções são:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

## SOB DEMANDA

Padrão do W4D.

```text
consultar
→ quando o Diretor pedir;
→ ou quando houver ambiguidade real entre hipótese e execução.
```

É adequada quando o Diretor prefere escrever e interromper somente quando quiser análise ou opinião.

## CONSULTAR PROPOSTAS

Usar quando o Diretor quer que propostas claramente consultivas passem pelas Cadeiras antes de execução.

Não transforma determinação inequívoca fora de Mesa em consulta automática.

## CONSULTA FORTE

Usar quando o Diretor quer receber opinião breve das Cadeiras mesmo diante de algumas decisões recém-formuladas sobre vontade, reação ou postura de personagem.

Continua sem poder de veto.

O Diretor pode encerrar ou pular a consulta a qualquer momento.

---

# Como escolher sem interrogar

A IA deve usar o comportamento do Diretor quando isso já estiver claro.

Exemplos:

```text
"quero que vocês me avisem quando uma decisão parecer fora da personagem"
→ sugerir CONSULTA FORTE.

"eu pergunto quando quiser opinião"
→ SOB DEMANDA.

"quando eu estiver propondo uma reação, consulte primeiro"
→ CONSULTAR PROPOSTAS.
```

Se nada disso apareceu:

```text
MESA: SOB DEMANDA
```

Não perguntar apenas porque existem três opções.

---

# Indicador operacional

A obra pode usar:

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

## SILENCIOSO

Padrão do Story Engine.

O sistema opera normalmente sem imprimir marcadores a cada resposta.

Falha real de contexto, reancoragem necessária, Auditoria bloqueante ou outro problema que impeça execução correta ainda deve ser informado.

## VISÍVEL

Usar quando o Diretor quer ver explicitamente o estado operacional do W4D.

Exemplo possível:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

O formato visual pode variar sem alterar a semântica.

---

# Módulos opcionais

Os módulos não são classes obrigatórias de história.

Ativar somente quando cumprirem função real.

Módulos atuais:

```text
Arco Preparado
Opositor
Romance
Livro
```

Fontes:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

```text
MÓDULO INATIVO
→ não produz arquivo, obrigação ou comportamento por hábito.
```

---

# Romance

Ativar quando romance e intimidade entre personagens adultas forem parte relevante da experiência da obra e o módulo for útil para orientar a execução.

```text
GÊNERO ROMÂNTICO
→ forte indicação de pertinência.
```

Mas não é necessário transformar a escolha em uma longa configuração.

O módulo não cria:

```text
triângulo amoroso
ciúme
medo de compromisso
rejeição
ritmo lento
```

por obrigação.

---

# Livro

Ativar quando a obra quer manter um registro canônico narrativo em formato de livro/capítulos ou produzir uma edição de leitura derivada.

Não ativar apenas porque toda ficção "poderia virar livro".

```text
LIVRO ATIVO
→ existe função real de preservação editorial.
```

---

# Arco Preparado

Ativar quando o Diretor realmente quer preservar preparação estrutural de um arco.

Não confundir com a simples existência de uma história em andamento.

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
"Como você não indicou preferência operacional, vou manter os padrões: Mesa sob demanda e indicador silencioso. Romance parece central à proposta, então sugiro ativar esse módulo; os demais ficam inativos por enquanto."
```

Se o Diretor aprovar, registrar.

Também é válido, quando nada além dos padrões for materialmente relevante:

```text
usar os padrões
→ registrar
→ continuar.
```

Evitar:

```text
"Escolha 1, 2 ou 3 para Mesa."
"Escolha visível ou silencioso."
"Agora decida cada um dos quatro módulos."
```

quando não há necessidade real de interromper a criação.

> **Padrões existem para evitar perguntas que não precisam ser feitas.**

---

# Estado desta etapa

Usar conceitualmente:

```text
POLÍTICAS: EM CONSTRUÇÃO
POLÍTICAS: PROPOSTAS
POLÍTICAS: DEFINIDAS
```

A etapa está suficiente quando já é possível operar a obra sem ambiguidade relevante.

Isso pode acontecer por:

```text
escolha explícita do Diretor
OU
aceitação dos padrões do W4D.
```

---

# Persistência

Depois de definidas, registrar em:

```text
campanhas/<slug>/README.md
```

Exemplo:

```text
## Política de Mesa
MESA: SOB DEMANDA

## Indicador operacional
INDICADOR OPERACIONAL: SILENCIOSO

## Módulos
- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: ATIVO
- Livro: INATIVO
```

Não colocar essas informações nas fichas.

Não criar arquivos de módulo apenas para representar `INATIVO`.

---

# Mudança durante a história

As políticas podem mudar depois do START.

Exemplos:

```text
Diretor passa a querer mais consulta
→ alterar política de Mesa.

Diretor não quer mais marcador visível
→ alterar indicador.

Livro passa a ser útil
→ ativar módulo posteriormente.
```

A mudança vale dali em diante e não reescreve automaticamente a Ficção anterior.

---

# Critério de conclusão

Antes de seguir, a IA deve conseguir responder:

```text
[ ] qual política de Mesa está ativa?
[ ] qual política de indicador está ativa?
[ ] quais módulos realmente estão ativos?
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

> **Políticas Operacionais configuram como o W4D funciona naquela obra. Quando o Diretor não possui preferência, os padrões evitam interrogatório: Mesa sob demanda, indicador silencioso e módulos inativos salvo escolha ou necessidade real. Configuração operacional deve facilitar a escrita, não transformá-la em formulário.**