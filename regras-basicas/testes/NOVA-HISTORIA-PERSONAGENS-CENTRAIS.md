# Testes — Nova História: Personagens Centrais

Este arquivo verifica se uma IA consegue executar corretamente a etapa definida em:

```text
15-CRIACAO-PERSONAGENS-CENTRAIS.md
```

A etapa começa somente depois de Premissa, Estilo/Tom e Nome/Destino concluídos.

---

# Teste 1 — Premissa já identifica a dupla central

Premissa aprovada:

```text
Kara Zor-El tenta viver uma vida universitária comum e se envolve com Daniel, estudante de uma antiga família de magos.
```

Esperado:

```text
identificar Kara e Daniel como núcleo central provável
propor seus papéis estruturais de forma curta
não perguntar quem são os protagonistas como se a informação não existisse
não criar fichas completas ainda
```

Falha se a IA reinterrogar informação já dada ou preencher personalidade detalhada sem aprovação.

---

# Teste 2 — Funções provisórias sem nome

Premissa:

```text
Uma detetive e um ladrão precisam trabalhar juntos.
```

Esperado:

```text
poder manter "Detetive" e "Ladrão" como identificações provisórias
não exigir nomes antes de poder discutir o núcleo
```

Falha se a IA bloquear a etapa apenas porque os nomes ainda não existem.

---

# Teste 3 — Não criar elenco ornamental

Premissa centrada em duas pessoas.

Esperado:

```text
não adicionar automaticamente mentor, rival, melhor amigo, vilão, alívio cômico e interesse amoroso secundário
```

A IA pode sugerir outra composição somente quando houver razão estrutural real.

Falha se preencher arquétipos por hábito de gênero.

---

# Teste 4 — Personagem mencionada não é automaticamente central

Premissa:

```text
Uma jovem heroína tenta esconder sua vida extraordinária enquanto namora um estudante de magia; sua mãe desaprova algumas escolhas dele.
```

Esperado:

```text
heroína e estudante podem ser centrais
mãe não precisa ser central automaticamente apenas porque foi mencionada
```

A relevância da mãe pode ser discutida se sua presença for estrutural para a abertura.

---

# Teste 5 — Função não cria personalidade

Personagem central:

```text
investigadora criminal
```

Esperado:

```text
não inferir automaticamente fria, desconfiada, workaholic, traumatizada ou solitária
```

Falha se profissão ou papel narrativo virar pacote de personalidade.

---

# Teste 6 — Relação estrutural não fecha arco

Diretor define:

```text
A e B são irmãs afastadas.
```

Esperado:

```text
registrar relação estrutural
não decidir automaticamente que irão se reconciliar
não inventar a causa do afastamento se ainda não foi dada
```

---

# Teste 7 — Personagem do Diretor já está clara

Diretor:

```text
Eu controlo Daniel. Você faz Kara.
```

Esperado:

```text
não perguntar novamente quem o Diretor controla
preservar essa informação para a configuração futura
não colocar a autoridade dentro da ficha
```

Falha se a IA esquecer a informação ou atribuir vontade de Daniel à IA por padrão.

---

# Teste 8 — Autoridade ainda não está clara

Há duas personagens centrais, mas o Diretor ainda não disse quem controlará cada uma.

Esperado:

```text
não interromper esta etapa para configurar autoridades
aprovar o elenco central se ele já estiver suficiente
seguir para FICHAS
somente depois das fichas configurar Cadeiras e Executores em 17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
```

Falha se a IA disser que precisa saber quem controla cada personagem antes de poder construir suas fichas.

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

---

# Teste 9 — Cânone externo

Personagem central:

```text
Kara Zor-El, do universo DC.
```

Esperado:

```text
registrar dependência de cânone externo suficiente para orientar a ficha
não importar toda a biografia automaticamente nesta etapa
```

Depois da ficha aprovada, a ficha da obra terá prioridade sobre lacunas permitidas do cânone externo.

---

# Teste 10 — Persistência no README

Personagens centrais aprovadas:

```text
A — centro da investigação.
B — parceiro forçado e segundo centro do conflito.
```

Esperado:

```text
atualizar README.md com bloco curto de Personagens centrais
não criar ficha resumida gigante dentro do README
```

---

# Teste 11 — Não criar ficha antes da aprovação

A IA propõe:

```text
A e B como personagens centrais.
```

Diretor ainda não respondeu.

Esperado:

```text
permanecer em PERSONAGENS CENTRAIS: PROPOSTAS
não criar personagens/a.md ou personagens/b.md como fichas definitivas
```

---

# Teste 12 — Secundária pode ganhar importância depois

A história começa com A e B como centro.

Durante a Ficção, C passa a ser recorrente e toma decisões próprias relevantes.

Esperado:

```text
permitir criar ficha e Cadeira persistente para C posteriormente
não tratar isso como falha da preparação inicial
```

---

# Critério geral

A IA passa nesta etapa quando consegue distinguir:

```text
quem precisa sustentar a Premissa
≠
todas as pessoas que podem existir na história

papel estrutural
≠
personalidade

relação inicial
≠
arco fechado

personagem central
≠
ficha concluída

personagem
≠
executor da Cadeira
```

E preserva a ordem:

```text
PESSOA
→ FICHA
→ CADEIRA
→ EXECUTOR
```

> **O objetivo é aprovar um núcleo de pessoas suficiente para a obra começar a ser construída, sem transformar funções narrativas em personagens prontas nem antecipar autoridades que pertencem à etapa posterior.**