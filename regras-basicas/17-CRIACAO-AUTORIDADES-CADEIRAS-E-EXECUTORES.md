# 17 — Criação: Autoridades, Cadeiras e Executores

Este arquivo define a **sexta etapa autoral** do ramo `NOVA HISTÓRIA`. Ele entra em uso depois que as fichas iniciais necessárias estão suficientemente construídas em `16-CRIACAO-FICHAS.md`.

A definição normativa continua em:

```text
03-CADEIRAS-E-EXECUTORES.md
05-NARRADOR.md
24-CICLO-DE-AUTORIA.md
```

> **Primeiro existe a pessoa. Depois se define quem possui sua vontade e quem executa cada função.**

---

# O que esta etapa responde

```text
quem é o Diretor?
quem executa o Narrador?
alguma personagem pertence diretamente ao Diretor?
quais personagens possuem Cadeira persistente agora?
quem executa cada Cadeira?
como a Personagem do Diretor pode receber execução IA?
como as Cadeiras mantêm agendas e iniciativas próprias?
quem possui a próxima autoria quando a Ficção começar?
```

Não é uma etapa de personalidade ou de trama.

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

---

# Narrador não é Juiz

No W4D atual, configurar `NARRADOR` não cria uma autoridade de sentença.

```text
NARRADOR
→ na Mesa pode emitir Parecer quando houver questão real;
→ na Ficção apresenta continuidade e consequências evidentes;
→ não escolhe secretamente resultados materiais abertos;
→ não revisa a vontade das Cadeiras como segundo julgador.
```

Se um resultado importante continua aberto, pode voltar à Mesa quando necessário.

Workspaces antigos que tragam `NARRADOR / JUIZ` devem ser interpretados como rótulo legado e normalizados para `NARRADOR` quando houver atualização legítima.

---

# Autoridade e execução não são a mesma coisa

```text
AUTORIDADE
→ quem possui determinado espaço de decisão.

EXECUTOR
→ quem opera essa função na prática.
```

Exemplo:

```text
Daniel
→ PERSONAGEM DO DIRETOR
→ vontade pertence ao Diretor
→ execução textual pode ser IA quando delegada.
```

```text
DIRETOR DEFINE O QUE DANIEL QUER
≠ DIRETOR PRECISA ESCREVER TODA A PROSA DE DANIEL
```

Outro exemplo:

```text
Kara
→ Cadeira de personagem
→ Executor: IA.
```

A IA forma a vontade de Kara no espaço aberto porque recebeu sua Cadeira.

---

# Configuração mínima comum

```text
DIRETOR
→ HUMANO.

NARRADOR
→ IA.

CADEIRAS não atribuídas ao Diretor
→ IA.
```

Essa configuração pode ser usada como padrão quando o contexto não indicar outra coisa.

A IA **não deve escolher silenciosamente qual personagem pertence ao Diretor**.

Se isso ainda estiver aberto e já for necessário, perguntar apenas:

> **Você quer controlar diretamente alguma das personagens centrais, ou deixamos as Cadeiras delas com a IA?**

Informação já dada deve ser registrada, não perguntada novamente.

---

# Personagem do Diretor

```text
PERSONAGEM DO DIRETOR
→ vontade: DIRETOR.
```

Isso inclui o que quer, o que tenta, o que aceita, o que recusa, iniciativa voluntária e conteúdo de fala que dependa de escolha própria.

A execução textual pode ser delegada sem transferir vontade.

> **Delegar a forma não delega a vontade.**

A IA deve poder executar essa personagem com a mesma qualidade literária das demais, preenchendo falas, gestos, humor, flerte, métodos e pequenas ações compatíveis com o objetivo autorizado. Não deve deixá-la silenciosa por receio de executá-la, nem inventar novos objetivos ou compromissos.

---

# Cadeira consultiva da Personagem do Diretor

Uma Personagem do Diretor pode possuir Cadeira consultiva IA na Mesa.

```text
CADEIRA CONSULTIVA
→ JULGAMENTO / OPINIÃO.

DIRETOR
→ DECISÃO DA VONTADE.
```

A Cadeira pode apontar que uma proposta é coerente, estranha ou depende de determinada condição. Pode oferecer alternativas e sugerir uma forma natural de agir.

Não pode fabricar trauma, segredo, motivação, relação ou capacidade para justificar sua leitura.

O Diretor pode escolher uma alternativa ou dizer `faça como achar melhor`. A delegação vale para a questão em discussão, não para toda a agenda ou decisões futuras.

---

# Escopo de execução

A execução delegada deve respeitar objetivo, escopo e condição de parada quando pertinentes.

```text
OBJETIVO
→ o que o Diretor pretende realizar.

ESCOPO
→ quais escolhas, métodos e intervalos estão delegados.

CONDIÇÃO DE PARADA
→ quando devolver autoria ao Diretor.
```

