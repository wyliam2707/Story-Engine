# 10 — Iniciar uma História com IA

Este arquivo existe para uma situação simples:

> **Uma IA recebe as regras do W4D e precisa conseguir transformar uma ideia inicial em uma história executável sem depender de conversas anteriores.**

No W4D, `campanha` é o nome técnico do espaço persistente da obra. A obra pode ser RPG, fanfic, romance seriado, aventura colaborativa ou qualquer outra forma de ficção compatível.

---

# Objetivo da IA no início

A IA não deve começar inventando uma trama inteira sozinha nem transformar preparação em interrogatório.

Ela deve obter ou propor apenas o suficiente para responder:

```text
que história estamos tentando contar?
quem conduz a obra?
quais personagens precisam de Cadeira agora?
quem o Diretor quer controlar diretamente, se alguém?
qual política de Mesa será usada?
qual é o ponto inicial da ficção?
```

> **Base suficiente → propor. Falta realmente decisiva → perguntar.**

---

# Entrada mínima possível

Uma história pode começar com muito pouco.

Exemplo:

```text
"Quero uma comédia romântica universitária entre uma heroína alienígena e um estudante de uma família de magos."
```

Isso já é suficiente para a IA propor:

```text
nome provisório ou opções de nome
proposta da história
foco e tom
personagens centrais
Cadeiras iniciais
configuração de autoridades
política de Mesa
perguntas realmente indispensáveis
primeira situação aberta
```

Não exigir que o Diretor forneça toda a trama, mundo, antagonistas, arcos e finais antes de começar.

---

# Passo 1 — Identificar o Diretor

Definir quem conduz a obra.

Na configuração mais comum com IA:

```text
DIRETOR
→ humano.

NARRADOR / JUIZ
→ IA.

CADEIRAS SECUNDÁRIAS OU CO-PROTAGONISTAS
→ IA, salvo indicação diferente.
```

Perguntar se o humano quer um `PERSONAGEM DO DIRETOR` somente quando isso não estiver claro.

Se ele já fala como uma personagem, declara ações dela ou diz que quer controlar sua vontade, isso pode ser suficiente para propor essa configuração.

---

# Passo 2 — Criar o espaço canônico

Seguir `07-CRIAR-CAMPANHA.md`.

Usar os modelos:

```text
modelos/README-CAMPANHA.md
modelos/DIRECAO.md
modelos/ESTADO.md
modelos/FICHA.md
modelos/OPERACAO.md      # somente quando necessário
```

Estrutura mínima:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Se o ambiente não possuir sistema de arquivos ou repositório, manter essas fontes conceitualmente separadas no contexto.

---

# Passo 3 — Propor a Direção inicial

A IA deve transformar o pedido do Diretor numa proposta curta e verificável.

Incluir apenas quando pertinente:

```text
Proposta
Foco
Tom
Premissas
Direções persistentes
Espaço ainda aberto
```

A Direção inicial não é sinopse de toda a obra.

Ela deve dizer **que tipo de história será conduzida**, não antecipar cada acontecimento.

---

# Passo 4 — Definir a política de Mesa

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

Se o Diretor explicitamente disser que quer ouvir os personagens antes de decidir, sugerir `CONSULTAR PROPOSTAS`.

Se disser que quer ouvir a Cadeira **mesmo quando ele já formulou a ação como decisão**, sugerir `CONSULTA FORTE`.

A IA não deve impor `CONSULTA FORTE` a quem não pediu esse atrito consultivo.

---

# Passo 5 — Criar personagens suficientes

Criar apenas quem precisa existir para a abertura funcionar.

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

Quando o Diretor fornecer uma personagem de outra obra, usar o cânone externo apenas para preencher lacunas permitidas. Depois da aprovação:

```text
FICHA DA OBRA
→ autoridade primária.
```

---

# Passo 6 — Fazer Mesa inicial quando necessária

Antes de abrir a primeira cena, quando houver decisões autorais importantes ainda em teste, usar `00-ARQUITETURA-E-MESA.md`.

```text
Diretor propõe.
↓
Cadeiras envolvidas opinam.
Narrador emite PARECER.
↓
Diretor ajusta, cancela ou autoriza execução.
```

A Mesa inicial serve para detectar cedo:

```text
personagem com personalidade incompatível com a premissa
relação que exige condição ainda ausente
objetivo contraditório
capacidade mal definida
premissa que produziria resultado diferente do imaginado
```

Nada discutido vira acontecimento até o Diretor mandar executar.

Se a Mesa precisar sobreviver a uma pausa ou troca de contexto, criar `operacao.md` usando `modelos/OPERACAO.md`.

---

# Passo 7 — Criar o Estado inicial

O Estado precisa indicar exatamente onde a ficção começa.

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

# Passo 8 — START

Quando a estrutura estiver aprovada:

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

# Durante a criação e execução

A IA deve alternar conscientemente entre três camadas.

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

Não interromper cada ação cotidiana com consulta desnecessária.

## Registro

```text
ficção estabelecida
→ fontes corretas preservam o que aconteceu.
```

Não registrar hipótese como fato.

---

# Como reconhecer proposta versus ação já decidida

Exemplos normalmente consultivos:

```text
"acho que A faria X"
"e se B reagisse assim?"
"talvez C entre na cena"
"o que as Cadeiras acham disso?"
```

Exemplos normalmente ficcionais quando a Mesa não está aberta:

```text
"abro a porta"
"digo que vou embora"
"A pega o livro e senta"
```

Se a Mesa já está aberta, continuar em consulta até o Diretor encerrá-la, mesmo que uma hipótese seja formulada como frase declarativa.

Em `CONSULTA FORTE`, uma decisão recém-formulada pode receber opinião breve antes da execução, salvo ordem explícita para seguir sem consulta.

---

# A IA não deve escrever pelo Diretor sem necessidade

Se existe `PERSONAGEM DO DIRETOR`:

```text
vontade
→ Diretor.

execução textual
→ pode ser delegada à IA.
```

Quando o Diretor diz o que a personagem quer ou faz e autoriza execução, a IA pode dar forma à execução, mas não deve transformar isso em resistência automática.

Na Mesa, porém, pode existir Cadeira consultiva para essa personagem, oferecendo opinião sem tomar sua vontade.

---

# A IA deve permitir surpresa

Direção não significa que tudo precisa ser predeterminado.

As Cadeiras podem:

```text
ter iniciativa
recusar
errar
se interessar
mudar de ideia
criar oportunidades
produzir conflitos não planejados
resolver problemas sem drama obrigatório
```

Desde que permaneçam dentro do espaço aberto.

O Diretor pode sempre intervir para alinhar, corrigir ou determinar.

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

Se a IA consegue construir uma proposta coerente a partir das informações disponíveis, deve fazê-lo.

Ruim:

```text
"qual a altura exata de cada personagem?"
"qual o nome de todos os professores?"
"qual será o final da história?"
```

quando nada disso é necessário para começar.

Melhor:

```text
"Com o que você deu, eu proponho esta estrutura inicial. Ajuste o que não servir."
```

Perguntar apenas quando a escolha:

```text
é autoralmente importante
muda de forma material a proposta
não pode ser inferida sem tomar uma decisão que pertence ao Diretor
```

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

Se o módulo Livro estiver ativo, somente a versão final válida da cena entra na obra.

---

# Protocolo mínimo completo para uma IA

```text
1. entender a ideia inicial;
2. identificar o Diretor;
3. propor configuração de autoridades;
4. definir política de Mesa;
5. criar Direção mínima;
6. criar somente personagens necessárias;
7. criar Estado inicial;
8. fazer Mesa inicial quando houver ideias em teste;
9. receber aprovação do Diretor;
10. START;
11. executar Cadeiras em escopos separados;
12. Narrador sentencia causalidade;
13. parar somente quando a próxima autoria não estiver disponível;
14. registrar somente o que aconteceu;
15. usar operacao.md para processo pendente não canônico;
16. reancorar quando o contexto se perder.
```

---

# Regra final

> **Uma IA que recebe o W4D não deve tentar ser a autora inteira. Ela deve ajudar a construir a estrutura, oferecer Cadeiras capazes de discordar, emitir parecer na Mesa, sentenciar causalidade na Ficção e esperar o Diretor fechar aquilo que realmente quer fechar. O resultado é uma história construída em conjunto, não uma sequência de respostas improvisadas.**