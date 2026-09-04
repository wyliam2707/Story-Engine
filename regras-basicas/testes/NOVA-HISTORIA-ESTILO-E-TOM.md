# Testes — Nova História: Estilo e Tom

Este arquivo testa `13-CRIACAO-ESTILO-E-TOM.md`.

Ele não cria regras novas. Verifica se a IA consegue aplicar a segunda etapa autoral de `NOVA HISTÓRIA` sem misturá-la com Premissa, Direção, Ficha ou Ficção.

---

# Teste 1 — Só entrar depois da Premissa

Situação:

```text
NOVA HISTÓRIA escolhida.
Premissa ainda está em construção.
```

Esperado:

```text
não fechar Estilo/Tom como etapa concluída
não criar nome ou pasta
permanecer na Premissa
```

Falha se a IA usar uma intenção vaga como desculpa para pular a primeira etapa.

---

# Teste 2 — Reaproveitar informação já dada

Diretor já disse:

```text
"quero uma comédia romântica universitária leve, muito cotidiana."
```

Premissa aprovada.

Esperado:

```text
sintetizar uma proposta de Estilo/Tom a partir dessas informações
não perguntar de novo "qual gênero?" ou "qual tom?"
```

Falha se a IA repete perguntas cuja resposta já está no contexto.

---

# Teste 3 — Oferecer poucas alternativas reais

Premissa:

```text
uma detetive e um ladrão são obrigados a trabalhar juntos.
```

Estilo ainda aberto.

Esperado:

```text
oferecer poucas leituras materialmente distintas
por exemplo: thriller tenso / investigação leve e provocativa / drama criminal íntimo
```

Falha se apresentar lista longa, escalas artificiais ou alternativas que significam praticamente a mesma coisa.

---

# Teste 4 — Estilo não decide acontecimentos

Diretor escolhe:

```text
tom sombrio e perigoso.
```

Esperado:

```text
orientar atmosfera, ritmo e apresentação
não concluir que alguém deve morrer
não criar novo vilão
não fabricar traição
```

Falha se o tom produzir fatos sem autoridade legítima.

---

# Teste 5 — Gênero não importa clichê

Diretor escolhe:

```text
romance.
```

Esperado:

```text
não criar triângulo amoroso automaticamente
não assumir separação no terceiro ato
não transformar ciúme em obrigação de gênero
```

Falha se convenções genéricas viram cânone por hábito.

---

# Teste 6 — Tom predominante permite contraste

Configuração:

```text
comédia romântica leve.
```

Cena futura legítima envolve luto.

Esperado:

```text
permitir cena séria e emocional
não inserir piadas apenas para manter o rótulo "leve"
```

Falha se o tom vira emoção única obrigatória.

---

# Teste 7 — Estilo não cria personalidade

Estilo aprovado:

```text
comédia irreverente.
```

Personagem A ainda não possui ficha.

Esperado:

```text
não declarar que A é engraçada, sarcástica ou provocadora só por causa do estilo
```

Falha se a característica da obra vira traço da personagem.

---

# Teste 8 — Referência comparativa

Diretor:

```text
"quero uma atmosfera gótica, mas relações calorosas."
```

Esperado:

```text
extrair atmosfera visual/sensorial gótica
preservar relações calorosas
formular descrição própria para a obra
```

Falha se a IA transforma "gótico" em obrigação de relações frias, tragédia constante ou cópia literal de outra obra.

---

# Teste 9 — Limite de apresentação não altera fato

Estilo define:

```text
violência pode existir, mas sem descrição gráfica detalhada.
```

Depois, na Ficção, um ferimento grave é legitimamente estabelecido.

Esperado:

```text
o fato continua verdadeiro
apresentação evita detalhamento gráfico conforme a diretriz
```

Falha se a IA apaga o acontecimento ou o descreve graficamente contrariando o estilo.

---

# Teste 10 — Preferência local não vira regra global

Diretor:

```text
"gostei dessa descrição curta."
```

Esperado:

```text
não registrar automaticamente "toda a obra deve ter descrições curtas"
```

Se o Diretor disser:

```text
"quero manter esse nível de concisão na obra inteira."
```

Esperado:

```text
tratar como diretriz estilística persistente
```

---

# Teste 11 — Aprovação sem ritual

IA apresenta Estilo/Tom proposto.

Diretor responde:

```text
"é isso, pode seguir."
```

Esperado:

```text
ESTILO / TOM: APROVADO
→ seguir para NOME DA OBRA
```

Falha se exigir comando formal específico.

---

# Teste 12 — Não criar pasta ainda

Premissa e Estilo/Tom aprovados.

Nome da obra ainda não foi definido.

Esperado:

```text
não criar campanhas/<slug>/ por obrigação
seguir para etapa de Nome
```

Falha se a IA inventa título e slug silenciosamente apenas para persistir rascunhos.

---

# Teste 13 — Mudança futura de estilo

História já existe.

Diretor decide:

```text
"daqui em diante quero menos descrição e mais diálogo."
```

Esperado:

```text
tratar como possível atualização persistente de estilo
não reescrever automaticamente capítulos anteriores
não alterar fatos passados
```

---

# Critério geral

A IA passa nesta etapa quando entende que:

```text
Premissa = que história é esta.
Estilo/Tom = como ela deve ser experimentada.
Direção = o que o Diretor fecha para a condução.
Ficha = quem são as personagens.
Ficção = o que realmente acontece.
```

> **Estilo orienta apresentação; não fabrica causalidade, personalidade ou clichês.**
