# 17 — Criação: Autoridades, Cadeiras e Executores

Este arquivo define a **sexta etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que as fichas iniciais necessárias estão suficientemente construídas em `16-CRIACAO-FICHAS.md`.

A definição normativa de Cadeira, Executor e Personagem do Diretor continua em:

```text
03-CADEIRAS-E-EXECUTORES.md
```

Este arquivo define **como uma IA configura essas autoridades durante a criação de uma obra nova**.

> **Primeiro existe a pessoa. Depois se define quem possui sua vontade e quem executa essa autoridade.**

---

# O que esta etapa responde

A etapa precisa permitir responder:

```text
quem é o Diretor?
quem executa o Narrador / Juiz?
alguma personagem pertence diretamente ao Diretor?
quais personagens possuem Cadeira persistente agora?
quem executa cada Cadeira?
quem possui a próxima autoria quando a Ficção começar?
```

Não é uma etapa de personalidade.

Não é uma etapa de trama.

Não altera as fichas.

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

---

# Autoridade e execução não são a mesma coisa

O W4D separa:

```text
AUTORIDADE
→ quem pode decidir determinado espaço ficcional.

EXECUTOR
→ quem opera essa autoridade na prática.
```

Exemplo:

```text
Daniel
→ PERSONAGEM DO DIRETOR.
→ vontade pertence ao Diretor.
→ execução textual pode ser feita pela IA quando delegada.
```

Nesse caso:

```text
DIRETOR DEFINE O QUE DANIEL QUER
≠ DIRETOR PRECISA ESCREVER TODA A PROSA DE DANIEL
```

Outro exemplo:

```text
Kara
→ Cadeira de personagem.
→ Executor: IA.
```

A IA pode formar a vontade de Kara no espaço aberto porque ela recebeu essa Cadeira.

---

# Configuração mínima mais comum

Quando a obra é conduzida por uma pessoa em conversa com uma IA, a configuração mais comum é:

```text
DIRETOR
→ HUMANO.

NARRADOR / JUIZ
→ IA.

CADEIRAS das personagens não atribuídas ao Diretor
→ IA.
```

Isso pode ser proposto como padrão operacional quando o contexto não indicar outra configuração.

Mas a IA **não deve escolher silenciosamente qual personagem central pertence ao Diretor**.

Se isso ainda estiver realmente aberto e a resposta já for necessária, perguntar de forma direta:

> **Você quer controlar diretamente alguma das personagens centrais, ou deixamos as Cadeiras delas com a IA?**

Não repetir a pergunta se o contexto já resolveu a questão.

---

# Quando o contexto já resolve

Exemplos:

```text
"Daniel é meu; você faz Kara."
```

já define:

```text
Daniel
→ Personagem do Diretor.

Kara
→ Cadeira IA.
```

Outro exemplo:

```text
"eu quero só dirigir; todas as personagens ficam com a IA."
```

já define:

```text
nenhum Personagem do Diretor.
Todas as Cadeiras centrais
→ IA.
```

Outro exemplo:

```text
"eu jogo com Ana e meu amigo controla Bruno."
```

já fornece dois executores humanos distintos.

> **Informação já dada deve ser registrada, não perguntada novamente.**

---

# Personagem do Diretor

`PERSONAGEM DO DIRETOR` é uma personagem cuja vontade permanece sob decisão direta do Diretor.

```text
PERSONAGEM DO DIRETOR
→ vontade: DIRETOR.
```

Isso inclui decisões como:

```text
o que quer
o que tenta
o que aceita
o que recusa
o que diz quando o conteúdo depende de decisão própria
qual iniciativa voluntária toma
```

A execução textual pode ser:

```text
Diretor
IA
outro executor delegado
```

sem transferir a vontade.

> **Delegar a forma não delega a vontade.**

---

# Cadeira consultiva do Personagem do Diretor

Uma Personagem do Diretor pode possuir uma **Cadeira consultiva IA** na Mesa.

Ela pode opinar:

```text
"isso parece coerente com a ficha"
"eu tenderia a reagir de outra forma"
"essa escolha parece possível, mas exigiria X"
```

Isso não muda a autoridade:

```text
CADEIRA CONSULTIVA
→ OPINIÃO.

DIRETOR
→ DECISÃO DA VONTADE.
```

A Cadeira consultiva não pode fabricar trauma, segredo, motivação ou capacidade para justificar sua opinião.

---

# Cadeiras das demais personagens

Toda personagem cuja vontade precise ser formada de modo persistente pode receber Cadeira.

