# W4D — RPG Puramente Narrativo de Autoria Distribuída

## Proposta

**W4D é um RPG puramente narrativo de autoria distribuída.**

Cada personagem possui uma Cadeira com agência própria. A ficha estabelece fatos. O Narrador julga o encontro entre decisões e realidade. O Diretor conduz a obra e pode deixar a história emergir ou fechar pontos específicos quando desejar.

> **As Cadeiras escrevem. A ficha estabelece fatos. O Narrador julga. O Diretor conduz.**

A história não precisa ser decidida por dados. Ela nasce do encontro entre autores, fatos, causalidade e Direção.

---

# Se você é uma IA: comece aqui

Este repositório é **autossuficiente**.

Você não precisa de conversa anterior para aprender o sistema.

Use como autoridade operacional:

```text
1. os arquivos atuais da branch main;
2. os arquivos canônicos da campanha que estiver sendo jogada;
3. as Direções atuais do Diretor.
```

Não trate como regra:

```text
memória de conversas anteriores
suposições sobre outros RPGs
versões antigas recuperadas do histórico do Git
cânone externo de personagens que a ficha da campanha tenha redefinido
hábitos narrativos não registrados
```

O histórico do Git só deve ser consultado quando o Diretor pedir explicitamente uma auditoria histórica.

## Ordem de leitura

Para aprender o motor, leia nesta ordem:

```text
README.md
↓
regras-basicas/01-AUTORIDADE-E-DIRECAO.md
↓
regras-basicas/02-RESOLUCAO.md
↓
regras-basicas/03-CADEIRAS-E-EXECUTORES.md
↓
regras-basicas/04-FICHA.md
↓
regras-basicas/05-NARRADOR.md
↓
regras-basicas/06-REGISTRO-E-RETOMADA.md
↓
regras-basicas/07-CRIAR-CAMPANHA.md
```

Depois leia **somente os módulos ativados** pela campanha.

---

# Mapa rápido do sistema

```text
DIRETOR
→ conduz a obra.
→ pode deixar aberto, consultar, orientar ou determinar.

DIREÇÃO
→ conteúdo autoral emitido pelo Diretor.
→ fecha somente aquilo que foi efetivamente determinado.

CADEIRA
→ autoria voluntária de uma personagem.
→ pode iniciar ações e ter a primeira ideia.

EXECUTOR
→ humano, IA ou outro meio que opera uma autoridade.
→ não muda a natureza da autoridade.

FICHA
→ fonte canônica de quem a personagem é.

ESTADO
→ fonte canônica de como a ficção está agora.

NARRADOR / JUIZ
→ cruza Direção, decisões, fatos e causalidade.
→ estabelece a consequência.

AUDITORIA
→ verifica fatos, coerência, autoridade e escopo.
→ informa; não governa o Diretor.

OPOSITOR
→ módulo opcional para forças adversariais persistentes sem Cadeira própria.
```

---

# Regra mais importante de autoria

> **A autonomia existe dentro do espaço que permanece aberto.**

Exemplo:

```text
DIRETOR
→ [A perde este confronto. A forma está aberta.]
```

Isso fecha:

```text
A perde.
```

Mas deixa aberto, salvo nova Direção:

```text
como A tenta vencer
como B joga
falas
decisões intermediárias
forma concreta da derrota
```

A Cadeira de A continua tentando agir como A realmente agiria.

```text
DIRETOR SABE QUE A PERDE
≠
A SABE QUE VAI PERDER
```

O executor não faz A se sabotar e também não procura uma brecha para transformar a derrota em vitória.

---

# Comunicação do Diretor em texto

Na execução textual, colchetes identificam comunicação fora da ficção:

```text
[texto]
→ Diretor.
```

**Os colchetes identificam a camada; a semântica identifica a operação.**

```text
[quero que X aconteça]
→ DIREÇÃO
→ seguir.

[acho que X foi incoerente; justifique]
→ ANÁLISE
→ suspender a progressão pertinente e explicar.

[confira X nas fontes]
→ AUDITORIA
→ parar, consultar e verificar.

[o que seria mais coerente?]
→ CONSULTA
→ apresentar alternativas; não escolher pelo Diretor.

[isso está errado; corrija conforme o cânone]
→ CORREÇÃO
→ verificar e reconstruir.
```

Uma IA não deve responder a um pedido de auditoria com um comentário breve e continuar a cena como se nada tivesse acontecido.

---

# Fluxo básico de cena

