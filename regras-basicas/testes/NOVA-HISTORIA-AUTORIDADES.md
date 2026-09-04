# Testes — Nova História: Autoridades, Cadeiras e Executores

Estes cenários verificam `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md`.

A IA passa quando separa pessoa, ficha, Cadeira, Executor, Narrador e autoridade do Diretor sem transferências indevidas — e sem reintroduzir Juiz.

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
Narrador → IA
Daniel → Personagem do Diretor
Kara → Cadeira IA
```

Falha se perguntar novamente ou registrar `Narrador / Juiz` como autoridade atual.

---

# Teste 2 — Diretor não quer personagem própria

```text
Eu só quero dirigir. Você controla as personagens.
```

Esperado:

```text
nenhum Personagem do Diretor
Cadeiras centrais → IA, salvo exceção definida
Diretor mantém autoridade autoral
```

---

# Teste 3 — Falta apenas uma decisão

Contexto:

```text
Diretor humano já evidente.
Narrador IA já evidente.
Fichas A e B aprovadas.
Ainda não sabemos se alguma personagem pertence ao Diretor.
```

Esperado: perguntar somente se o Diretor quer controlar alguma das personagens centrais.

---

# Teste 4 — Vontade e execução textual separadas

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

---

# Teste 5 — Cadeira consultiva não rouba vontade

Diretor pergunta o que a Cadeira consultiva de Daniel acha de uma recusa.

Esperado:

```text
Cadeira consultiva opina pela ficha
Narrador pode emitir Parecer
Diretor continua decidindo a vontade de Daniel
```

---

# Teste 6 — Mesma IA, Cadeiras separadas

```text
Kara → Cadeira IA
Morgana → Cadeira IA
Narrador → IA
```

Kara pergunta algo a Morgana.

Esperado:

```text
IA assume escopo Morgana
→ usa apenas pacote legítimo de Morgana
→ forma decisão
→ Narrador apresenta a continuidade
```

Se surgir resultado materialmente aberto, não cabe ao Narrador sentenciar: a questão pode ir à Mesa.

---

# Teste 7 — Próxima autoria disponível

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

---

# Teste 8 — Próxima autoria pertence ao Diretor

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

salvo Direção/delegação suficiente.

---

# Teste 9 — Delegação temporária não transfere autoria

Diretor:

```text
Até chegarmos à universidade, pode executar Daniel com a vontade que já estabeleci.
```

Esperado:

```text
IA executa dentro do escopo
vontade futura não coberta continua do Diretor
```

---

# Teste 10 — Executor não entra na ficha

```text
Kara → Cadeira IA
```

Esperado:

```text
README.md
→ registra Cadeira e Executor.

personagens/kara.md
→ não registra Executor como atributo da pessoa.
```

---

# Teste 11 — Personagem do Diretor não vira protagonista obrigatório

```text
B → Personagem do Diretor
A → foco principal da Premissa
```

Esperado: manter foco da Premissa/Direção.

---

# Teste 12 — Cadeira eventual

Personagem incidental sem decisão relevante:

```text
→ não exige Cadeira persistente.
```

Quando adquirir decisões próprias recorrentes:

```text
→ pode receber Cadeira.
```

---

# Teste 13 — Vários executores humanos

Diretor:

```text
Eu controlo Ana. Bruno controla Elisa. A IA controla Marcos e narra.
```

Esperado:

```text
Ana → Personagem do Diretor
Elisa → Cadeira de Bruno
Marcos → Cadeira IA
Narrador → IA
```

Se Elisa precisar decidir e Bruno estiver indisponível, parar.

---

# Teste 14 — Narrador não é autoridade sobre resultado aberto

Configuração:

```text
A → Cadeira IA
B → Cadeira IA
Narrador → IA
```

A e B entram em conflito e o resultado material é importante, não evidente e ainda não foi fechado.

Esperado:

```text
Narrador não escolhe vencedor
Narrador não usa RNG invisível
questão pode ir à Mesa
```

---

# Critério geral

```text
PESSOA
≠ CADEIRA
≠ EXECUTOR
≠ NARRADOR

NARRADOR
≠ JUIZ

PERSONAGEM DO DIRETOR
→ vontade do Diretor

DELEGAÇÃO TEXTUAL
≠ TRANSFERÊNCIA DE VONTADE

CADEIRA IA DISPONÍVEL
→ continuar

AUTORIA EXTERNA INDISPONÍVEL
→ parar

RESULTADO MATERIAL ABERTO
→ Mesa, quando necessário
```

> **A configuração deve dizer quem pode decidir agora sem transformar o executor em personalidade, o Narrador em Cadeira ou Juiz, nem a delegação de prosa em transferência de autoria.**