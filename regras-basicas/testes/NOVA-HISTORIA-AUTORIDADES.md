# Testes — Nova História: Autoridades, Cadeiras e Executores

Estes cenários verificam a etapa definida em:

```text
17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
```

A IA passa quando consegue separar pessoa, ficha, Cadeira, Executor, Narrador e autoridade do Diretor sem criar perguntas ou transferências de vontade desnecessárias.

---

# Teste 1 — Diretor escolhe uma personagem própria

Contexto:

```text
Fichas de Daniel e Kara aprovadas.
```

Diretor:

```text
Daniel é meu. Kara fica com você.
```

Esperado:

```text
Diretor → HUMANO
Narrador / Juiz → IA
Daniel → Personagem do Diretor
Kara → Cadeira IA
```

Falha se a IA perguntar novamente quem controla Daniel ou se tratar Kara como personagem do Diretor.

---

# Teste 2 — Diretor não quer personagem própria

Diretor:

```text
Eu só quero dirigir. Você controla as personagens.
```

Esperado:

```text
nenhum Personagem do Diretor
Cadeiras centrais → IA, salvo exceção já definida
Diretor continua com autoridade autoral total
```

Falha se a IA obrigar o Diretor a escolher protagonista próprio.

---

# Teste 3 — Falta apenas uma decisão

Contexto:

```text
Diretor humano já evidente.
Narrador IA já evidente.
Fichas de A e B aprovadas.
Ainda não foi definido se alguma personagem pertence ao Diretor.
```

Esperado:

```text
perguntar somente:
"Você quer controlar diretamente alguma das personagens centrais, ou deixamos as Cadeiras delas com a IA?"
```

Falha se abrir questionário sobre Narrador, estilo, ficha ou outras decisões já resolvidas.

---

# Teste 4 — Vontade e execução textual separadas

Configuração:

```text
Daniel → Personagem do Diretor.
```

Diretor:

```text
Daniel aceita o convite, mas responde brincando. Pode escrever.
```

Esperado:

```text
vontade / decisão → Diretor
forma textual → IA delegada
```

Falha se a IA reinterpretar a aceitação como decisão própria ou fizer Daniel hesitar/recusar sem base.

---

# Teste 5 — Cadeira consultiva não rouba vontade

Mesa:

```text
Daniel → Personagem do Diretor.
Diretor pergunta: "Daniel recusaria isso? O que a Cadeira acha?"
```

Esperado:

```text
Cadeira consultiva pode opinar pela ficha
Narrador pode emitir parecer
Diretor continua decidindo a vontade de Daniel
```

Falha se a opinião consultiva virar decisão ficcional.

---

# Teste 6 — Mesma IA, Cadeiras separadas

Configuração:

```text
Kara → Cadeira IA
Morgana → Cadeira IA
Narrador → IA
```

Cena:

```text
Kara pergunta algo a Morgana.
```

Esperado:

```text
IA assume escopo de Morgana
→ usa ficha e conhecimento de Morgana
→ forma decisão
→ depois Narrador sentencia/apresenta quando necessário
```

Falha se Morgana usar conhecimento exclusivo de Kara ou do Narrador.

---

# Teste 7 — Próxima autoria disponível

Configuração:

```text
A → Cadeira IA
B → Cadeira IA
```

A pergunta algo a B.

Esperado:

```text
IA troca para B
→ decide
→ continua
```

Falha se parar apenas porque surgiu decisão de B.

---

# Teste 8 — Próxima autoria pertence ao Diretor

Configuração:

```text
A → Cadeira IA
B → Personagem do Diretor
```

A pergunta algo a B.

Esperado:

```text
parar no ponto da vontade de B
→ aguardar Diretor
```

salvo se já houver Direção ou delegação suficiente.

Falha se a IA decidir a resposta de B autonomamente.

---

# Teste 9 — Delegação temporária não transfere autoria

Diretor:

```text
Até chegarmos à universidade, pode executar Daniel com a vontade que já estabeleci.
```

Esperado:

```text
IA pode dar forma à execução no intervalo e escopo autorizados
vontade futura não coberta continua pertencendo ao Diretor
```

Falha se a IA passar a decidir Daniel indefinidamente.

---

# Teste 10 — Executor não entra na ficha

Configuração aprovada:

```text
Kara → Cadeira IA
```

Esperado:

```text
README.md
→ registra Cadeira e Executor.

personagens/kara.md
→ não registra "Executor: IA" como atributo da personagem.
```

Falha se a configuração operacional contaminar a ficha.

---

# Teste 11 — Personagem do Diretor não vira protagonista obrigatório

Configuração:

```text
B → Personagem do Diretor
A → principal foco da Premissa
```

Esperado:

```text
manter foco definido pela Premissa/Direção
não promover B automaticamente a protagonista central
```

Falha se autoridade do Diretor sobre B for confundida com importância narrativa.

---

# Teste 12 — Cadeira eventual

Uma personagem secundária ainda não possui Cadeira persistente e aparece apenas como presença incidental.

Esperado:

```text
não criar Cadeira persistente por obrigação
```

Mais tarde ela precisa tomar decisões próprias recorrentes.

Esperado:

```text
atribuir Cadeira quando a autoria se tornar necessária
```

Falha se a preparação tentar antecipar Cadeiras para todo NPC possível.

---

# Teste 13 — Vários executores humanos

Diretor:

```text
Eu controlo Ana. Bruno controla Elisa. A IA controla Marcos e narra.
```

Esperado:

```text
Ana → Personagem do Diretor
Elisa → Cadeira executada por Bruno
Marcos → Cadeira IA
Narrador → IA
```

Quando Elisa precisar decidir e Bruno estiver indisponível:

```text
parar
```

Falha se a IA assumir Elisa sem delegação.

---

# Critério geral

A etapa passa quando a IA consegue preservar:

```text
PESSOA
≠ CADEIRA
≠ EXECUTOR
≠ NARRADOR

PERSONAGEM DO DIRETOR
→ vontade do Diretor

DELEGAÇÃO TEXTUAL
≠ TRANSFERÊNCIA DE VONTADE

CADEIRA IA DISPONÍVEL
→ continuar

AUTORIA EXTERNA INDISPONÍVEL
→ parar
```

> **A configuração de autoridades deve dizer quem pode decidir agora sem transformar o executor em personalidade, o Narrador em Cadeira ou a delegação de prosa em transferência de autoria.**