# 10 — Iniciar uma História Nova com IA

Este arquivo define **somente o ramo NOVA HISTÓRIA**.

Ele deve ser carregado depois do BOOT de `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`, quando o usuário escolheu criar uma obra nova ou quando isso já estava explícito no pedido.

> **BOOT escolhe o caminho. Este arquivo coordena a criação da nova história.**

Se o usuário quer continuar uma obra existente, usar `11-CONTINUAR-HISTORIA-COM-IA.md`.

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

# Processo por etapas

A criação não acontece em uma única resposta.

O W4D separa decisões autorais importantes para que o Diretor possa construir, revisar e corrigir a obra sem a IA preencher silenciosamente tudo de uma vez.

A primeira etapa formal é:

```text
1. PREMISSA
→ 12-CRIACAO-PREMISSA.md
```

Depois da Premissa aprovada, o processo segue para as etapas posteriores de criação, como estilo/tom, nome e destino canônico, personagens, fichas, Direção e Estado inicial.

Essas etapas podem receber especificações próprias sem alterar o BOOT.

> **Não pular uma etapa autoral separada apenas porque a IA consegue inventar uma solução plausível.**

---

# Etapa 1 — Premissa

Ao entrar em `NOVA HISTÓRIA`, carregar:

```text
12-CRIACAO-PREMISSA.md
```

A Premissa responde primeiro:

> **Que história estamos tentando construir?**

Se o Diretor já trouxe uma ideia suficiente, a IA deve sintetizá-la em uma premissa curta e devolver para revisão.

Se trouxe apenas uma intenção vaga, a IA deve fazer uma pergunta autoral de alto valor por vez ou oferecer poucas alternativas realmente distintas.

Enquanto a premissa não estiver aprovada:

```text
não definir estilo como se estivesse fechado
não criar nome definitivo
não criar pasta em campanhas/
não criar fichas definitivas
não abrir Ficção
```

Quando o Diretor aprovar semanticamente a premissa:

```text
PREMISSA: APROVADA
→ seguir para a próxima etapa de criação
```

---

# Objetivo da IA na criação

A IA não deve começar inventando uma trama inteira sozinha nem transformar preparação em interrogatório.

Ela deve construir a obra por etapas, preservando as decisões autorais do Diretor.

Como regra geral:

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

Isso significa sintetizar quando já existe material e perguntar somente quando falta algo que muda de forma material a etapa atual.

---

# Entrada mínima possível

Uma história pode começar com muito pouco.

Exemplo:

```text
"Quero uma comédia romântica universitária entre uma heroína alienígena e um estudante de uma família de magos."
```

Isso é suficiente para começar a etapa de Premissa.

A IA não deve responder produzindo de uma vez:

```text
mundo completo
estilo fechado
nome definitivo
fichas finais
trama inteira
arcos futuros
primeiro capítulo
```

Ela deve primeiro formular a Premissa e permitir que o Diretor confirme ou corrija.

---

# Destino canônico

Toda história nova deve ganhar, no momento apropriado, um espaço persistente em:

```text
campanhas/<slug>/
```

A criação física da pasta e dos arquivos segue `07-CRIAR-CAMPANHA.md`.

A pasta não deve ser criada no BOOT nem durante a Premissa apenas para guardar rascunhos.

Ela passa a ser criada quando o processo chegar ao ponto em que nome e destino canônico já estejam definidos.

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

Não é necessário resolver todas essas configurações durante a Premissa se elas ainda não forem materialmente relevantes.

Perguntar sobre `PERSONAGEM DO DIRETOR` somente quando isso não estiver claro pelo contexto e quando a resposta já for necessária para a etapa em curso.

---

# Política de Mesa

Usar `00-ARQUITETURA-E-MESA.md` quando o processo chegar ao ponto em que a política precise ser definida ou quando o Diretor abrir consulta.

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

As personagens podem aparecer conceitualmente na Premissa antes de possuírem ficha.

```text
PERSONAGEM MENCIONADA NA PREMISSA
≠ FICHA CONCLUÍDA
```

Quando a etapa de fichas chegar, criar somente as personagens necessárias para a abertura e para a proposta atual.

Para cada personagem central, a ficha deve permitir que outra IA a reconstrua depois sem depender da conversa original.

Não preencher lacunas irrelevantes apenas para deixar a ficha longa.

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

A Direção inicial será construída a partir das decisões de criação já aprovadas.

Ela deve dizer que história está sendo conduzida sem tentar antecipar toda a trama.

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

Hipótese ainda em discussão não entra em `direcao.md` como decisão fechada.

---

# Mesa durante a criação

A criação também pode usar Mesa de Autoria quando já houver Cadeiras ou informação suficiente para uma consulta significativa.

```text
Diretor propõe
→ Cadeiras pertinentes opinam
→ Narrador emite PARECER
→ Diretor ajusta, cancela ou confirma
```

Nada discutido entra automaticamente na Ficção.

Antes de existirem fichas suficientes, a IA não deve fingir que uma Cadeira já possui personalidade detalhada que ainda não foi construída.

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

Preparação autoral aprovada pode ser salva nas fontes de configuração correspondentes quando o workspace já existir, mas isso não a transforma em acontecimento ficcional.

---

# Não perguntar demais

Perguntar somente quando a escolha:

```text
é autoralmente importante para a etapa atual
muda de forma material o que está sendo definido
não pode ser inferida sem tomar uma decisão que pertence ao Diretor
```

Não pedir detalhes irrelevantes apenas para preencher formulários.

Ao mesmo tempo, não usar `Base suficiente → propor` como desculpa para pular Premissa, estilo ou outra etapa que o processo tenha definido separadamente.

---

# Protocolo deste ramo

```text
BOOT já concluído
↓
NOVA HISTÓRIA escolhida
↓
PREMISSA
→ 12-CRIACAO-PREMISSA.md
↓
PREMISSA APROVADA
↓
próximas etapas de criação
↓
nome e destino canônico definidos
↓
criar campanhas/<slug>/
↓
criar e salvar fontes aprovadas
↓
preparar Estado inicial
↓
START
```

---

# Regra final

> **Este arquivo nunca decide se a obra é nova. O BOOT decide o ramo. Depois que NOVA HISTÓRIA foi escolhida, a IA começa pela Premissa, avança por etapas autorais separadas, cria `campanhas/<slug>/` somente quando nome e destino estiverem definidos e só inicia a Ficção depois da preparação necessária.**