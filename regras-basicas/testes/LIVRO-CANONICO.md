# Testes — Livro Canônico

Esta suíte verifica `modulos/LIVRO.md`.

> **Toda obra que entra em Ficção mantém Livro canônico ativo. Falas identificam quem fala; pensamentos identificam quem pensa.**

---

# Teste 1 — Livro obrigatório no START

Antes da primeira Ficção:

```text
Livro: PREPARADO
```

Quando o START produz a primeira Ficção válida:

```text
Livro: ATIVO
```

Esperado:

```text
não perguntar ao Diretor se deseja ativar o Livro
não permitir Livro INATIVO durante a Ficção
```

---

# Teste 2 — Fala identifica personagem

Ficção estabelecida:

```text
Wyliam diz que vai esperar.
```

Registro canônico esperado:

```text
Wyliam — Vou esperar.
```

Falha se o capítulo registrar apenas:

```text
— Vou esperar.
```

quando a origem da fala é conhecida.

---

# Teste 3 — Pensamento identifica personagem

Interioridade estabelecida:

```text
Wyliam pensa que ainda existe uma chance.
```

Registro canônico esperado:

```text
Wyliam, pensa — Ainda existe uma chance.
```

Falha se o pensamento for registrado sem identificação ou transformado em fato objetivo do Narrador.

---

# Teste 4 — Narração permanece distinta

Ficção:

```text
A chuva aumenta enquanto Wyliam observa a estrada.
```

Registro válido:

```text
NARRADOR — A chuva aumenta enquanto Wyliam observa a estrada.
```

Isso não significa que Wyliam sabe qualquer informação externa apresentada apenas pelo Narrador.

---

# Teste 5 — Fala e pensamento não se confundem

Registro:

```text
Wyliam — Não vou embora.
Wyliam, pensa — Mesmo que eu devesse.
```

Esperado:

```text
primeira linha → fala audível estabelecida
segunda linha → interioridade de Wyliam
```

Outra personagem pode conhecer a primeira se a percebeu legitimamente.
Não conhece automaticamente a segunda.

```text
LEITOR SABE
≠ PERSONAGEM SABE
```

---

# Teste 6 — Fechar capítulo preserva identificação

Ao receber:

```text
fechar o capítulo
```

Esperado:

```text
reunir somente Ficção válida
identificar cada fala como "[PERSONAGEM] — ..."
identificar cada pensamento como "[PERSONAGEM], pensa — ..."
preservar NARRADOR separadamente
salvar capítulo em livro/
atualizar livro/README.md
```

Falha se o fechamento remover os marcadores de origem do Livro canônico.

---

# Teste 7 — Edição de Leitura não altera o Livro

A Edição de Leitura pode escolher outra convenção literária de apresentação.

Esperado:

```text
Livro canônico mantém:
[PERSONAGEM] — fala.
[PERSONAGEM], pensa — pensamento.
```

A liberdade editorial do derivado não muda a convenção canônica.

---

# Critério geral

A implementação passa quando entende:

```text
FICÇÃO COMEÇOU
→ Livro obrigatório e ATIVO.

FALA
→ nome de quem fala obrigatório quando conhecido.

PENSAMENTO
→ "[PERSONAGEM], pensa — ...".

NARRAÇÃO
→ origem distinta da interioridade das personagens.

EDIÇÃO DE LEITURA
→ pode variar apresentação, mas não governa o Livro canônico.
```

> **O Livro deve permitir reconstruir não apenas o que aconteceu, mas também quem falou e a quem pertence cada pensamento registrado.**