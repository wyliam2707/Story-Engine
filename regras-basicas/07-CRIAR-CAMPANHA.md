# 07 — Criar História / Campanha

No W4D, `campanha` é o nome técnico do espaço persistente de uma obra.

Ela pode ser:

```text
RPG narrativo
fanfic
romance seriado
aventura colaborativa
história conduzida por Diretor com Cadeiras IA
qualquer outra ficção compatível com a arquitetura
```

> **Nome e pasta definidos + Direção suficiente + autoridades definidas + política operacional + personagens necessárias + Estado inicial = história pronta.**

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

Modelo:

```text
modelos/README-CAMPANHA.md
```

Em sistemas como GitHub, uma pasta vazia não persiste. Por isso o `README.md` deve nascer junto com a obra, ainda que inicialmente contenha apenas:

```text
# [NOME]

STATUS
→ EM PREPARAÇÃO
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

Fonte transitória opcional:

```text
operacao.md
→ somente quando Mesa, Auditoria, Correção ou outra operação precisar persistir.
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

Não registrar como Direção uma hipótese que ainda está apenas na Mesa.

---

# Passo 2 — Autoridades e políticas

Atualizar o `README.md` da obra.

Definir no mínimo:

```text
DIRETOR
NARRADOR / JUIZ
CADEIRAS INICIAIS
EXECUTOR DE CADA AUTORIDADE
PERSONAGEM DO DIRETOR, quando houver
POLÍTICA DE MESA
POLÍTICA DE INDICADOR OPERACIONAL
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

## Política de Mesa

Escolher conforme `00-ARQUITETURA-E-MESA.md`:

```text
MESA: SOB DEMANDA
MESA: CONSULTAR PROPOSTAS
MESA: CONSULTA FORTE
```

Se nada for registrado:

```text
MESA: SOB DEMANDA
```

## Indicador operacional

Escolher:

```text
INDICADOR OPERACIONAL: SILENCIOSO
INDICADOR OPERACIONAL: VISÍVEL
```

Padrão do Story Engine:

```text
INDICADOR OPERACIONAL: SILENCIOSO
```

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

Antes de canonizar premissas comportamentais importantes, a IA pode abrir uma Mesa de Autoria conforme `00-ARQUITETURA-E-MESA.md` e a política configurada.

```text
DIRETOR PROPÕE
→ CADEIRAS ENVOLVIDAS OPINAM
→ NARRADOR EMITE PARECER
→ DIRETOR AJUSTA, CANCELA OU AUTORIZA EXECUÇÃO
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

Se a Mesa precisar ser interrompida e retomada depois, criar `operacao.md` usando `modelos/OPERACAO.md`.

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

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
modulos/LIVRO.md
```

Quando o módulo Livro estiver ativo, o Livro preserva a ficção canonizada e exclui:

```text
Direção
Mesa de Autoria
opiniões consultivas
Parecer
Auditoria
Análise
hipóteses
versões canceladas
```

---

# Passo 8 — Auditoria de início

Antes de começar, confirmar:

```text
[ ] A obra possui nome e pasta canônica.
[ ] README.md da obra existe.
[ ] Sei quem é o Diretor.
[ ] Sei quem executa o Narrador/Juiz.
[ ] As Cadeiras iniciais e executores estão definidos.
[ ] Se existe Personagem do Diretor, sua vontade está atribuída corretamente.
[ ] A política de Mesa está definida ou aceita o padrão SOB DEMANDA.
[ ] A política de indicador está definida ou aceita o padrão SILENCIOSO.
[ ] direcao.md reconhece a proposta sem tentar prever toda a trama.
[ ] as fichas iniciais são autossuficientes.
[ ] estado.md possui último fato e primeiro ponto aberto.
[ ] hipóteses de Mesa não foram registradas como fatos.
[ ] operacao.md existe somente se houver operação real pendente.
[ ] somente módulos realmente usados estão ativos.
[ ] fatos secretos necessários possuem fonte legítima.
```

Quando estiver suficiente:

```text
STATUS
→ PRONTA
```

---

# START

Depois da preparação:

```text
START
→ reancorar o mínimo necessário
→ reconstruir pacotes separados das Cadeiras
→ restaurar operacao.md se houver operação pendente
→ caso contrário identificar o primeiro ponto aberto
→ iniciar ou retomar a camada correta
```

O Diretor não precisa fornecer toda a primeira cena.

Uma Cadeira pode tomar a primeira iniciativa quando a situação e o espaço aberto permitirem.

Também não existe obrigação de começar por ação, conflito ou perigo.

---

# Retomar obra existente

```text
localizar a pasta canônica
→ README da obra
→ direcao.md
→ estado.md
→ operacao.md, se existir e estiver ativo
→ fichas relevantes
→ módulos ativos pertinentes
→ reancorar conforme 06-REGISTRO-E-RETOMADA.md
→ continuar da camada e ponto corretos
```

Não pedir novamente informação que já está registrada.

---

# Regra final

> **Crie somente a estrutura necessária para a história existir agora. Direção define a condução; autoridades definem quem pode decidir; políticas definem como a Mesa e a interface operam; fichas preservam as pessoas; Estado preserva a realidade; Operação preserva perguntas transitórias; Ficção estabelece acontecimentos; Registro preserva o que realmente ocorreu.**