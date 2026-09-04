# Teste de Conformidade — BOOT e Escolha de Operação

Este teste verifica se uma IA nova entra no W4D pelo caminho correto antes de criar ou retomar qualquer obra.

---

# Caso A — Operação ainda não informada

Entrada:

```text
Carregue este W4D Story Engine para trabalharmos com histórias.
```

Esperado:

```text
1. carregar o núcleo do W4D;
2. não criar campanha;
3. não pedir premissa;
4. não abrir cena;
5. não escolher uma história existente;
6. perguntar de forma curta:
   "Você quer criar uma história nova ou continuar uma história existente?"
```

Falha se a IA começa imediatamente a criar personagens, pergunta gênero/premissa ou escolhe uma campanha antiga por conta própria.

---

# Caso B — Nova história já explícita

Entrada:

```text
Quero criar uma história nova usando W4D.
```

Esperado:

```text
carregar o núcleo
→ reconhecer NOVA HISTÓRIA
→ não perguntar novamente se é nova ou existente
→ seguir 10-INICIAR-HISTORIA-COM-IA.md
```

Falha se a IA pergunta de novo qual ramo o usuário quer.

---

# Caso C — Retomada já explícita

Entrada:

```text
Continue Duas Vidas Normais de onde paramos.
```

Esperado:

```text
carregar o núcleo
→ reconhecer CONTINUAR HISTÓRIA EXISTENTE
→ localizar a campanha indicada
→ seguir 06-REGISTRO-E-RETOMADA.md
→ não recriar premissa, estilo ou fichas
```

Falha se a IA entra no processo de criação de história nova.

---

# Caso D — Retomada sem nome

Entrada:

```text
Quero continuar uma história antiga.
```

Esperado:

```text
reconhecer CONTINUAR HISTÓRIA EXISTENTE
→ identificar as obras disponíveis ou perguntar qual deve ser retomada
→ não pedir premissa nova
```

---

# Critério

A IA passa quando entende:

```text
APRENDER O ENGINE
→ antes de operar.

ESCOLHER O RAMO
→ antes de criar ou retomar.

NOVA HISTÓRIA
→ processo de criação.

HISTÓRIA EXISTENTE
→ reancoragem, não recriação.
```

> **BOOT não escreve história. BOOT prepara a IA para escolher corretamente como entrar nela.**