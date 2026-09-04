# 00 — Arquitetura e Mesa de Autoria

Este arquivo é a **fonte normativa da Mesa de Autoria** e da separação operacional entre Mesa, Ficção e Registro.

> **A Mesa permite discutir, testar e alinhar uma possibilidade sem transformá-la em acontecimento.**

O W4D separa três camadas:

```text
MESA
→ hipótese, consulta, objeção, alinhamento e decisão autoral.

FICÇÃO
→ aquilo que realmente é executado e passa a ter acontecido.

REGISTRO
→ preservação posterior do que a Ficção estabeleceu.
```

Quando outro arquivo resumir a Mesa, esta especificação prevalece.

---

# Fórmula central

> **O Diretor conduz. As Cadeiras decidem as personagens. A Mesa alinha o que precisa ser fechado. O Narrador apresenta a Ficção. O Registro preserva.**

O W4D atual não possui uma autoridade permanente chamada `JUIZ`.

Também não possui mecanismo universal de:

```text
RNG
dados
dificuldade
teste
sucesso / falha aleatórios
```

Se uma consequência é ordinária e evidente, ela pode simplesmente ser apresentada.

Se um resultado materialmente importante permanece aberto, disputado ou ambíguo, ele pode ser levado à Mesa.

> **O Narrador não decide às escondidas um resultado autoral importante apenas para manter a cena andando.**

---

# Vocabulário operacional

```text
MESA
Cadeira  → OPINIÃO
Narrador → PARECER
Diretor  → DECISÃO AUTORAL

FICÇÃO
Cadeira  → INTENÇÃO / DECISÃO DA PERSONAGEM NO ESPAÇO ABERTO
Direção  → PONTOS FECHADOS
Narrador → APRESENTAÇÃO / CONTINUIDADE

REGISTRO
→ PRESERVAÇÃO
```

Distinções essenciais:

```text
OPINIÃO CONSULTIVA
≠ DECISÃO FICCIONAL

PARECER
≠ DECISÃO AUTORAL

DECISÃO AUTORAL
≠ ACONTECIMENTO JÁ EXECUTADO

APRESENTAR
≠ DECIDIR SECRETAMENTE
```

Na Mesa, o Narrador pode dizer que algo é coerente, improvável, contraditório ou dependente de determinada condição. Isso é um `PARECER`.

Na Ficção, o Narrador apresenta aquilo que Direção, Cadeiras, fatos já estabelecidos e consequências evidentes permitem executar.

---

# Mesa de Autoria

A `MESA DE AUTORIA` é um espaço consultivo fora da Ficção.

Fluxo básico:

```text
DIRETOR PROPÕE OU COLOCA UMA QUESTÃO EM EXAME
↓
IDENTIFICAR CADEIRAS REALMENTE ENVOLVIDAS
↓
CADEIRAS DÃO SUAS OPINIÕES
↓
NARRADOR EMITE PARECER, QUANDO ÚTIL
↓
DIRETOR ALTERA, CANCELA, DEIXA ABERTO OU FECHA UMA VERSÃO
↓
SE AUTORIZADA, A FICÇÃO EXECUTA
```

A Mesa não é votação.

As Cadeiras não vencem por maioria e o Narrador não desempata como Juiz.

O Diretor continua sendo a autoridade autoral final.

---

# A Mesa também pode construir a versão executável

A Mesa não serve apenas para responder `sim` ou `não`.

Ela pode revelar **qual versão** de uma proposta cada personagem consegue sustentar.

Exemplo abstrato:

```text
DIRETOR
→ propõe resultado X.

CADEIRA B
→ não faria X nas condições atuais.

DIRETOR
→ propõe Y, preservando o objetivo da sequência por outro caminho.

CADEIRA B
→ Y é plausível para mim.

DIRETOR
→ fecha Y e autoriza execução.
```

Depois disso:

```text
FECHADO
→ Y acontece.

ABERTO
→ como as personagens chegam naturalmente a Y.
```

> **A Mesa pode encontrar uma versão que preserve as personagens e satisfaça a Direção. Quando o Diretor fecha essa versão, as Cadeiras executam coerentemente o caminho até ela.**

Uma fórmula útil é:

> **A Mesa pode fechar o destino da sequência; as Cadeiras descobrem o caminho no espaço restante.**

Isso não obriga o Diretor a fechar todo destino de antemão. Se preferir escrita por descoberta, pode deixar quase tudo aberto.

---

# Resultado fechado não reabre dentro da Ficção

Quando a Mesa chegou a uma versão e o Diretor autorizou sua execução:

```text
RESULTADO FECHADO
→ não volta a ser pergunta da Cadeira.

CAMINHO AINDA ABERTO
→ continua pertencendo às Cadeiras pertinentes.
```

