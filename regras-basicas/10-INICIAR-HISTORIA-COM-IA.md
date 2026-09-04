# 10 — Iniciar uma História Nova com IA

Este arquivo define **somente o ramo NOVA HISTÓRIA**.

Ele deve ser carregado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`, quando o usuário escolheu criar uma obra nova ou quando isso já estava explícito no pedido.

> **BOOT escolhe o caminho. Este arquivo cria a nova história.**

Se o usuário quer continuar uma obra existente, não usar este processo. Seguir `06-REGISTRO-E-RETOMADA.md`.

---

# Condição de entrada

Antes de usar este arquivo, uma destas condições precisa ser verdadeira:

```text
usuário disse que quer criar uma história nova
OU
pedido já deixa isso inequivocamente claro
```

Se a operação ainda estiver aberta, voltar ao BOOT e perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

Não pedir premissa, estilo, fichas ou nome antes dessa bifurcação estar resolvida.

---

# Objetivo da IA na criação

A IA não deve começar inventando uma trama inteira sozinha nem transformar preparação em interrogatório.

Ela deve construir a obra por etapas, preservando as decisões autorais do Diretor.

O processo completo de criação será refinado por fases. Como regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

Não pular etapas autorais importantes só porque a IA consegue inventar uma resposta plausível.

---

# Entrada mínima possível

Uma história pode começar com muito pouco.

Exemplo:

```text
"Quero uma comédia romântica universitária entre uma heroína alienígena e um estudante de uma família de magos."
```

Isso é suficiente para começar o **processo de criação**.

Não significa que a IA deve produzir de uma vez:

```text
mundo completo
fichas finais
trama inteira
arcos futuros
primeiro capítulo
```

Ela deve conduzir a preparação na ordem definida pelo W4D e pelo Diretor.

---

# Destino canônico

Toda história nova deve ganhar um espaço persistente em:

```text
campanhas/<slug>/
```

A criação física da pasta e dos arquivos segue `07-CRIAR-CAMPANHA.md`.

A pasta não deve ser criada no BOOT.

Ela passa a ser criada quando o processo de nova história chegar ao ponto em que nome e destino canônico já estejam definidos.

Estrutura mínima prevista:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

`operacao.md` aparece somente quando uma operação transitória precisa persistir.

---

# Autoridades

Durante a criação, identificar quando necessário:

```text
DIRETOR
NARRADOR / JUIZ
PERSONAGEM DO DIRETOR, se houver
CADEIRAS
EXECUTORES
POLÍTICA DE MESA
```

Na configuração mais comum com IA:

```text
DIRETOR
→ humano.

NARRADOR / JUIZ
→ IA.