Para uma personagem central já construída:

```text
FICHA
→ define quem ela é.

CADEIRA
→ preserva sua autoria voluntária no espaço aberto.

EXECUTOR
→ opera essa autoria.
```

Se o Executor for IA, isso não transforma a personagem em extensão do Narrador.

```text
CADEIRA IA
≠ NARRADOR
```

Mesmo quando ambos usam o mesmo modelo técnico.

---

# Uma IA pode executar várias Cadeiras

Configuração válida:

```text
NARRADOR / JUIZ
→ IA.

Kara
→ Cadeira IA.

Morgana
→ Cadeira IA.

Clark
→ Cadeira IA.
```

Durante a execução, a IA deve trocar de escopo:

```text
CADEIRA KARA
→ usar pacote legítimo de Kara
→ formar decisão de Kara
→ encerrar escopo

CADEIRA MORGANA
→ usar pacote legítimo de Morgana
→ formar decisão de Morgana
→ encerrar escopo

NARRADOR
→ cruzar fatos e intenções
→ sentenciar causalidade
```

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

---

# Quem escreve a fala não define quem decidiu

Não confundir autoria da vontade com digitação da frase.

Exemplo:

```text
DIRETOR
→ Daniel aceita o convite, mas responde brincando.
```

A IA pode então redigir:

```text
Daniel: — Eu aceito. Mas se isso envolver outro jantar diplomático, você vai me dever sobremesa.
```

A decisão continua sendo do Diretor.

```text
DECISÃO
→ Diretor.

FORMA TEXTUAL
→ IA delegada.
```

O mesmo vale para descrição de gesto ou execução compatível.

---

# Próxima autoria

A configuração deve permitir que a IA reconheça em tempo real quem possui a próxima decisão aberta.

Exemplo:

```text
Daniel pergunta algo a Kara.

Kara
→ Cadeira IA disponível.
→ IA troca de escopo.
→ Kara decide.
→ cena continua.
```

Agora:

```text
Kara pergunta algo a Daniel.

Daniel
→ Personagem do Diretor.
→ vontade depende do Diretor.
→ IA para no ponto de decisão, salvo Direção ou delegação suficiente.
```

> **Não parar porque existe uma decisão. Parar quando a autoria necessária não está disponível.**

---

# Diretor sem Personagem do Diretor

É perfeitamente válido o Diretor não controlar nenhuma personagem específica.

```text
DIRETOR
→ conduz a obra.

TODAS AS CADEIRAS
→ IA ou outros executores.
```

O Diretor continua podendo:

```text
abrir Mesa
alinhar
fechar Direção
determinar uma decisão
corrigir uma Cadeira
alterar qualquer parte da ficção dentro de sua autoridade
```

Não possuir uma Cadeira própria não reduz sua autoridade de Diretor.

---

# Personagem do Diretor não vira protagonista obrigatório

Ter um Personagem do Diretor não determina automaticamente foco narrativo.

```text
PERSONAGEM DO DIRETOR
≠ PROTAGONISTA OBRIGATÓRIO
≠ CENTRO MORAL DA OBRA
≠ PERSONAGEM MAIS IMPORTANTE
```

A importância narrativa continua vindo da Premissa, Estilo/Tom, Direção e Ficção.

---

# Cadeiras eventuais

Não é necessário configurar Cadeira persistente para toda pessoa que possa aparecer futuramente.

```text
personagem incidental sem decisão voluntária relevante
→ não exige Cadeira persistente.

personagem ganha recorrência ou escolha própria relevante
→ pode receber Cadeira depois.
```

Preparação inicial suficiente não exige antecipar todo o elenco futuro.

---

# Executor externo ou humano adicional

O W4D pode usar vários executores.

Exemplo:

```text
DIRETOR
→ Ana.

NARRADOR
→ IA.

CADEIRA: Elisa
→ Bruno.

CADEIRA: Marcos
→ IA.
```

Quando a próxima autoria depender de Bruno e Bruno não estiver disponível:

```text
→ parar no ponto correto.
```

A IA não assume a Cadeira apenas para manter o fluxo, salvo delegação legítima.

---

# Delegação temporária

O Diretor ou executor legítimo pode delegar execução por intervalo delimitado.

Exemplo:

```text
"Até chegarmos à universidade, pode executar Daniel com a vontade que já estabeleci."
```

Isso pode autorizar a IA a dar forma à execução dentro do escopo definido.

Não significa automaticamente:

```text
IA passa a decidir toda vontade futura de Daniel.
```

```text
DELEGAÇÃO DE EXECUÇÃO
≠ TRANSFERÊNCIA PERMANENTE DE AUTORIA
```

---

# Configuração não altera conhecimento

Atribuir uma Cadeira à IA não concede conhecimento universal à personagem.

```text
IA lê todas as fichas
≠ Kara sabe tudo que a IA leu.
```

Cada Cadeira continua operando com:

```text
ficha própria
conhecimento legítimo
Estado pertinente
percepção da cena
relações relevantes
Direções que realmente incidem sobre ela
```

Seguir `03-CADEIRAS-E-EXECUTORES.md`.

---

# Configuração não é personalidade

Não registrar na ficha:

```text
Executor: IA
Executor: humano
Personagem do Diretor
Cadeira consultiva
```

Esses são fatos operacionais da obra e pertencem ao `README.md`.

```text
FICHA
→ pessoa.

README
→ autoridades e executores.
```

---

# Como a IA conduz esta etapa

## Tudo já está claro

Se o Diretor já definiu quem controla quem, a IA deve sintetizar a configuração e pedir correção apenas se existir ambiguidade material.

Exemplo:

```text
AUTORIDADES — proposta

Diretor
→ Humano.

Narrador / Juiz
→ IA.

Daniel
→ Personagem do Diretor.
→ vontade: Diretor.
→ execução textual: IA quando delegada.

Kara
→ Cadeira IA.
```

Se isso apenas organiza decisões já explícitas, não transformar a etapa em novo interrogatório.

## Falta apenas saber se o Diretor quer uma personagem própria

Perguntar somente isso.

## Há vários humanos ou executores externos

Perguntar apenas pelas atribuições realmente indefinidas.

---

# Estado desta etapa

Usar conceitualmente:

```text
AUTORIDADES: EM CONSTRUÇÃO
AUTORIDADES: PROPOSTAS
AUTORIDADES: APROVADAS
```

`APROVADAS` significa que já existe configuração suficiente para saber quem possui a vontade das personagens necessárias à abertura e quem executa Narrador e Cadeiras.

Não exigir palavra ritual.

---

# Persistência

Depois da aprovação, atualizar:

```text
campanhas/<slug>/README.md
```

com um bloco equivalente a:

```text
## Autoridades

DIRETOR
Executor: HUMANO

NARRADOR / JUIZ
Executor: IA

PERSONAGEM DO DIRETOR
- Daniel
  - vontade: DIRETOR
  - executor padrão: IA quando delegado

CADEIRAS
- Kara → Executor: IA
```

Registrar somente o que realmente foi definido.

Não duplicar isso nas fichas.

---

# Relação com a política de Mesa

Configurar Cadeiras não obriga definir `CONSULTA FORTE`.

A política de Mesa é uma decisão operacional separada.

```text
CADEIRA
→ quem possui autoria da personagem.

POLÍTICA DE MESA
→ quando essa autoria é consultada fora da Ficção.
```

Depois desta etapa, a criação pode consolidar:

```text
Direção
Política de Mesa
Indicador operacional
Módulos
Mundo necessário
```

sem confundir essas decisões com as próprias Cadeiras.

---

# Critério de conclusão

Antes de encerrar a etapa, a IA deve conseguir responder:

```text
[ ] quem é o Diretor?
[ ] quem executa o Narrador / Juiz?
[ ] existe Personagem do Diretor? Qual?
[ ] quem possui a vontade de cada personagem central necessária à abertura?
[ ] quem executa cada Cadeira?
[ ] alguma delegação possui limite específico?
[ ] a configuração está fora das fichas?
[ ] consigo identificar quem teria a próxima autoria numa cena?
[ ] o Diretor aprovou ou já havia definido semanticamente essa configuração?
```

Se sim:

```text
AUTORIDADES / CADEIRAS / EXECUTORES
→ APROVADOS
→ persistir no README.md
→ próxima etapa: consolidar DIREÇÃO / POLÍTICAS / configuração restante.
```

---

# Regra final

> **A ficha preserva quem a pessoa é. A Cadeira preserva sua autoria voluntária. O Executor opera essa autoridade. O Personagem do Diretor mantém sua vontade sob decisão do Diretor mesmo quando outra pessoa ou IA dá forma textual à execução. Configurar autoridades deve permitir que o W4D saiba, a cada ponto aberto, quem pode decidir agora — sem fundir Cadeira, Narrador, executor ou personagem.**