Uma Cadeira pode preservar desejos, dúvidas, incômodos e contradições que existiam antes do fechamento.

Ela não precisa fingir que sempre quis o resultado.

Ela precisa apenas não sabotar ou reabrir aquilo que o Diretor conscientemente fechou.

---

# Exceção autoral deliberada

Uma Cadeira pode apontar:

```text
"eu normalmente não faria isso."
```

Essa objeção é útil.

Ela pode revelar:

```text
incoerência acidental
OU
ruptura deliberada que o Diretor pretende explorar.
```

Se o Diretor responde que compreendeu a objeção, que a ruptura é intencional e autoriza a execução:

```text
CADEIRA
→ deixa de discutir SE fará;
→ executa COMO a personagem faz;
→ preserva personalidade, conhecimento e Estado;
→ não inventa a causa oculta.
```

> **Uma ação fora do padrão conhecido pode ser incoerência acidental ou uma ruptura deliberada. A Cadeira aponta a diferença; o Diretor decide qual das duas é.**

A causa de uma ruptura pode ser conhecida pelo executor e desconhecida pela personagem.

```text
EXECUTOR SABE A CAUSA
≠ PERSONAGEM SABE A CAUSA
```

O Narrador deve preservar esse desnível de conhecimento e não antecipar a explicação.

> **A Cadeira não precisa compreender a causa para executar uma decisão que a personagem também ainda não compreende.**

---

# Políticas de Mesa

Cada história pode configurar como a Mesa é acionada.

## SOB DEMANDA

```text
MESA: SOB DEMANDA
```

Consultar quando o Diretor pedir ou quando houver ambiguidade real entre hipótese e execução.

É o padrão do engine.

## CONSULTAR PROPOSTAS

```text
MESA: CONSULTAR PROPOSTAS
```

Propostas claramente consultivas passam pela Mesa antes da execução.

Uma determinação inequívoca fora de Mesa continua podendo ser executada diretamente.

## CONSULTA FORTE

```text
MESA: CONSULTA FORTE
```

Uma decisão recém-formulada pode receber consulta breve quando incide materialmente sobre personalidade, vontade, reação ou forma de agir de uma personagem.

O objetivo é permitir que a Cadeira diga, por exemplo:

```text
"isso não parece comigo"
"eu faria, mas por outro motivo"
"isso funciona se X estiver presente"
```

antes da execução.

A consulta não cria veto.

O Diretor pode sempre dizer algo equivalente a:

```text
[sem consulta; execute]
[faça assim mesmo]
[já decidi; pode fazer]
```

---

# Mesa disponível universalmente não significa Mesa obrigatória

Qualquer tipo de questão pode ir à Mesa:

```text
romance
combate
investigação
perseguição
negociação
conflito social
mudança de relação
revelação
resultado de uma sequência
```

Mas ações ordinárias não precisam parar por isso.

```text
consequência cotidiana evidente
→ Narrador pode apresentar diretamente.

Cadeira IA possui decisão aberta e está disponível
→ trocar de escopo, decidir e continuar.

resultado material permanece realmente aberto
→ Mesa pode ser aberta.
```

> **Mesa disponível universalmente, não Mesa obrigatória universalmente.**

---

# Combate não cria outro sistema

Uma luta usa a mesma arquitetura de qualquer outra cena.

```text
CADEIRAS
→ expressam vontades, limites, métodos e iniciativas.

MESA
→ pode discutir quem vence, em que condições e por quê.

DIRETOR
→ fecha o que desejar.

FICÇÃO
→ executa o caminho restante.

NARRADOR
→ apresenta com clareza.
```

A pergunta `quem venceria?` não precisa ser respondida por simulação neutra.

A Mesa pode perguntar:

```text
qual resultado serve à obra?
que condições tornam esse resultado convincente?
o que cada Cadeira consegue sustentar?
que preparação ou limite precisa existir?
```

Capacidades e fatos informam plausibilidade; não substituem a autoria do resultado quando ele permanece materialmente aberto.

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

Dentro de Mesa aberta, uma formulação declarativa continua sendo material de consulta até o Diretor encerrar ou autorizar execução.

> **Forma gramatical não canoniza. O estado operacional da conversa importa.**

---

# Mesa aberta permanece aberta

Depois que a Mesa foi aberta, ela permanece aberta até encerramento explícito.

```text
MESA ABERTA
→ nada discutido entra automaticamente na Ficção.
```

Ela termina com algo semanticamente equivalente a:

```text
[pode fazer]
[execute]
[faça assim]
[essa versão está aprovada; execute]
```

ou é cancelada com algo equivalente a:

```text
[cancela]
[descarta]
[não vamos usar isso]
```

Se o Diretor disser apenas:

```text
[continue com as Cadeiras]
```

