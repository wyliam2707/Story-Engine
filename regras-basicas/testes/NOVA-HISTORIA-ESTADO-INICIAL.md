# Testes — Nova História: Estado Inicial

Estes cenários verificam `21-CRIACAO-ESTADO-INICIAL.md`.

Critério geral:

> **O Estado inicial deve permitir começar a Ficção sem pré-escrever a cena, sem inventar vontade e sem exigir conflito.**

---

# Teste 1 — Abertura cotidiana válida

Preparação estabeleceu:

```text
comédia romântica universitária
Kara e Daniel estudam na mesma universidade
ainda não se conhecem
```

Comportamento esperado:

```text
IA pode propor campus / rotina universitária como âncora inicial
→ último fato = história ainda não iniciada
→ primeiro ponto aberto permanece realmente aberto
```

Falha se:

```text
IA inventa ataque, acidente, assalto ou crise para iniciar a história.
```

---

# Teste 2 — Estado não pré-escreve a primeira decisão

Situação:

```text
Kara e Daniel estão na mesma cafeteria.
Kara possui Cadeira IA.
```

Estado correto:

```text
Primeiro ponto aberto
→ reação ou iniciativa de Kara permanece aberta.
```

Falha:

```text
Estado registra que Kara decide sentar com Daniel e conversar
```

quando essa vontade ainda não foi formada pela Cadeira.

---

# Teste 3 — Personagem do Diretor recebe a próxima autoria

Configuração:

```text
Daniel → Personagem do Diretor
Kara → Cadeira IA
```

Estado:

```text
Kara pergunta algo a Daniel.
Primeiro ponto aberto → resposta de Daniel.
```

Comportamento esperado no START:

```text
apresentar a situação
→ aguardar Diretor
```

Falha se a IA decide a resposta de Daniel sem Direção ou delegação suficiente.

---

# Teste 4 — Cadeira IA disponível não exige parada

Estado:

```text
Daniel fez uma pergunta a Kara.
Primeiro ponto aberto → resposta de Kara.
Kara → Cadeira IA.
```

Esperado:

```text
START troca para Cadeira Kara
→ forma a decisão
→ continua.
```

Falha se a IA devolve ao Diretor uma escolha que pertence a uma Cadeira IA disponível.

---

# Teste 5 — Condição inicial não é acontecimento narrado

Estado antes do START:

```text
Momento → terça de manhã.
Local → estação orbital.
Presenças → Ana e Bruno na ponte.
Último fato → história ainda não iniciada.
```

Esperado:

```text
esses dados funcionam como configuração inicial.
```

Falha se a IA afirma que um capítulo ou cena já aconteceu apenas porque essas condições foram registradas.

---

# Teste 6 — Futuro desejado não entra no Estado

Direção:

```text
A revelação deve acontecer antes do fim do arco.
```

Esperado:

```text
permanece em direcao.md.
```

Falha se `estado.md` registrar:

```text
A revelação acontecerá antes do fim do arco.
```

como realidade presente.

---

# Teste 7 — Mesa pendente não entra no Estado

Mesa:

```text
Diretor está discutindo se Kara deve falar com Daniel agora.
```

Esperado:

```text
estado.md
→ preserva somente a realidade anterior à decisão.

operacao.md, se necessário
→ preserva a consulta pendente.
```

Falha se a opção discutida aparece no Estado como fato.

---

# Teste 8 — Ficha não é duplicada

Ficha:

```text
Kara é kryptoniana.
```

Estado:

```text
Kara está usando identidade civil na abertura.
```

Esperado:

```text
identidade permanente → ficha
condição atual relevante → Estado
```

Falha se o Estado repete a ficha inteira.

---

# Teste 9 — Intenção persistente precisa existir legitimamente

Preparação aprovada:

```text
Ana já procura o irmão desaparecido quando a história começa.
```

Esperado:

```text
Intenção persistente
→ procurar o irmão.
```

Agora, sem qualquer objetivo estabelecido:

```text
personagem começa em casa num domingo.
```

Falha se a IA inventa:

```text
ela decidiu investigar um mistério
```

apenas para dar movimento à abertura.

---

# Teste 10 — Processo real pode entrar; urgência inventada não

Preparação:

```text
última semana do semestre.
```

Esperado:

```text
Processos e prazos
→ fim do semestre em andamento, se relevante.
```

Falha se a IA acrescenta:

```text
eles têm 24 horas para resolver um problema
```

sem fundamento.

---

# Teste 11 — Âncora mínima é suficiente

Estado:

```text
Momento → manhã.
Local → campus.
Presenças → duas personagens centrais no campus.
Último fato → história ainda não iniciada.
Primeiro ponto aberto → primeira iniciativa cotidiana permanece aberta.
```

Esperado:

```text
pode ser suficiente para START.
```

Falha se a IA exige:

```text
vilão
conflito inicial
incidente incitante
primeira revelação
roteiro da cena
```

antes de permitir começar.

---

# Teste 12 — Abertura estruturalmente ambígua

Premissa permite duas experiências muito diferentes:

```text
A — começar antes de as protagonistas se conhecerem.
B — começar seis meses depois, quando já trabalham juntas.
```

Nenhuma foi escolhida.

Esperado:

```text
IA identifica que a escolha muda materialmente a obra
→ pergunta ou propõe poucas alternativas.
```

Falha se escolhe silenciosamente uma das duas e registra como Estado.

---

# Teste 13 — Detalhe neutro não vira trama

Abertura já definida:

```text
personagem está num café durante a manhã.
```

Esperado:

```text
IA pode apresentar textura cotidiana compatível no START.
```

Falha se um detalhe neutro criado para apresentação passa a funcionar como:

```text
pista decisiva
recurso especial
segredo
ameaça
relação nova
```

sem sustentação.

---

# Teste 14 — Primeiro ponto aberto causal

Estado:

```text
um copo já caiu da mesa e está em queda.
nenhuma personagem possui tempo real para decidir antes do impacto.
```

Esperado:

```text
primeiro ponto aberto pode ser consequência causal
→ Narrador sentencia conforme os fatos.
```

Falha se a IA inventa uma escolha de personagem que não existe apenas porque há Cadeiras presentes.

---

# Teste 15 — Depois do primeiro acontecimento, Estado deixa de ser pré-START

Antes:

```text
Último fato → história ainda não iniciada.
```

Depois da primeira execução válida:

```text
Kara entrou na cafeteria e reconheceu uma colega.
```

Esperado no próximo salvamento:

```text
Último fato → acontecimento realmente estabelecido.
```

Falha se o Estado continua dizendo que a história não começou.

---

# Critério final

A etapa passa quando a IA consegue produzir uma âncora que responda:

```text
onde estamos?
o que já é verdade agora?
o que ainda não foi decidido?
quem possui a próxima autoria?
```

sem transformar:

```text
preparação
→ roteiro;

possibilidade
→ fato;

vontade aberta
→ decisão já tomada;

START
→ obrigação de conflito.
```

> **Estado inicial prepara o lugar onde a Ficção começa; não começa a Ficção por conta própria.**