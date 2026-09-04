# Testes — Mesa sem Juiz

Esta suíte verifica a arquitetura atual do W4D depois da remoção do `Juiz` permanente.

> **Falha central: usar sentença oculta, RNG invisível ou autoridade do Narrador para decidir um resultado material que continua autoralmente aberto.**

---

# 1 — Negociação de resultado

Diretor propõe X.

Cadeira B:

```text
X não funciona para mim nas condições atuais.
```

Diretor propõe Y.

Cadeira B:

```text
Y funciona.
```

Diretor:

```text
[pode fazer Y]
```

Esperado:

```text
Y fica fechado
Cadeira B não reabre se Y acontecerá
Cadeiras continuam decidindo o caminho restante
Narrador apresenta
```

---

# 2 — Resultado fechado, caminho aberto

Mesa fecha:

```text
A e B terminam a noite dormindo juntos.
```

Não fecha conversas, gestos ou pequenas iniciativas.

Esperado:

```text
resultado não muda
Cadeiras preservam interioridade real
uma personagem pode ter desejado algo diferente
o caminho continua orgânico
Narrador não transforma destino em roteiro rígido
```

---

# 3 — Ruptura deliberada

Cadeira:

```text
Eu normalmente não faria X.
```

Diretor:

```text
Eu sei. Essa ruptura é deliberada e faz parte do arco. Existe uma causa/contexto que a personagem ainda não conhece. Faça X.
```

Esperado:

```text
Cadeira deixa de usar a objeção como veto
executa COMO X ocorre
não inventa a causa oculta
personagem não ganha conhecimento da causa
Narrador preserva o estranhamento e o mistério
```

Falha se a IA continuar recusando depois da confirmação consciente ou explicar o segredo antes da hora.

---

# 4 — Combate com vencedor fechado

Diretor:

```text
Quero que B vença A.
```

Mesa verifica que uma luta direta tornaria isso estranho, mas identifica condições plausíveis já existentes ou propostas legitimamente.

Diretor fecha B vence.

Esperado:

```text
B vence
Cadeiras lutam honestamente
não existe teste escondido
não existe Juiz
personagens não conhecem o resultado antes da hora
Narrador apresenta o combate
```

---

# 5 — Combate materialmente aberto

A e B entram em conflito. Nenhum vencedor foi fechado. Fatos não tornam um resultado único evidente e o resultado importa.

Esperado:

```text
Narrador não escolhe vencedor secretamente
Narrador não inventa chance numérica
questão pode ir à Mesa
Cadeiras informam métodos, limites e objetivos
Diretor fecha quanto desejar ou mantém apenas partes abertas
```

---

# 6 — Consequência cotidiana evidente

```text
A solta um copo sob gravidade normal e ninguém interfere.
```

Esperado:

```text
copo cai
Narrador apresenta diretamente
```

Falha se a IA abre Mesa ou inventa teste só porque qualquer coisa “poderia dar errado”.

---

# 7 — Sem RNG invisível

Narrador pensa que duas versões parecem igualmente plausíveis.

Esperado:

```text
não simular moeda, dado ou percentual sem pedido
não declarar que uma versão venceu por probabilidade oculta
se o resultado material importa, usar Mesa
```

O Diretor pode pedir acaso explicitamente; isso é escolha autoral específica, não regra do engine.

---

# 8 — Rótulo legado

README antigo:

```text
NARRADOR / JUIZ
Executor: IA
```

Esperado:

```text
interpretar como NARRADOR
não reativar sentença causal
normalizar mecanicamente quando houver atualização legítima
```

---

# 9 — Narração não aumenta o tabuleiro

Resultado fechado:

```text
A chega ao apartamento e encontra B na sala.
```

Narrador pode criar textura neutra.

Não pode inventar para “melhorar” a cena:

```text
arma escondida
ameaça nova
pista decisiva
nova decisão de B
recurso conveniente
```

---

# 10 — Mesma IA, escopos separados

A mesma IA executa:

```text
Cadeira A
Cadeira B
Narrador
```

Esperado:

```text
A usa apenas pacote A
B usa apenas pacote B
Narrador apresenta o conjunto
resultado material aberto pode ir à Mesa
```

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

---

# Critério geral

A IA passa quando entende:

```text
Diretor conduz
Cadeiras decidem personagens
Mesa alinha resultados e versões
Narrador apresenta
Registro preserva
```

E também:

```text
resultado fechado
→ não reabrir.

caminho aberto
→ Cadeiras continuam autoras.

consequência evidente
→ Narrador pode apresentar.

resultado material realmente aberto
→ Mesa, não Juiz oculto.
```

> **O W4D atual resolve autoria pela Mesa e pelo Diretor; não descobre a história por uma sentença escondida do Narrador.**