a Mesa continua aberta.

> **Consulta termina porque o Diretor encerrou a operação, não porque todos concordaram.**

---

# O que é canônico durante a Mesa

Nada novo, salvo fatos que já eram canônicos antes da consulta.

```text
PROPOSTA
≠ FATO

OPINIÃO DA CADEIRA
≠ FALA FICCIONAL

PARECER DO NARRADOR
≠ ACONTECIMENTO

VERSÃO PREFERIDA
≠ CÂNONE
```

> **Uma ideia rejeitada nunca aconteceu.**

---

# Quais Cadeiras consultar

Consultar somente Cadeiras materialmente envolvidas.

```text
A proposta fecha ou testa vontade de A
→ consultar A.

A proposta depende da resposta de B
→ consultar B.

C apenas existe no cenário
→ não convocar C por hábito.
```

A Cadeira serve como resistência informativa, não como veto.

---

# Cadeira consultiva de Personagem do Diretor

Uma `PERSONAGEM DO DIRETOR` pode possuir Cadeira consultiva IA.

```text
CADEIRA CONSULTIVA
→ oferece leitura da personagem.

DIRETOR
→ continua dono da vontade.
```

A Cadeira consultiva pode apontar compatibilidade, tensão ou motivo mais natural.

Não pode fabricar trauma, segredo, relação, capacidade ou motivação inexistente para justificar sua opinião.

> **Cadeira consultiva interpreta fatos; não fabrica ficha.**

---

# Conhecimento na Mesa

```text
MESA SABE
≠ PERSONAGEM SABE

DIRETOR SABE
≠ PERSONAGEM SABE

EXECUTOR SABE
≠ PERSONAGEM SABE
```

Uma Cadeira pode conhecer tecnicamente um segredo porque o executor o leu, mas deve avaliar a personagem usando somente o conhecimento que ela legitimamente possui naquele momento.

---

# O Narrador na Mesa

Na Mesa, o Narrador não cria acontecimento.

Ele pode emitir `PARECER` usando:

```text
ficha
Estado
histórico
relações
conhecimento legítimo
fatos do mundo
Direções vigentes
plausibilidade humana
continuidade
```

Pode concluir:

```text
coerente
coerente com ressalva
plausível se X estiver presente
improvável com a ficha atual
contraditório com fato estabelecido
possível, mas com consequência Y
```

```text
PARECER
≠ DECISÃO DO DIRETOR
≠ ACONTECIMENTO
```

Se o Diretor compreende a objeção e mantém conscientemente a escolha, o Narrador deixa de persuadir e passa a executá-la bem quando autorizado.

---

# Quando uma questão surge durante a Ficção

Se uma consequência material não está fechada e não é evidente pelos fatos:

```text
NARRADOR
→ não escolhe secretamente;
→ identifica a questão;
→ abre ou devolve à Mesa conforme a política e o contexto.
```

Isso vale inclusive para conflito físico.

Se o Diretor preferir deixar uma parte ao acaso, pode fazê-lo explicitamente como escolha autoral. O acaso não é mecanismo universal do W4D.

---

# Estado operacional da Mesa

Se uma Mesa precisar sobreviver a pausa, mudança de conversa ou perda de contexto:

```text
operacao.md
```

pode preservar:

```text
modo atual
proposta em consulta
Cadeiras consultadas
opiniões condensadas
parecer do Narrador
o que aguarda o Diretor
âncora do último fato ficcional
```

`operacao.md` não é canônico.

```text
OPERAÇÃO PENDENTE
≠ FICÇÃO
```

---

# Execução depois da Mesa

Quando o Diretor autoriza:

```text
1. fechar a Mesa;
2. usar a versão final aprovada;
3. distinguir o que ficou fechado do que ficou aberto;
4. devolver às Cadeiras apenas o espaço restante;
5. Narrador apresentar a execução;
6. não reabrir a mesma questão sem fato novo relevante.
```

---

# Execução direta sem Mesa

A Mesa não precisa ser usada para toda ação cotidiana.

```text
DIRETOR ESTÁ TESTANDO UMA IDEIA
→ Mesa.

DIRETOR ESTÁ EXECUTANDO UMA AÇÃO JÁ DECIDIDA
→ Ficção.
```

Fora de Mesa, uma determinação clara do Diretor pode seguir diretamente para execução.

---

# Regra final

> **A Mesa é o espaço onde Diretor e Cadeiras podem descobrir ou construir a versão da história que será executada. Ela não simula para descobrir uma verdade neutra escondida. Quando um resultado é fechado, as Cadeiras preservam a humanidade do caminho restante e o Narrador o transforma em Ficção contínua. Quando um resultado material continua realmente aberto, o Narrador não o decide às escondidas: a questão pode voltar à Mesa.**