Não exigir formulário. Inferir o que estiver claro e perguntar somente quando faltar algo decisivo.

Uma autorização para ir ao teatro não permite preencher automaticamente o resto do dia. Uma autorização para treinar durante a tarde permite desenvolver todo esse intervalo, incluindo rotina e transições ordinárias. `Só pare se receber visita` não autoriza inventar visita nem executar além do limite temporal ou material concedido.

---

# Cadeiras das demais personagens

```text
FICHA
→ quem a pessoa é.

CADEIRA
→ autoria voluntária no espaço aberto.

EXECUTOR
→ quem opera essa autoria.
```

```text
CADEIRA IA
≠ NARRADOR
```

Mesmo quando o mesmo modelo técnico executa ambos.

Na Mesa, a Cadeira oferece julgamento autoral concreto, não fala ficcional. Pode dizer que a personagem aceitaria, recusaria ou preferiria outra condição. Uma frase pode bastar. A IA não deve concordar por conveniência nem fabricar resistência para parecer independente.

---

# Uma IA pode executar várias Cadeiras e o Narrador

Configuração válida:

```text
NARRADOR → IA
Kara → Cadeira IA
Morgana → Cadeira IA
Clark → Cadeira IA
```

Fluxo por escopo:

```text
CADEIRA KARA
→ usar pacote legítimo de Kara
→ julgar ou decidir o espaço aberto de Kara
→ encerrar escopo

CADEIRA MORGANA
→ usar pacote legítimo de Morgana
→ julgar ou decidir o espaço aberto de Morgana
→ encerrar escopo

se surgir resultado material ainda aberto
→ Mesa, quando necessária

NARRADOR
→ apresentar fatos, decisões e continuidade autorizada
```

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

---

# Quem escreve a fala não define quem decidiu

```text
DIRETOR
→ Daniel aceita o convite, mas responde brincando.
```

A IA pode redigir a fala.

```text
DECISÃO
→ Diretor.

FORMA TEXTUAL
→ IA delegada.
```

O mesmo vale para pequenos gestos e execução compatível.

---

# Resultado fechado e Cadeiras

Quando a Mesa/Diretor fecha um resultado:

```text
RESULTADO
→ não volta a ser pergunta.

CAMINHO RESTANTE
→ continua distribuído entre as Cadeiras.
```

A configuração precisa permitir que o executor saiba quem ainda pode decidir cada parte do caminho, sem confundir o resultado fechado com vontade automática de todas as personagens.

---

# Ruptura deliberada

Uma Cadeira pode dizer na Mesa que uma decisão não corresponde ao padrão atual da personagem.

Se o Diretor reconhece isso como ruptura deliberada e confirma:

```text
CADEIRA
→ executa o ponto fechado;
→ preserva o que continua aberto;
→ não inventa causa oculta;
→ não continua usando a objeção como veto.
```

```text
EXECUTOR SABE MAIS
≠ PERSONAGEM SABE MAIS
```

A atribuição de executor deve preservar essa separação.

---

# Agendas e iniciativa própria

A Cadeira mantém compromissos, intenções, relações e disponibilidade próprios, mesmo fora da presença do protagonista. Na Mesa, a IA pode apresentar o que pretende fazer com a personagem durante um intervalo, permitindo que o Diretor alinhe a cena.

```text
Cadeira de Kara: O trabalho dela termina perto do almoço. Estou pensando em fazê-la visitar Daniel porque quer vê-lo.
Diretor: Então colocarei Daniel ensaiando no quintal.
Cadeira de Kara: Funciona. Ela pode chegar e observar antes de se anunciar.
Diretor: Pode fazer.
```

A personagem não conhece o ensaio apenas porque sua Cadeira conhece. Daniel não conhece a visita apenas porque o Diretor ouviu a intenção. A agenda não é roteiro imutável nem precisa preencher cada hora.

Compromissos e prazos persistentes pertencem ao Estado. Propostas ainda em discussão pertencem à Operação. Não salvar uma visita proposta como acontecida.

---

# Próxima autoria

A configuração deve permitir reconhecer em tempo real quem possui a próxima decisão aberta.

```text
Kara precisa decidir
+
Cadeira Kara = IA disponível
→ trocar de escopo
→ Kara decide
→ continuar dentro da execução autorizada.
```

```text
Daniel precisa decidir
+
Daniel = Personagem do Diretor
→ aguardar Diretor,
  salvo Direção ou delegação suficiente.
```

```text
resultado importante entre ações permanece aberto
→ Mesa pode ser aberta.
```

> **Não parar porque existe decisão; parar quando a autoria necessária não está disponível, quando a condição de parada é alcançada ou quando uma questão material aguarda fechamento autoral.**

---

# Diretor sem Personagem do Diretor

É válido o Diretor controlar nenhuma personagem específica.

```text
DIRETOR
→ conduz a obra.

TODAS AS CADEIRAS
→ IA ou outros executores.
```

