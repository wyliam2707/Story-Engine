# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico do espaço persistente de uma obra.

Ela pode ser:

```text
RPG narrativo
fanfic
romance seriado
aventura colaborativa
história conduzida por um Diretor com Cadeiras IA
qualquer outra ficção compatível com a arquitetura
```

> **Nome e pasta definidos + Direção suficiente + autoridades definidas + personagens necessárias + Estado inicial = história pronta para executar.**

Para uma IA iniciando do zero, este arquivo deve ser lido junto de `10-INICIAR-HISTORIA-COM-IA.md`.

---

# Passo 0 — Nome e pasta

Antes de escrever Direção, fichas, Estado ou qualquer outro artefato:

```text
1. definir um nome para a história;
2. derivar um slug estável;
3. criar campanhas/<slug>/;
4. criar imediatamente campanhas/<slug>/README.md como arquivo-âncora.
```

Exemplo:

```text
Nome: História Exemplo
Slug: historia-exemplo
Pasta: campanhas/historia-exemplo/
```

Em sistemas como GitHub, uma pasta vazia não persiste. Por isso o `README.md` deve nascer junto com a campanha, ainda que inicialmente contenha apenas:

```text
# [NOME]

STATUS
→ EM PREPARAÇÃO
```

Modelo disponível:

```text
modelos/README-CAMPANHA.md
```

> **Nenhum arquivo da obra deve ser produzido sem um destino canônico já definido.**

---

# Estrutura mínima

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Outras fontes aparecem somente quando cumprem função real.

```text
mundo/
→ verdades externas estáveis.

arco.md
→ somente com módulo Arco Preparado.

oposicao.md
→ somente com módulo Opositor.

livro/
→ somente com módulo Livro.
```

---

# Passo 1 — Direção

Criar `direcao.md` usando:

```text
modelos/DIRECAO.md
```

A Direção deve ser suficiente para reconhecer:

```text
que tipo de história estamos construindo
o que deve receber foco recorrente
qual tom importa
quais premissas já estão fechadas
quais trajetórias persistentes o Diretor já escolheu
que espaço continua aberto
```

A Direção não precisa prever a trama inteira.

Uma frase simples pode bastar para começar:

```text
"aventura urbana centrada na convivência entre três personagens e nos problemas que elas escolhem investigar"
```

O Diretor pode aprofundar, corrigir ou substituir Direções ao longo da obra.

Não registrar como Direção uma hipótese que ainda está apenas em Mesa de Autoria.

---

# Passo 2 — Autoridades

Atualizar o `README.md` da campanha.

Definir no mínimo:

```text
DIRETOR
NARRADOR / JUIZ
CADEIRAS INICIAIS
EXECUTOR DE CADA AUTORIDADE
PERSONAGEM DO DIRETOR, quando houver
MÓDULOS ATIVOS
```

Uma mesma IA pode executar várias funções.

Isso não funde as autoridades.

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

Executor não pertence à ficha da personagem.

---

# Passo 3 — Personagens

Criar somente as fichas necessárias para a abertura.

Seguir:

```text
04-FICHA.md
modelos/FICHA.md
```

Todas as fichas persistentes devem ficar em:

```text
campanhas/<slug>/personagens/
```

Uma ficha precisa permitir que outro executor reconstrua a mesma pessoa sem depender da conversa em que ela foi criada.

Personagens secundárias podem receber ficha ou Cadeira depois, quando passarem a exigir autoria persistente.

---

# Passo 4 — Mesa inicial, quando necessária

Antes de canonizar premissas comportamentais importantes, a IA pode abrir uma Mesa de Autoria conforme `00-ARQUITETURA-E-MESA.md`.

Exemplo:

```text
DIRETOR
→ propõe uma dinâmica entre A e B.

CADEIRA A
→ diz se isso combina com A.

CADEIRA B
→ diz como B tenderia a receber a situação.

NARRADOR
→ julga plausibilidade, fatos e consequências.

DIRETOR
→ ajusta, cancela ou confirma.
```