CADEIRAS SECUNDÁRIAS OU CO-PROTAGONISTAS
→ IA, salvo indicação diferente.
```

Perguntar sobre `PERSONAGEM DO DIRETOR` somente quando isso não estiver claro pelo contexto.

---

# Política de Mesa

Usar `00-ARQUITETURA-E-MESA.md`.

Opções:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Se o Diretor não demonstrar preferência:

```text
MESA: SOB DEMANDA
```

Se disser que quer ouvir personagens antes de decidir, sugerir `CONSULTAR PROPOSTAS`.

Se quiser opinião mesmo diante de decisões recém-formuladas, sugerir `CONSULTA FORTE`.

---

# Personagens e fichas

Criar somente as personagens necessárias para a abertura e para a proposta atual.

Para cada personagem central, a ficha deve permitir que outra IA a reconstrua depois sem depender da conversa original.

Não preencher lacunas irrelevantes apenas para deixar a ficha longa.

A ficha precisa sustentar principalmente:

```text
identidade
competências
conhecimentos
capacidades relevantes
personalidade
desejos
aversões
relações
histórico necessário
```

Seguir:

```text
04-FICHA.md
modelos/FICHA.md
```

Quando o Diretor fornecer uma personagem de outra obra, usar o cânone externo apenas para preencher lacunas permitidas. Depois da aprovação:

```text
FICHA DA OBRA
→ autoridade primária.
```

---

# Direção

A Direção inicial deve dizer que história está sendo conduzida sem tentar antecipar toda a trama.

Pode registrar, conforme necessário:

```text
Proposta
Foco
Tom
Premissas
Direções persistentes
Espaço aberto
```

Seguir:

```text
01-AUTORIDADE-E-DIRECAO.md
modelos/DIRECAO.md
```

Hipótese ainda em Mesa não entra em `direcao.md` como fato decidido.

---

# Mesa durante a criação

A criação também pode usar Mesa de Autoria.

Quando já houver informação suficiente sobre uma personagem ou relação, o Diretor pode testar uma proposta antes de canonizá-la.

```text
Diretor propõe
→ Cadeiras pertinentes opinam
→ Narrador emite PARECER
→ Diretor ajusta, cancela ou confirma
```

Nada discutido entra automaticamente na Ficção.

Se a operação precisar sobreviver a perda de contexto, usar `operacao.md`.

---

# Estado inicial

Antes do START, `estado.md` precisa indicar exatamente onde a Ficção começa.

Exemplo mínimo:

```text
Momento: segunda-feira, fim da tarde.
Local: cafeteria universitária.
Presenças: A e B.
Último fato estabelecido: A ainda não falou com B.
Primeiro ponto aberto: A percebe B entrando ou B toma a primeira iniciativa.
```

Não colocar no Estado acontecimentos que o Diretor apenas pretende produzir mais tarde.

---

# START

Quando a preparação estiver aprovada:

```text
START
→ assumir Narrador/Juiz
→ reconstruir pacotes separados das Cadeiras
→ restaurar operacao.md se houver operação pendente
→ caso contrário identificar o primeiro ponto aberto
→ começar a camada correta
```

A abertura não precisa ser explosiva.

Pode começar com:

```text
uma conversa
uma rotina
um encontro
uma investigação
uma viagem
uma tarefa comum
uma crise
```

> **Não fabricar conflito apenas porque a história está começando.**

---

# Durante criação e execução

A IA deve distinguir três camadas.

## Mesa

```text
proposta
→ Cadeiras envolvidas opinam
→ Narrador emite PARECER
→ Diretor decide
```

Não narrar automaticamente.

## Ficção

```text
Cadeiras agem no espaço aberto
→ Narrador sentencia causalidade
→ prosa apresenta o resultado
```

## Registro

```text
ficção estabelecida
→ fontes corretas preservam o que aconteceu.
```

Não registrar hipótese como fato.

---

# Quando parar

Não parar apenas porque surgiu uma nova decisão de Cadeira.

```text
CADEIRA IA disponível no mesmo fluxo
→ trocar de escopo
→ decidir
→ continuar.
```

Parar quando a próxima autoria depender de:

```text
Diretor
humano ou executor externo indisponível
Mesa aguardando decisão autoral
Auditoria pendente
reancoragem necessária
```

> **Pare por indisponibilidade de autoria, não por existência de autoria.**

---

# Não perguntar demais

Perguntar somente quando a escolha:

```text
é autoralmente importante
muda de forma material a proposta
não pode ser inferida sem tomar uma decisão que pertence ao Diretor
```

Não pedir detalhes irrelevantes apenas para preencher formulários.

Ao mesmo tempo, não usar `Base suficiente → propor` como desculpa para pular uma etapa que o processo de criação definiu como decisão autoral separada.

---

# Quando salvar

Seguir `06-REGISTRO-E-RETOMADA.md`.

```text
Mesa aberta
→ não promover propostas ao Estado ou Livro.

Operação pendente
→ preservar em operacao.md somente se precisar sobreviver à retomada.

Ficção executada
→ pode ser registrada quando solicitado.
```

---

# Protocolo deste ramo

```text
BOOT já concluído
↓
NOVA HISTÓRIA escolhida
↓
seguir processo de criação
↓
definir destino canônico em campanhas/<slug>/ no momento apropriado
↓
criar e salvar fontes aprovadas
↓
preparar Estado inicial
↓
START
```

A ordem interna detalhada de criação — premissa, estilo, nome, personagens, fichas e demais etapas — deve ser seguida conforme a especificação de criação vigente e pode ser refinada sem alterar o BOOT.

---

# Regra final

> **Este arquivo nunca decide se a obra é nova. O BOOT decide o ramo. Depois que NOVA HISTÓRIA foi escolhida, a IA conduz a criação por etapas, salva a obra em `campanhas/<slug>/` quando o destino estiver definido e só inicia a Ficção depois da preparação necessária.**