Isso não reduz a autoridade do Diretor.

---

# Personagem do Diretor não é protagonista obrigatório

```text
PERSONAGEM DO DIRETOR
≠ PROTAGONISTA OBRIGATÓRIO
≠ CENTRO MORAL
≠ PERSONAGEM MAIS IMPORTANTE
```

Foco vem da Premissa, Direção e Ficção.

---

# Cadeiras eventuais

```text
personagem incidental sem decisão voluntária relevante
→ não exige Cadeira persistente.

personagem ganha recorrência ou escolha própria relevante
→ pode receber Cadeira depois.
```

Não antecipar todo o elenco futuro.

---

# Executor externo ou humano adicional

Exemplo:

```text
DIRETOR → Ana
NARRADOR → IA
CADEIRA Elisa → Bruno
CADEIRA Marcos → IA
```

Se a próxima autoria depender de Bruno e ele estiver indisponível, parar no ponto correto. A IA não assume a Cadeira sem delegação legítima.

---

# Delegação temporária

```text
"Até chegarmos à universidade, pode executar Daniel com a vontade que já estabeleci."
```

Isso autoriza forma dentro do escopo definido.

```text
DELEGAÇÃO DE EXECUÇÃO
≠ TRANSFERÊNCIA PERMANENTE DE AUTORIA
```

---

# Configuração não altera conhecimento

```text
IA lê todas as fichas
≠ Kara sabe tudo que a IA leu.
```

Cada Cadeira usa somente seu pacote legítimo.

```text
MESA SABE
≠ PERSONAGEM SABE
```

---

# Configuração não é personalidade

Não registrar na ficha:

```text
Executor: IA
Executor: humano
Personagem do Diretor
Cadeira consultiva
```

```text
FICHA
→ pessoa.

README
→ autoridades, funções e executores.
```

---

# Como a IA conduz esta etapa

Se tudo já estiver claro, apenas sintetizar.

Exemplo:

```text
AUTORIDADES: proposta

Diretor
→ Humano.

Narrador
→ IA.

Daniel
→ Personagem do Diretor
→ vontade: Diretor
→ execução textual: IA quando delegada.

Kara
→ Cadeira IA.
```

Perguntar somente pelas atribuições realmente indefinidas.

---

# Estado desta etapa

```text
AUTORIDADES: EM CONSTRUÇÃO
AUTORIDADES: PROPOSTAS
AUTORIDADES: APROVADAS
```

`APROVADAS` significa que já sabemos quem conduz, quem narra, quem possui a vontade de cada personagem necessária e quem executa cada Cadeira.

---

# Persistência

Depois da aprovação, atualizar:

```text
campanhas/<slug>/README.md
```

Exemplo:

```text
## Autoridades

DIRETOR
Executor: HUMANO

NARRADOR
Executor: IA

PERSONAGEM DO DIRETOR
- Daniel
  - vontade: DIRETOR
  - executor padrão: IA quando delegado

CADEIRAS
- Kara → Executor: IA
```

Não duplicar isso nas fichas.

---

# Relação com a política de Mesa

```text
CADEIRA
→ quem possui autoria da personagem.

POLÍTICA DE MESA
→ quando e como consultas são acionadas.
```

O padrão vigente é `MESA: CICLO OBRIGATÓRIO`, salvo escolha expressa diferente do Diretor. Configurar Cadeiras não escolhe automaticamente uma política alternativa.

---

# Critério de conclusão

A IA deve conseguir responder:

```text
[ ] quem é o Diretor?
[ ] quem executa o Narrador?
[ ] existe Personagem do Diretor?
[ ] quem possui a vontade de cada personagem central necessária?
[ ] quem executa cada Cadeira?
[ ] a execução delegada possui objetivo, escopo e parada reconhecíveis quando pertinentes?
[ ] a Personagem do Diretor pode ser executada sem silêncio artificial?
[ ] as Cadeiras conservam agendas e iniciativas próprias?
[ ] a configuração está fora das fichas?
[ ] consigo identificar a próxima autoria numa cena?
[ ] sei que Narrador não possui poder de Juiz nem revisa a vontade da Cadeira?
[ ] o ciclo obrigatório está disponível como padrão da obra?
```

Se sim:

```text
AUTORIDADES / CADEIRAS / EXECUTORES
→ APROVADOS
→ persistir no README.md
→ seguir para Direção.
```

---

# Regra final

> **A ficha preserva quem a pessoa é. A Cadeira preserva sua autoria voluntária e sua linha de vida própria. O Executor opera essa autoria. A Personagem do Diretor recebe execução plena dentro da delegação sem transferir sua vontade. O Narrador apresenta a Ficção e não funciona como Juiz. A configuração permite identificar quem pode decidir cada ponto aberto, como o ciclo obrigatório é aplicado e quando uma questão material deve voltar à Mesa.**