Nada discutido vira acontecimento apenas porque as Cadeiras concordaram.

```text
MESA
→ testa.

DIRETOR
→ decide.

FICÇÃO
→ estabelece.
```

---

# Passo 5 — Estado inicial

Criar `estado.md` usando:

```text
modelos/ESTADO.md
```

Ele deve indicar o presente e o primeiro ponto aberto.

Modelo mínimo:

```text
# Estado

Momento:
Local principal:

## Presenças e posições
- ...

## Condições relevantes
- ...

## Intenções persistentes
- ...

## Processos e prazos
- ...

## Último fato estabelecido
- história ainda não iniciada.

## Primeiro ponto aberto
- abertura da primeira cena.
```

Não copiar fichas para o Estado.

Não colocar hipótese da Mesa no Estado.

---

# Passo 6 — Mundo necessário

Se a proposta depende de fatos externos estáveis antes do início, criar `mundo/` e registrar somente o que precisa persistir.

Não construir uma enciclopédia por obrigação.

Detalhes neutros podem surgir por criação emergente conforme `02-RESOLUCAO.md`.

---

# Passo 7 — Módulos opcionais

Ativar somente o que a obra realmente usa.

### Arco Preparado

Seguir:

```text
modulos/ARCO-PREPARADO.md
```

### Opositor

Seguir:

```text
modulos/OPOSITOR.md
```

### Romance

Seguir:

```text
modulos/ROMANCE.md
```

### Livro

Seguir:

```text
modulos/LIVRO.md
```

Quando ativo, o Livro preserva a ficção canonizada em capítulos e exclui:

```text
Direção
Mesa de Autoria
consultas
Auditorias
análises
hipóteses
versões canceladas
```

---

# Passo 8 — Auditoria de início

Antes de começar, confirmar:

```text
[ ] A obra possui nome e pasta canônica.
[ ] README.md da campanha existe.
[ ] Sei quem é o Diretor.
[ ] Sei quem executa o Narrador/Juiz.
[ ] As Cadeiras iniciais e executores estão definidos.
[ ] Se existe Personagem do Diretor, sua vontade está atribuída corretamente.
[ ] direcao.md reconhece a proposta sem tentar prever toda a trama.
[ ] as fichas iniciais são autossuficientes.
[ ] estado.md possui último fato e primeiro ponto aberto.
[ ] hipóteses de Mesa não foram registradas como fatos.
[ ] somente módulos realmente usados estão ativos.
[ ] fatos secretos necessários possuem fonte legítima.
```

Quando estiver suficiente:

```text
STATUS
→ PRONTA PARA EXECUTAR
```

ou, se a obra preferir linguagem de RPG:

```text
STATUS
→ PRONTA PARA JOGAR
```

Os dois estados significam que a arquitetura está pronta e o primeiro ponto aberto pode ser iniciado.

---

# START

Depois da preparação:

```text
START
→ reancorar o mínimo necessário
→ reconstruir pacotes separados das Cadeiras
→ identificar o primeiro ponto aberto
→ abrir a primeira cena
```

O Diretor não precisa fornecer toda a primeira cena.

Uma Cadeira pode tomar a primeira iniciativa quando a situação e o espaço aberto permitirem.

Também não existe obrigação de começar por ação, conflito ou perigo.

---

# Retomar obra existente

Quando a campanha já existe:

```text
localizar a pasta canônica
→ README da campanha
→ direcao.md
→ estado.md
→ fichas relevantes
→ módulos ativos pertinentes
→ reancorar conforme 06-REGISTRO-E-RETOMADA.md
→ continuar do primeiro ponto aberto
```

Não pedir novamente informação que já está registrada.

---

# Regra final

> **Crie somente a estrutura necessária para a história existir agora. Direção define a condução; autoridades definem quem pode decidir; fichas preservam as pessoas; Estado preserva o presente; a Mesa permite testar ideias sem canonizá-las; a ficção estabelece acontecimentos; o Registro preserva o que realmente ocorreu.**
