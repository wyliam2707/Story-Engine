# 00 — Arquitetura e Mesa de Autoria

Este arquivo é a **fonte normativa da Mesa de Autoria** e da separação operacional entre Mesa, Ficção e Registro.

> **A Mesa permite discutir uma possibilidade sem transformá-la em acontecimento.**

O W4D separa três camadas:

```text
MESA
→ hipótese, consulta, objeção, alinhamento e decisão autoral.

FICÇÃO
→ aquilo que realmente é executado e passa a ter acontecido.

REGISTRO
→ preservação posterior do que a ficção já estabeleceu.
```

Quando outro arquivo resumir a Mesa, esta especificação prevalece para o funcionamento operacional.

---

# Vocabulário operacional

As mesmas funções atuam de formas diferentes conforme a camada.

```text
MESA
Cadeira  → OPINIÃO
Narrador → PARECER
Diretor  → DECISÃO AUTORAL

FICÇÃO
Cadeira  → INTENÇÃO / DECISÃO DA PERSONAGEM
Narrador → SENTENÇA CAUSAL
Prosa    → APRESENTAÇÃO

REGISTRO
→ PRESERVAÇÃO
```

Isso evita uma confusão importante:

```text
PARECER
≠ SENTENÇA

OPINIÃO CONSULTIVA
≠ DECISÃO FICCIONAL

DECISÃO AUTORAL
≠ ACONTECIMENTO JÁ EXECUTADO
```

Na Mesa, o Narrador pode dizer que algo é coerente, improvável ou contraditório. Isso é um **parecer** para ajudar o Diretor.

Na Ficção, depois que autoridades, fatos e decisões foram cruzados, o Narrador estabelece o que aconteceu. Isso é uma **sentença**.

---

# Mesa de Autoria

A `MESA DE AUTORIA` é um modo consultivo fora da ficção.

Ela existe para que o Diretor possa testar uma ideia contra as personagens antes de decidir se quer realmente usá-la.

Fluxo padrão:

```text
DIRETOR PROPÕE OU APRESENTA UMA DECISÃO PARA EXAME
↓
IDENTIFICAR CADEIRAS REALMENTE ENVOLVIDAS
↓
CADA CADEIRA DÁ SUA OPINIÃO
↓
NARRADOR EMITE PARECER
↓
DIRETOR DECIDE
```

A decisão final pode ser:

```text
cancelar
alterar
testar outra versão
pedir nova consulta
confirmar e executar
```

A Mesa não é votação. Não vence a opção que recebe mais concordâncias. Cada Cadeira responde a partir de sua própria lógica e o Diretor continua responsável pela decisão autoral final.

---

# Políticas de Mesa

Cada história pode configurar como a Mesa é acionada.

## SOB DEMANDA

```text
MESA: SOB DEMANDA
```

Consultar somente quando o Diretor pedir ou quando houver ambiguidade real entre hipótese e execução.

## CONSULTAR PROPOSTAS

```text
MESA: CONSULTAR PROPOSTAS
```

Quando o Diretor estiver claramente propondo uma ação, reação, motivação ou trajetória para avaliação, consultar as Cadeiras envolvidas antes de executar.

Uma determinação inequívoca fora de Mesa continua sendo executada normalmente.

## CONSULTA FORTE

```text
MESA: CONSULTA FORTE
```

É permitido oferecer uma consulta breve **mesmo quando a formulação do Diretor soa como determinação**, se a decisão disser respeito de modo material à personalidade, vontade, reação ou forma de agir de uma personagem.

O objetivo é permitir que o Diretor perceba algo como:

```text
"isso não parece comigo"
"eu faria, mas por outro motivo"
"isso funciona somente se X estiver presente"
```

antes da execução.

A consulta continua sem poder de veto.

O Diretor pode sempre dizer algo semanticamente equivalente a:

```text
[sem consulta; execute]
[faça assim mesmo]
[já decidi; pode fazer]
```

Nesse caso, a Mesa fecha ou é pulada e a determinação segue para a Ficção.

Se a história não registrar política própria, usar `SOB DEMANDA` como padrão seguro.

---

# Entrar na Mesa

A Mesa pode ser aberta explicitamente por frases como:

```text
[o que vocês acham?]
[consulte as Cadeiras]
[vamos testar uma ideia]
[e se A fizer X?]
[quero ouvir A e B antes de decidir]
```

Também pode ser reconhecida semanticamente conforme a política ativa.

Exemplo:

```text
"acho que A poderia entrar dançando"
```

é proposta quando o contexto é consultivo.

Dentro de uma Mesa já aberta, uma formulação declarativa também pode continuar sendo apenas hipótese:

```text
"A entra dançando na sala"
```

> **Forma gramatical não canoniza. O estado operacional da conversa importa.**

---

# Mesa aberta e determinação