```text
DIRETOR pode orientar ou deixar aberto
↓
CADEIRA declara intenção
↓
NARRADOR consulta fatos
↓
OS FATOS JÁ DETERMINAM?
├─ SIM → sentenciar
└─ NÃO
   ↓
   EXISTE DECISÃO VOLUNTÁRIA REALMENTE DISPONÍVEL A OUTRA CADEIRA?
   ├─ SIM → essa Cadeira decide
   └─ NÃO → não criar reação
↓
AUDITAR objeção factual, se houver
↓
NARRADOR cruza tudo e sentencia
↓
NARRAR
↓
PARAR quando surgir nova decisão realmente disponível
```

## Ser afetado não cria reação

```text
SER AFETADO
≠
TER UMA DECISÃO DISPONÍVEL
```

Uma Cadeira só recebe escolha quando percepção, tempo, oportunidade, posição, capacidade e meios realmente permitem decidir.

> **A existência de uma Cadeira protege autoria; não garante oposição.**

---

# Ficha

A ficha descreve a pessoa, não um orçamento.

Ela registra:

```text
Descrição Física
Conceito
Competências e Conhecimentos
Traços, Poderes e Meios
Personalidade e Vida Emocional
Histórico
```

O Estado temporário fica fora da ficha para existir em uma única fonte.

Capacidades podem receber graduação apenas quando comparação for útil:

```text
[1] — EXTRAORDINÁRIO
[2] — ELITE
[3] — ÁPICE
```

```text
[1] < [2] < [3]
```

A graduação mede intensidade do efeito descrito. Não cria nível geral.

---

# Narrador

O Narrador não escreve voluntariamente pelas Cadeiras.

> **Julgue primeiro. Narre depois. Registre por último.**

A prosa pode dar forma a tom, voz, ritmo, gesto e atmosfera, mas não pode esconder dentro da descrição uma nova ameaça, recurso, decisão ou solução.

Combate, romance, investigação, exploração e cotidiano usam a mesma estrutura de autoria. O foco muda; o motor não.

---

# Campanha

A estrutura mínima recomendada é:

```text
campanhas/<nome>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Arquivos opcionais aparecem somente quando necessários:

```text
mundo/
arco.md
oposicao.md
livro/
```

Para criar uma campanha, siga:

```text
regras-basicas/07-CRIAR-CAMPANHA.md
```

Para retomar uma campanha existente:

```text
README da campanha
→ direcao.md
→ estado.md
→ fichas relevantes
→ módulos ativos pertinentes
→ reancorar
→ continuar do primeiro ponto aberto.
```

---

# Módulos opcionais

```text
regras-basicas/modulos/ARCO-PREPARADO.md
→ preparação prévia de um arco e fatos que precisam existir antes da descoberta.

regras-basicas/modulos/OPOSITOR.md
→ autoridade estratégica para forças adversariais persistentes sem Cadeira própria.

regras-basicas/modulos/ROMANCE.md
→ orientações para histórias que tratam romance e intimidade adulta como foco relevante.

regras-basicas/modulos/LIVRO.md
→ arquivo literário opcional do que realmente aconteceu.
```

Módulo inativo não participa da campanha.

---

# Exemplo operacional mínimo

```text
DIRETOR
→ [quero que A provoque B porque considera B indigno, até a situação chegar a um confronto.]

→ trajetória vinculante.
→ a execução decide como chegar lá dentro do espaço aberto.

CADEIRA DE A
→ age segundo a personalidade de A e produz a provocação de forma própria.

CADEIRA DE B
→ responde somente quando e como a ficção realmente lhe oferece decisão.

NARRADOR
→ julga cada encontro e conduz a causalidade até o confronto.
```

Mais tarde:

```text
DIRETOR
→ [acho que a reação de B foi incoerente; confira a ficha e justifique.]
```

Então:

```text
PROGRESSÃO PERTINENTE
→ PARA.

AUDITORIA
→ consulta ficha, Estado e contexto.
→ explica se a reação foi coerente.
→ corrige se houver fundamento ou se o Diretor assim determinar.
```

Esse comportamento é parte do sistema, não uma preferência de conversa.

---

# Princípio documental

A documentação ativa segue:

> **Uma ideia, uma definição, uma fonte principal.**

Se dois arquivos parecerem contraditórios, use o arquivo cuja função é especificamente definir aquela questão e, se necessário, abra Auditoria. A branch `main` representa o sistema vigente.

---

## Lema

> **As Cadeiras escrevem. A ficha estabelece fatos. O Narrador julga. O Diretor conduz.**