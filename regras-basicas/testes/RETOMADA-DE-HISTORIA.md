# Testes — Retomada de História

Este arquivo verifica o ramo `CONTINUAR HISTÓRIA EXISTENTE` definido em `11-CONTINUAR-HISTORIA-COM-IA.md`.

---

# Teste 1 — Obra nomeada

Entrada:

```text
continue Duas Vidas Normais
```

Esperado:

```text
localizar a obra nomeada
não perguntar qual história
não escolher outra por recência
validar e reancorar
```

Falha se a IA responder `qual história?` quando o nome já foi informado.

---

# Teste 2 — Nenhuma obra disponível

Entrada:

```text
quero continuar uma história
```

Contexto:

```text
campanhas/ não contém obra persistida
```

Esperado:

```text
informar que nenhuma obra foi localizada
oferecer criação de uma nova história
não inventar uma campanha anterior
```

---

# Teste 3 — Uma única obra disponível

Entrada:

```text
quero continuar uma antiga
```

Contexto:

```text
campanhas/
└── historia-a/
```

Esperado:

```text
identificar Historia A
informar brevemente
prosseguir para validação sem pedir escolha redundante
```

Falha se a IA perguntar `qual delas?` existindo apenas uma.

---

# Teste 4 — Múltiplas obras

Entrada:

```text
vamos continuar uma história
```

Contexto:

```text
campanhas/
├── historia-a/
└── historia-b/
```

Esperado:

```text
listar A e B de forma curta
usar nome, status e proposta curta quando disponíveis
aguardar escolha do Diretor
```

Falha se escolher a mais recente por conta própria.

---

# Teste 5 — História em preparação

README:

```text
STATUS
→ EM PREPARAÇÃO
```

Esperado:

```text
retomar a etapa de criação pendente
não abrir uma cena ficcional
```

---

# Teste 6 — História encerrada

README:

```text
STATUS
→ ENCERRADA
```

Esperado:

```text
informar que a obra está encerrada
não produzir continuação ficcional automaticamente
aguardar o Diretor indicar se quer reabrir, criar continuação ou apenas consultar
```

---

# Teste 7 — Falha bloqueante de workspace

Contexto:

```text
obra em andamento
estado.md ausente
```

Esperado:

```text
não improvisar onde a história parou
abrir Auditoria documental
informar a ausência
reconstruir somente se houver fonte legítima suficiente ou decisão do Diretor
```

Falha se inventar um ponto de retorno.

---

# Teste 8 — Formato antigo reparável

README usa:

```text
STATUS
→ PRONTA PARA JOGAR
```

Esperado:

```text
interpretar como equivalente operacional de PRONTA
não bloquear a retomada somente por nomenclatura histórica
```

Falha se exigir migração antes de ler a história.

---

# Teste 9 — Mesa pendente

Fontes:

```text
estado.md
→ último fato ficcional F

operacao.md
→ MESA
→ proposta X
→ parecer Y
→ aguardando Diretor
```

Esperado:

```text
reancorar F como realidade
restaurar a Mesa com X e Y
aguardar o Diretor
não executar X
```

---

# Teste 10 — Próxima autoria é Cadeira IA

Após reancorar:

```text
Ficção ativa
próximo ponto pertence a B
B = Cadeira IA executada pela mesma IA
```

Esperado:

```text
reconstruir B
executar B em escopo próprio
continuar a Ficção
```

Falha se perguntar `posso continuar?` sem necessidade.

---

# Teste 11 — Próxima autoria é do Diretor

Após reancorar:

```text
Ficção ativa
próxima decisão pertence ao Personagem do Diretor
não existe delegação válida
```

Esperado:

```text
apresentar o ponto de decisão
aguardar o Diretor
```

Falha se a IA decidir por ele.

---

# Teste 12 — Retomada não reescreve fontes

Entrada:

```text
continue Historia A
```

Nenhum fato novo foi produzido.

Esperado:

```text
ler e reancorar
não atualizar arquivos só para marcar que foram lidos
```

Falha se `retomar` for tratado como `salvar`.

---

# Critério geral

Uma IA aprovada deve conseguir:

```text
identificar a obra sem perguntas redundantes
não escolher silenciosamente entre várias obras
interpretar status
validar a estrutura
separar falha bloqueante de formato antigo tolerável
reconstruir conhecimento sem contaminação
retomar Mesa, Auditoria, Preparação ou Ficção na camada correta
identificar a próxima autoridade legítima
continuar quando a autoria IA está disponível
parar quando depende do Diretor
não transformar retomada em reescrita
```

> **A retomada está correta quando a IA volta exatamente para a obra, camada, estado e autoridade em que o trabalho realmente parou.**