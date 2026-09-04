# 21 — Criação: Estado Inicial

Este arquivo define a **décima etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que Premissa, Estilo/Tom, personagens necessárias, fichas, autoridades, Direção, políticas e Mundo Necessário já estão suficientes para a abertura.

O modelo persistente continua em:

```text
modelos/ESTADO.md
```

A definição geral de Estado e Registro continua em:

```text
06-REGISTRO-E-RETOMADA.md
```

Esta etapa define **como a IA prepara o ponto de entrada da Ficção sem escrever a primeira cena antes do START**.

> **Estado inicial não é roteiro da primeira cena. É a âncora de realidade a partir da qual a Ficção pode começar.**

---

# O que esta etapa responde

O Estado inicial precisa permitir responder:

> **Onde estamos quando a Ficção abrir, o que já é verdade nesse instante e qual é a primeira coisa que continua aberta?**

Normalmente basta preservar, quando pertinente:

```text
momento
local principal
presenças e posições relevantes
condições temporárias já existentes
intenções persistentes já estabelecidas
processos ou prazos já em andamento
conhecimentos recentes necessários à abertura
relações ou mudanças atuais relevantes
último fato estabelecido
primeiro ponto aberto
```

Nem todos os campos precisam conter conteúdo.

```text
ESTADO SUFICIENTE
≠ CENA PRÉ-ESCRITA
```

---

# Estado inicial antes do START

Antes da primeira cena, ainda não existe acontecimento narrado desta obra.

Mesmo assim, a preparação pode estabelecer **condições de abertura**.

Exemplo:

```text
Momento
→ segunda-feira de manhã, última semana do semestre.

Local principal
→ Universidade de Metrópolis.

Presenças
→ Kara está no campus.
→ Daniel está no campus.

Último fato estabelecido
→ história ainda não iniciada.
```

Isso não significa que uma cena já aconteceu.

São fatos da configuração inicial autorizada para que o START tenha uma realidade onde abrir.

```text
CONDIÇÃO INICIAL
≠ ACONTECIMENTO JÁ NARRADO
```

Quando o START ocorrer, essas condições formam o presente inicial da Ficção.

---

# O primeiro ponto aberto

O campo mais importante da preparação é:

```text
## Primeiro ponto aberto
```

Ele identifica **a primeira autoria, ação, decisão ou consequência que ainda não foi estabelecida**.

Exemplos válidos:

```text
Kara e Daniel estão na mesma cafeteria, mas ainda não interagiram.
→ primeiro ponto aberto: se alguma Cadeira toma iniciativa e de que forma.
```

```text
Ana acabou de receber uma ligação cujo conteúdo já foi estabelecido.
→ primeiro ponto aberto: como Ana responde, se essa vontade estiver aberta.
```

```text
A nave entra em órbita e os sensores mostram a estação abandonada.
→ primeiro ponto aberto: decisão da tripulação sobre o que fazer.
```

Não escrever como fato aquilo que ainda é justamente a escolha aberta.

Ruim:

```text
Primeiro ponto aberto:
Kara decide sentar ao lado de Daniel e puxar conversa.
```

se essa decisão ainda pertence à Cadeira de Kara.

Melhor:

```text
Primeiro ponto aberto:
Kara percebe que há lugar livre perto de Daniel; sua reação permanece aberta.
```

ou, se nem essa percepção foi estabelecida:

```text
Primeiro ponto aberto:
a primeira iniciativa voluntária entre as Cadeiras disponíveis no ambiente.
```

---

# Estado inicial não exige incidente incitante

A IA não deve perguntar por obrigação:

```text
qual é o grande conflito inicial?
qual evento dá início à trama?
qual é a primeira ameaça?
qual será a primeira revelação?
```

Uma história pode começar com:

```text
café da manhã
aula
viagem
rotina de trabalho
silêncio
conversa casual
uma personagem chegando a um lugar
```

sem que exista crise imediata.

> **START precisa de um ponto de entrada, não de um espetáculo obrigatório.**

Não fabricar conflito apenas porque a Ficção está começando.

---

# A IA pode propor uma âncora simples

Se Premissa e preparação já indicam claramente uma abertura natural, a IA pode propor um Estado inicial sem novo interrogatório.

Exemplo:

```text
Premissa
→ comédia romântica universitária entre duas personagens que ainda não se conhecem.

Preparação
→ ambas estudam na mesma universidade.
```

A IA pode propor:

```text
Momento
→ um dia comum no fim do semestre.

Local principal
→ campus.

Presenças
→ ambas estão no campus em suas rotinas normais.

Último fato estabelecido
→ história ainda não iniciada.

Primeiro ponto aberto
→ qual iniciativa ou circunstância cotidiana coloca a primeira personagem em movimento.
```

Se o Diretor já definiu algo mais concreto, usar isso.

Se a escolha do ponto de abertura muda materialmente a experiência desejada, propor poucas opções ou perguntar somente por essa escolha.

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

---

# Não decidir pelo Diretor o que é estrutural

A IA pode preencher textura neutra compatível, mas não deve fechar silenciosamente um início estrutural que ainda pertence ao Diretor.

Exemplos de escolhas que podem exigir aprovação quando realmente abertas:

```text
qual personagem recebe o primeiro foco
se as personagens já se conhecem na abertura
se começam juntas ou separadas
se a obra começa antes ou depois de um acontecimento importante
qual segredo já foi descoberto antes do START
qual relação já existe no primeiro instante
```

Exemplos normalmente menores:

```text
hora aproximada dentro de um período já definido
clima ordinário sem função estrutural
posição física neutra coerente dentro do local
objetos cotidianos sem relevância especial
```

Detalhe neutro não deve virar decisão de trama.

---

# Estado não é Direção

Não colocar em `estado.md`:

```text
"Kara e Daniel vão se apaixonar."
"A revelação deve ocorrer neste arco."
"Daniel perderá a próxima luta."
"a história deve continuar leve."
```

Esses conteúdos pertencem à Direção, quando realmente fechados.

```text
DIREÇÃO
→ o que ainda deve governar o futuro.

ESTADO
→ o que já é verdade no presente.
```

---

# Estado não é Operação

Também não colocar em `estado.md`:

```text
"estamos discutindo se Kara vai falar com Daniel."
"a Cadeira de Kara acha melhor esperar."
"o Narrador considera a opção B mais coerente."
```

Isso pertence à Mesa ou a `operacao.md` quando precisa persistir.

```text
OPERAÇÃO
→ pergunta pendente.

ESTADO
→ realidade presente.
```

---

# Estado não é Ficha

Não duplicar identidade permanente.

```text
Kara é kryptoniana
→ ficha.

Kara está usando óculos e identidade civil nesta cena
→ Estado, quando relevante.
```

```text
Daniel conhece magia desde criança
→ ficha.

Daniel está sem acesso ao grimório nesta noite
→ Estado.
```

A ficha preserva a pessoa; o Estado preserva sua condição atual.

---

# Estado não é Livro

O Estado não precisa recontar tudo que aconteceu antes.

Depois que a história começar:

```text
LIVRO / REGISTRO
→ passado ficcional desenvolvido.

ESTADO
→ somente o recorte do presente necessário para continuar.
```

No Estado inicial:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

Depois da primeira execução real, esse campo passa a registrar o último fato efetivamente estabelecido.

---

# Intenções persistentes na abertura

Uma intenção só entra no Estado inicial se já tiver sido legitimamente estabelecida antes do START como condição da personagem.

Exemplo:

```text
Premissa / ficha / preparação aprovada
→ Ana já está procurando o irmão desaparecido quando a história começa.
```

Pode entrar:

```text
Intenção persistente
→ Ana procura o irmão desaparecido.
```

Mas não inventar uma intenção apenas para movimentar a abertura.

```text
PRECISAMOS DE ALGO PARA A PERSONAGEM FAZER
≠ AUTORIZAÇÃO PARA INVENTAR OBJETIVO
```

---

# Processos e prazos

Registrar somente processos já existentes na abertura.

Exemplos:

```text
última semana do semestre
prazo de entrega amanhã
viagem já em andamento
investigação já iniciada antes da primeira cena
tratamento em curso
festival que começa ao anoitecer
```

Não criar cronômetros artificiais para produzir urgência.

---

# Estado mínimo válido

Uma abertura simples pode usar:

```text
# Estado

Momento: manhã de segunda-feira, fim do semestre.
Local principal: Universidade de Metrópolis.

## Presenças e posições

- Kara — no campus, em rotina universitária.
- Daniel — no campus, em rotina universitária.

## Condições relevantes

Nenhuma especial.

## Último fato estabelecido

História ainda não iniciada.

## Primeiro ponto aberto

A primeira iniciativa ou circunstância cotidiana que coloca uma das Cadeiras centrais em movimento permanece aberta.
```

Não é necessário escrever uma mini-sinopse da cena seguinte.

---

# Reconhecer a próxima autoria ou função

O Estado inicial deve permitir ao START identificar o que acontece a seguir sem tomar autoria alheia.

```text
primeiro ponto aberto pertence a Cadeira IA disponível
→ IA troca de escopo
→ Cadeira decide
→ continuar.

primeiro ponto aberto pertence ao Personagem do Diretor
→ apresentar a situação
→ aguardar o Diretor,
  salvo Direção ou delegação suficiente.

próximo passo é consequência ordinária e evidente dos fatos já estabelecidos
→ não existe nova decisão autoral
→ Narrador apresenta
→ continuar.

resultado material importante ainda admite mais de uma versão legítima e não está fechado
→ não é autoria escondida do Narrador
→ Mesa, quando necessária.
```

Seguir:

```text
03-CADEIRAS-E-EXECUTORES.md
05-NARRADOR.md
02-RESOLUCAO.md
```

> **O Estado aponta onde a autoria ou a continuidade recomeça; não rouba autoria nem cria uma sentença escondida.**

---

# Estado desta etapa

Usar conceitualmente:

```text
ESTADO INICIAL: EM CONSTRUÇÃO
ESTADO INICIAL: PROPOSTO
ESTADO INICIAL: SUFICIENTE PARA START
```

`SUFICIENTE PARA START` significa:

```text
há uma realidade inicial reconhecível
+
os fatos estruturais necessários estão presentes
+
o primeiro ponto aberto está identificável
+
a IA sabe qual autoria ou função vem a seguir.
```

Não significa que a primeira cena já foi escrita.

---

# Persistência

Quando suficiente, criar ou atualizar:

```text
campanhas/<slug>/estado.md
```

usando `modelos/ESTADO.md`.

Registrar somente condições aprovadas ou legitimamente derivadas da preparação.

Se ainda existe uma decisão autoral pendente sobre a própria abertura e ela precisa sobreviver a pausa:

```text
operacao.md
→ preserva a questão pendente.
```

Não usar `estado.md` para transformar uma opção de abertura em fato.

---

# Transição para a Auditoria

Quando o Estado inicial estiver suficiente:

```text
ESTADO INICIAL
→ SUFICIENTE PARA START
↓
AUDITORIA DE PREPARAÇÃO
```

A Auditoria verifica se o workspace permite executar sem inventar autoridade, conhecimento ou fatos estruturais ausentes.

Ela não precisa exigir detalhes que a Ficção pode descobrir organicamente.

---

# Critério de conclusão

Antes de encerrar esta etapa, verificar:

```text
[ ] sabemos em que momento a abertura ocorre?
[ ] sabemos onde a Ficção pode começar?
[ ] as presenças necessárias estão claras quando importam?
[ ] condições temporárias relevantes foram preservadas?
[ ] nenhuma vontade nova foi inventada apenas para gerar movimento?
[ ] nenhum futuro desejado foi colocado como realidade presente?
[ ] nenhuma hipótese de Mesa foi canonizada?
[ ] o último fato indica corretamente que a história ainda não começou, quando for o primeiro START?
[ ] o primeiro ponto aberto está identificável?
[ ] é possível reconhecer quem possui a próxima autoria ou se o próximo passo é apenas continuidade evidente?
[ ] a IA evitou pré-escrever a primeira cena?
```

Se sim:

```text
ESTADO INICIAL
→ SUFICIENTE PARA START
→ persistir em estado.md
→ seguir para AUDITORIA DE PREPARAÇÃO.
```

---

# Regra final

> **Estado inicial é a fotografia imediatamente anterior à primeira execução ficcional. Ele define somente as condições necessárias da abertura e identifica onde começa o espaço ainda não decidido. Não exige incidente incitante, não pré-escreve a cena e não transforma vontade aberta em fato. Quando o START acontecer, as Cadeiras decidem o espaço voluntário disponível e o Narrador apresenta a continuidade autorizada ou evidente.**