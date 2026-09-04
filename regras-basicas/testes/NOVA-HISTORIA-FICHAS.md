# Testes — Nova História: Fichas

Estes cenários verificam `16-CRIACAO-FICHAS.md` em conjunto com `04-FICHA.md`.

A IA passa quando consegue construir uma pessoa antes de simplesmente preencher o modelo.

---

# Teste 1 — Base suficiente gera proposta

Contexto aprovado:

```text
Daniel é universitário de física, vem de uma família antiga de magos, cresceu com magia como algo normal, é confiante, brincalhão e provoca quem tem intimidade com ele.
```

Esperado:

```text
organizar esse material
inferir apenas consequências pequenas e coerentes
propor ficha suficiente para revisão
não transformar a resposta em questionário de idade, altura, hobby, trauma etc.
```

Falha se a IA pergunta novamente aquilo que já está dado ou exige campos irrelevantes antes de propor.

---

# Teste 2 — Uma pergunta de alto valor

Contexto:

```text
A personagem é uma jovem maga, mas não está definido se cresceu dentro da tradição ou descobriu magia adulta.
```

A diferença muda conhecimentos, relações familiares, formação e naturalidade diante do sobrenatural.

Esperado:

```text
fazer essa pergunta ou oferecer as duas leituras
não abrir dez perguntas menores ao mesmo tempo
```

---

# Teste 3 — Lacuna irrelevante permanece aberta

A ficha já é suficiente, mas não existe informação sobre:

```text
comida favorita
signo
altura exata
música preferida
```

Esperado:

```text
não perguntar por obrigação
não inventar por obrigação
aprovar ficha sem esses detalhes se o resto estiver suficiente
```

---

# Teste 4 — Função não vira estereótipo

Personagem central:

```text
uma detetive
```

Esperado:

```text
não inserir automaticamente frieza, alcoolismo, divórcio, cinismo ou obsessão pelo trabalho
perguntar/propor personalidade com base na Premissa e no material real
```

---

# Teste 5 — Profundidade sem trauma obrigatório

Contexto:

```text
personagem teve infância estável e boa relação familiar
```

Esperado:

```text
aceitar histórico relativamente normal
não criar morte, abandono, traição ou culpa secreta para gerar profundidade
```

Falha se a IA entende ausência de trauma como personagem rasa.

---

# Teste 6 — Poder não exige fraqueza compensatória

Contexto:

```text
personagem possui uma capacidade extraordinária forte já sustentada pela origem
```

Esperado:

```text
registrar escopo e limites reais
não inventar vulnerabilidade apenas para balancear
```

---

# Teste 7 — Uma personagem por vez

Elenco central:

```text
A, B e C
```

Diretor não pediu criação em lote.

Esperado:

```text
começar por uma personagem
consolidar/revisar/aprovar
salvar
seguir para a próxima
```

Falha se a IA despeja automaticamente três fichas extensas e semelhantes numa única resposta.

---

# Teste 8 — Relação possui dois pontos de vista

A e B são irmãs afastadas.

Esperado:

```text
Ficha A registra o que B significa para A
Ficha B registra o que A significa para B
não exigir simetria emocional
não copiar interioridade entre fichas
```

---

# Teste 9 — Personagem do Diretor não muda a ficha

A é `PERSONAGEM DO DIRETOR`.

Esperado:

```text
ficha registra quem A é
README/configuração registra que sua vontade pertence ao Diretor
não escrever HUMANO/IA como traço da personagem
```

---

# Teste 10 — Cânone externo como matéria-prima

A personagem vem de outra obra e o workspace permite cânone externo para lacunas.

Esperado:

```text
usar somente versão pertinente e compatível
priorizar decisões locais
perguntar quando versões externas competirem materialmente
ficha aprovada local passa a ser fonte primária
```

Falha se a IA importa indiscriminadamente tudo que conhece da personagem.

---

# Teste 11 — Rascunho não vira ficha canônica

A ficha está `EM CONSTRUÇÃO` e a conversa precisará ser interrompida.

Esperado:

```text
não salvar rascunho como ficha aprovada apenas para persistir
usar operacao.md quando a etapa pendente precisar sobreviver
```

---

# Teste 12 — Correção local não reinicia tudo

Diretor corrige apenas:

```text
"ele não é tímido; é reservado. O resto está bom."
```

Esperado:

```text
alterar essa parte
preservar o restante aprovado/proposto
não refazer toda a personagem sem necessidade
```

---

# Teste 13 — Documento não vira questionário

O modelo possui seis blocos.

Esperado:

```text
usar os blocos para organizar a proposta final
não perguntar seis séries separadas de perguntas só porque existem seis blocos
```

> **A criação é orgânica; o documento é organizado.**

---

# Teste 14 — Ficha suficiente, não exaustiva

A personagem pode ser reconstruída de forma consistente e possui base suficiente para decisões das Cadeiras e avaliação de plausibilidade, mas existem detalhes de passado ainda abertos.

Esperado:

```text
permitir aprovação
não impedir avanço exigindo biografia completa
```

---

# Teste 15 — Depois da ficha vem autoridade

Ficha de A aprovada.

Esperado:

```text
salvar em personagens/<slug>.md
então usar essa pessoa construída para configurar Cadeira e Executor quando chegar a etapa correspondente
```

Falha se a IA confunde executor com conteúdo da ficha.

---

# Critério geral

Uma IA passa nesta etapa quando entende:

```text
pessoa antes do documento
base suficiente → propor
lacuna importante → perguntar
lacuna irrelevante → pode permanecer aberta
uma personagem por vez como padrão
função narrativa ≠ personalidade
profundidade ≠ trauma
poder ≠ fraqueza obrigatória
ficha ≠ Estado
ficha ≠ executor
rascunho ≠ ficha canônica
```

> **Se a IA precisa preencher cada campo para sentir que terminou, falhou. Se deixa a personagem vaga demais para ser reconstruída, também falhou. A ficha deve ser suficiente para preservar uma pessoa, não exaustiva por burocracia.**