Esta regra resolve a precedência entre `00-ARQUITETURA-E-MESA.md` e `01-AUTORIDADE-E-DIRECAO.md`.

Fora da Mesa:

```text
[faça X]
→ DETERMINAÇÃO
→ executar X conforme a autoridade normal.
```

Dentro de uma Mesa aberta:

```text
formulação de X
→ continua sendo material de consulta
```

**até que o Diretor também encerre a Mesa ou autorize a execução.**

Isso pode acontecer na mesma frase:

```text
"então faça X; pode executar"
```

ou depois:

```text
"X parece melhor."
→ ainda pode ser preferência de Mesa.

"pode fazer."
→ fecha a Mesa e autoriza execução.
```

> **Mesa aberta prevalece sobre a forma declarativa; autorização de execução encerra a consulta.**

Uma história com `CONSULTA FORTE` pode inclusive consultar uma determinação recém-formulada antes da execução, salvo quando o Diretor mandar seguir sem consulta.

---

# A Mesa é persistente até ser encerrada

Depois que a Mesa foi aberta, ela **permanece aberta**.

A IA não deve responder a uma consulta e depois continuar a cena por conta própria.

```text
MESA ABERTA
→ nada discutido entra automaticamente na ficção.
```

Ela termina quando o Diretor fecha a operação com algo semanticamente equivalente a:

```text
[pode fazer]
[execute]
[faça assim]
[essa versão está aprovada; execute]
[volte para a ficção e use isso]
```

ou cancela com algo como:

```text
[cancela]
[deixa como estava]
[descarta essa ideia]
[não vamos usar isso]
```

Se o Diretor disser apenas:

```text
[continue com as Cadeiras]
```

então a Mesa continua aberta.

> **Consulta não termina porque o Narrador respondeu. Termina porque o Diretor decidiu encerrar a operação.**

---

# O que é canônico durante a Mesa

Nada novo, salvo se o Diretor estiver apenas consultando fatos que já eram canônicos.

```text
PROPOSTA
≠ FATO

REAÇÃO CONSULTIVA DA CADEIRA
≠ FALA QUE A PERSONAGEM REALMENTE DISSE

PARECER DO NARRADOR
≠ ACONTECIMENTO

VERSÃO PREFERIDA PELA MESA
≠ CÂNONE
```

Somente depois da autorização de execução a versão escolhida entra na ficção.

Se a proposta for descartada, ela desaparece do fluxo canônico.

> **Uma ideia rejeitada nunca aconteceu.**

---

# Quais Cadeiras consultar

Consultar somente as Cadeiras cuja personalidade, vontade, interpretação ou reação seja materialmente relevante.

```text
A faz uma proposta sobre si mesma
→ Cadeira de A pode opinar.

A proposta afeta diretamente B
→ Cadeira de B pode opinar.

C está apenas disponível, mas não tem relação material com a questão
→ não convocar C.
```

Não convocar personagens apenas para aumentar o número de opiniões.

---

# Cadeira consultiva de Personagem do Diretor

Mesmo quando a vontade de uma personagem pertence ao Diretor, o sistema pode abrir uma `CADEIRA CONSULTIVA` para ela.

Isso não transfere a vontade da personagem para a IA.

A função é apenas responder:

```text
essa proposta parece compatível comigo?
que parte combina comigo?
que parte soa falsa?
que motivo seria mais natural?
como eu tenderia a receber essa situação?
```

```text
CADEIRA CONSULTIVA DO PERSONAGEM DO DIRETOR
→ oferece leitura.

DIRETOR
→ continua dono da vontade.
```

A Cadeira consultiva também não ganha poder para inventar passado, trauma, segredo, relação, capacidade ou motivação inexistente apenas para justificar sua opinião.

> **Cadeira consultiva interpreta fatos; não fabrica ficha.**

---

# Conhecimento na Mesa

A Mesa pode conhecer mais do que cada personagem.

```text
MESA SABE
≠ PERSONAGEM SABE

DIRETOR SABE
≠ PERSONAGEM SABE

EXECUTOR SABE
≠ PERSONAGEM SABE
```

Se o Diretor revelar um segredo durante a consulta, a Cadeira pode avaliar a hipótese como executor, mas deve formar sua opinião sobre a reação ficcional usando somente o conhecimento que a personagem legitimamente possuiria naquele momento.

Exemplo:

```text
MESA
→ sabe que B é o assassino.

PERSONAGEM A
→ ainda não descobriu isso.

CADEIRA DE A
→ não pode usar esse segredo para decidir como A reagiria agora.
```

---

# Como uma Cadeira responde na Mesa

A resposta deve ser curta e útil. Ela não precisa encenar uma cena inteira.

Formato recomendado:

```text
### Resultado da consulta

**A:** faria; combina com seu humor e com o Estado atual.

**B:** acharia estranho; interpretaria como provocação se houvesse contexto suficiente.

**Narrador:** coerente com ressalva X / incoerente por Y / depende da condição Z.
```

