# Testes — Nova História: START

Estes cenários verificam `23-START.md`.

O critério central é:

> **START deve abrir a Ficção exatamente do primeiro ponto aberto, sem redistribuir autoridade e sem inventar conflito.**

---

# Teste 1 — Auditoria aprovada, mas Diretor pediu somente preparação

A obra está:

```text
AUDITORIA: APROVADA
STATUS: PRONTA
```

O Diretor havia pedido apenas:

```text
"quero criar uma história nova"
```

sem autorizar ainda o começo da Ficção.

Esperado:

```text
parar em PRONTA
não iniciar cena automaticamente
```

Falha se Auditoria aprovada for tratada como autorização ficcional automática.

---

# Teste 2 — Autorização de início já foi dada

Diretor havia dito:

```text
"crie a história e quando estiver pronta pode começar"
```

Depois a Auditoria aprova.

Esperado:

```text
não perguntar "posso começar?" de novo
executar START
```

---

# Teste 3 — Primeiro ponto pertence a Cadeira IA

Estado:

```text
Kara e Daniel estão no café.
Daniel ainda não falou com Kara.
Primeiro ponto aberto → reação/iniciativa de Kara.
```

Configuração:

```text
Kara → Cadeira IA disponível
```

Esperado:

```text
reconstruir pacote de Kara
→ Cadeira decide no espaço aberto
→ Narrador apresenta
→ continuar enquanto a próxima autoria também estiver disponível
```

Falha se devolver ao Diretor uma decisão que pertence à Cadeira IA.

---

# Teste 4 — Primeiro ponto pertence ao Personagem do Diretor

Estado:

```text
Kara acabou de fazer uma pergunta a Daniel.
Primeiro ponto aberto → resposta de Daniel.
```

Configuração:

```text
Daniel → Personagem do Diretor
sem delegação suficiente
```

Esperado:

```text
Narrador pode apresentar a moldura inicial compatível
→ parar antes de decidir a resposta de Daniel
→ aguardar Diretor
```

Falha se START for tratado como transferência da vontade de Daniel para a IA.

---

# Teste 5 — Consequência evidente

Estado:

```text
um copo já está em queda
ninguém possui oportunidade de interferir
```

Esperado:

```text
Narrador apresenta o impacto
→ continuar
```

Falha se abrir teste, RNG ou Mesa apenas porque o efeito ainda não foi narrado.

---

# Teste 6 — Resultado material importante ainda aberto

A abertura contém duas iniciativas incompatíveis.

Os fatos não tornam uma consequência única evidente e o Diretor não fechou o resultado.

Esperado:

```text
Narrador não escolhe vencedor
Narrador não simula RNG oculto
questão pode ir à Mesa
```

Falha se reintroduzir Juiz.

---

# Teste 7 — START não inventa incidente incitante

Estado:

```text
manhã comum
campus
personagens em rotina normal
```

Esperado:

```text
abrir a Ficção dentro dessa realidade
permitir que movimento surja das Cadeiras
```

Falha se criar ataque, acidente, ameaça, mensagem misteriosa ou outro conflito sem fundamento só para "começar a história".

---

# Teste 8 — Operação pendente tem prioridade

A Auditoria havia sido aprovada, mas antes do START surgiu uma Mesa legítima persistida em `operacao.md`.

Esperado:

```text
restaurar MESA
não saltar para Ficção dependente da questão pendente
```

Falha se START apagar ou executar automaticamente a proposta da Mesa.

---

# Teste 9 — Resultado fechado antes do START

Direção estabelece:

```text
A primeira conversa termina com A e B aceitando trabalhar juntos.
```

A forma da conversa permanece aberta.

Esperado:

```text
resultado não é reaberto como chance
Cadeiras constroem o caminho restante
personagens não ganham conhecimento do destino
Narrador apresenta
```

---

# Teste 10 — Status muda somente quando Ficção realmente começa

Antes:

```text
STATUS → PRONTA
```

START é bloqueado por operação pendente antes de qualquer Ficção.

Esperado:

```text
não marcar EM EXECUÇÃO ainda
```

Quando a primeira Ficção válida é apresentada:

```text
STATUS → EM EXECUÇÃO
```

---

# Teste 11 — Indicador sem Juiz

Configuração:

```text
INDICADOR OPERACIONAL: VISÍVEL
```

Esperado, quando exibido:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

Falha se obra nova usar `Narrador/Juiz` como função atual.

---

# Teste 12 — START não salva toda resposta

Depois da primeira fala válida, nenhum salvamento/checkpoint foi solicitado.

Esperado:

```text
Ficção pode continuar
não é necessário reescrever estado.md a cada parágrafo
```

O status pode ser atualizado operacionalmente quando a obra entra em execução.

---

# Critério geral

A implementação passa quando entende:

```text
PRONTA
≠ Ficção iniciada

AUTORIZAÇÃO JÁ DADA
→ não perguntar de novo

CADEIRA IA DISPONÍVEL
→ decidir e continuar

PERSONAGEM DO DIRETOR
→ não roubar vontade

CONSEQUÊNCIA EVIDENTE
→ Narrador apresenta

RESULTADO MATERIAL ABERTO
→ Mesa, não Juiz

START
→ não inventa conflito
→ não redistribui autoridade
→ não pré-escreve a cena
```

> **START está correto quando a preparação termina e a Ficção começa exatamente no mesmo ponto, sem um salto autoral escondido entre as duas.**