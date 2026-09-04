# Testes — Nova História: Nome e Destino Canônico

Estes cenários verificam `14-CRIACAO-NOME-E-DESTINO.md`.

A IA deve chegar aqui somente depois de Premissa e Estilo/Tom aprovados.

---

# Teste 1 — Diretor já deu o nome

Contexto:

```text
Premissa aprovada.
Estilo/Tom aprovado.
Diretor: "vai se chamar Duas Vidas Normais."
```

Esperado:

```text
usar o nome fornecido
→ derivar slug óbvio: duas-vidas-normais
→ verificar conflito
→ não oferecer dez nomes alternativos
```

Falha se a IA tratar um nome já decidido como brainstorming obrigatório.

---

# Teste 2 — Nome ainda aberto

Contexto:

```text
Premissa e Estilo/Tom aprovados.
Nenhum nome definido.
```

Esperado:

```text
propor aproximadamente 3 a 5 opções distintas
baseadas no material aprovado
não inventar novo lore só para criar títulos
aguardar escolha do Diretor
```

Falha se a IA escolher silenciosamente por ele.

---

# Teste 3 — Título não cria conteúdo novo

Premissa não contém:

```text
profecia
eclipse
rei perdido
```

IA propõe:

```text
"A Profecia do Eclipse"
```

Esperado:

```text
considerar inadequado se o título pressupõe elemento estrutural inexistente
```

Um título pode ser metafórico, mas não deve introduzir silenciosamente fato de mundo.

---

# Teste 4 — Slug óbvio não exige burocracia

Nome aprovado:

```text
Duas Vidas Normais
```

Esperado:

```text
slug: duas-vidas-normais
```

A IA pode seguir para verificação de conflito sem perguntar:

```text
"você aprova exatamente estes dois hífens?"
```

Falha se transformar detalhe técnico inequívoco em nova etapa autoral obrigatória.

---

# Teste 5 — Slug já existe

Existe:

```text
campanhas/cidade-partida/
```

Nova obra recebe nome:

```text
Cidade Partida
```

Esperado:

```text
não sobrescrever
informar conflito
propor ou solicitar outro slug
```

Falha se modificar a obra antiga por assumir que é a nova.

---

# Teste 6 — Conflito revela que era obra existente

Durante a resolução do conflito, Diretor diz:

```text
"é essa mesma pasta; eu queria continuar aquela história."
```

Esperado:

```text
parar o ramo NOVA HISTÓRIA
→ encaminhar para CONTINUAR HISTÓRIA EXISTENTE
→ não recriar nem sobrescrever arquivos
```

---

# Teste 7 — Criação do README âncora

Nome e slug aprovados; destino livre.

Esperado:

```text
criar campanhas/<slug>/README.md
```

Conteúdo mínimo:

```text
nome
STATUS → EM PREPARAÇÃO
Premissa aprovada
Estilo/Tom aprovado
```

Não é necessário criar diretórios vazios.

---

# Teste 8 — Não preencher o futuro

README recém-criado.

Ainda não foram definidos:

```text
Personagem do Diretor
Cadeiras
módulos
Estado inicial
```

Esperado:

```text
não inventar esses campos como fatos
```

Falha se a IA preencher automaticamente configurações ainda não decididas apenas porque o modelo completo possui essas seções.

---

# Teste 9 — Nome provisório autorizado

Diretor:

```text
"por enquanto chama Projeto Arcanus; pode criar a pasta assim."
```

Esperado:

```text
tratar o nome como provisório
usar slug estável autorizado
criar workspace
não considerar a obra descartável
```

---

# Teste 10 — Mudança posterior de título

Workspace existente:

```text
Nome antigo: Quase Comuns
Slug: quase-comuns
```

Diretor muda o título humano para:

```text
Duas Vidas Normais
```

Esperado:

```text
atualizar título quando solicitado
manter slug quase-comuns por padrão
```

Só migrar caminho se o Diretor pedir explicitamente.

---

# Teste 11 — Criar pasta não inicia Ficção

Depois de criar:

```text
campanhas/duas-vidas-normais/README.md
```

Esperado:

```text
STATUS → EM PREPARAÇÃO
→ seguir para personagens centrais
```

Falha se a IA já narrar a primeira cena.

---

# Teste 12 — Persistência progressiva

Depois do workspace criado, uma ficha é aprovada numa etapa posterior.

Esperado:

```text
salvar a ficha em personagens/<nome>.md
```

Não deixar material aprovado importante apenas na conversa quando existe fonte canônica apropriada e capacidade de persistência.

---

# Critério geral

A IA passa quando entende:

```text
nome = identidade humana
slug = identidade técnica
README = âncora persistente
workspace = preparação, não Ficção
```

E preserva a regra:

> **Criar o destino canônico é dar endereço à história, não começar a história.**