A Cadeira pode discordar do Diretor.

Isso é uma função desejada, não uma falha.

> **A Cadeira serve como resistência informativa, não como veto.**

---

# O Narrador na Mesa

Na Mesa, o Narrador não narra a cena e não produz sentença ficcional.

Ele emite `PARECER` usando, quando pertinentes:

```text
ficha
Estado
histórico
relações
conhecimento legítimo
causalidade
posição e oportunidade
Direções vigentes
plausibilidade humana
```

Pode concluir, por exemplo:

```text
coerente
coerente com ressalva
plausível se X estiver presente
improvável com a ficha atual
contraditório com fato estabelecido
possível, mas produziria consequência Y
```

```text
PARECER DO NARRADOR
≠ DECISÃO DO DIRETOR
≠ SENTENÇA DA FICÇÃO
```

Se o Diretor mantém conscientemente uma escolha que o Narrador considera estranha, o Narrador executa depois da autorização e preserva as consequências.

---

# Quando a proposta muda durante a consulta

Se o Diretor altera a ideia:

```text
VERSÃO A
→ consultada.

DIRETOR MUDA PARA VERSÃO B
→ consultar novamente somente os pontos e Cadeiras materialmente afetados.
```

Não é necessário repetir toda a Mesa quando a alteração é pequena e não muda nenhuma leitura relevante.

---

# Estado operacional da Mesa

Mesa, Auditoria e outras operações pendentes podem precisar sobreviver a perda de contexto, troca de conversa ou checkpoint.

Essas informações **não pertencem a `estado.md`**, porque não são realidade ficcional.

Quando necessário, usar:

```text
operacao.md
```

seguindo `modelos/OPERACAO.md`.

Ele pode preservar:

```text
modo atual
proposta em consulta
Cadeiras consultadas
opiniões condensadas
parecer do Narrador
o que está aguardando o Diretor
âncora do último fato ficcional
```

`operacao.md` é operacional, não canônico.

```text
OPERAÇÃO PENDENTE
≠ FICÇÃO
```

Quando a operação terminar, limpar ou remover seu conteúdo transitório conforme `06-REGISTRO-E-RETOMADA.md`.

---

# Execução depois da Mesa

Quando o Diretor diz `pode fazer`, `execute` ou equivalente:

```text
1. fechar a Mesa;
2. usar a versão final aprovada;
3. retornar às regras normais de autoridade e resolução;
4. executar a ficção;
5. não reabrir a mesma consulta sem fato novo relevante.
```

A partir desse ponto, as Cadeiras voltam a ser Cadeiras ficcionais no espaço que ainda permanece aberto.

A consulta anterior não precisa ser repetida dentro da prosa.

---

# Execução direta sem Mesa

A Mesa não precisa ser usada para toda ação cotidiana.

Fora de uma consulta aberta, o Diretor pode executar diretamente sua própria personagem ou emitir uma determinação clara conforme `01-AUTORIDADE-E-DIRECAO.md`.

Também pode dizer explicitamente:

```text
[sem consulta; faça X]
```

Nesse caso, executar conforme a autoridade normal.

A distinção prática é:

```text
DIRETOR ESTÁ TESTANDO UMA IDEIA
→ Mesa.

DIRETOR ESTÁ ESCREVENDO / EXECUTANDO UMA AÇÃO JÁ DECIDIDA
→ Ficção.
```

Quando houver dúvida real sobre qual dos dois está acontecendo, perguntar de forma curta em vez de canonizar uma hipótese por engano.

---

# Exemplo genérico

O Diretor propõe:

```text
A começa a dançar no jardim.
```

A Mesa está aberta.

```text
CADEIRA DE A
→ "sem motivo, isso não parece comigo; eu poderia fazer uma dança deliberadamente ridícula para provocar alguém."

CADEIRA DE B
→ "eu acharia engraçado se entendesse a provocação; sem isso, pareceria aleatório."

NARRADOR — PARECER
→ "como ação gratuita, considero incoerente; como provocação consciente, considero plausível."
```

O Diretor pode dizer:

```text
"é, ficou ridículo. Cancela."
```

Resultado:

```text
NADA ACONTECEU NA FICÇÃO.
```

Ou:

```text
"faça como provocação deliberada. Pode executar."
```

Resultado:

```text
A versão ajustada segue para a Ficção.
```

---

# Regra final

> **Na Mesa, o Diretor experimenta; as Cadeiras opinam como intérpretes das personagens; o Narrador emite parecer; nada acontece ainda. A política de Mesa define quando a consulta é acionada. Uma Mesa aberta permanece aberta até o Diretor cancelar ou autorizar execução. Quando ele confirma, a ficção volta a operar por decisões, fatos e sentença causal.**
