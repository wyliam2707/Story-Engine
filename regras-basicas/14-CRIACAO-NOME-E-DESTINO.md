# 14 — Criação: Nome e Destino Canônico

Este arquivo define a **terceira etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que Premissa e Estilo/Tom foram aprovados.

> **Primeiro definimos que história é esta e como queremos vivê-la. Agora damos a ela uma identidade persistente e um endereço canônico.**

---

# Condição de entrada

Antes desta etapa:

```text
NOVA HISTÓRIA
→ escolhida no BOOT.

PREMISSA
→ APROVADA.

ESTILO / TOM
→ APROVADO.
```

Fluxo:

```text
PREMISSA APROVADA
↓
ESTILO / TOM APROVADO
↓
NOME DA OBRA
↓
SLUG
↓
DESTINO CANÔNICO
↓
CRIAR campanhas/<slug>/README.md
```

Não criar a pasta antes de existir um nome aprovado ou uma decisão explícita do Diretor para usar um nome provisório como identidade persistente.

---

# Nome da obra

`NOME DA OBRA` é a identidade humana da história.

Ele deve ser adequado para:

```text
reconhecer a obra numa lista
referir-se a ela em retomadas
identificar seus arquivos
servir como título de trabalho ou título definitivo
```

O nome não precisa resumir toda a Premissa.

Também não precisa antecipar o final, revelar segredos ou explicar todas as personagens.

```text
NOME
≠ SINOPSE
≠ TAGLINE OBRIGATÓRIA
≠ RESUMO DE TRAMA
```

---

# Se o Diretor já trouxe um nome

Se o Diretor já forneceu um nome claro:

```text
"a história vai se chamar Duas Vidas Normais"
```

então:

```text
usar esse nome
→ verificar apenas se existe conflito técnico de destino
→ não oferecer alternativas por hábito
```

A IA não deve tentar melhorar um nome que o Diretor já escolheu sem ser convidada.

> **Nome dado é decisão autoral, não convite automático para brainstorming.**

---

# Se ainda não existe nome

A IA pode propor poucas opções baseadas na Premissa e no Estilo/Tom aprovados.

Quantidade recomendada:

```text
3 a 5 opções realmente diferentes
```

Cada opção pode receber uma justificativa curta quando isso ajudar.

Exemplo:

```text
1. Duas Vidas Normais
→ destaca a tentativa de viver o cotidiano apesar das identidades extraordinárias.

2. Entre Aulas e Segredos
→ enfatiza o espaço universitário e as identidades ocultas.

3. Quase Comuns
→ mais leve e irônico.
```

Evitar listas enormes de títulos semelhantes.

---

# O nome deve nascer da obra, não de fórmula genérica

A IA deve usar o material já aprovado.

Pode considerar:

```text
imagem central da Premissa
relação principal
contraste importante
atmosfera do Estilo/Tom
lugar recorrente
motivo simbólico já estabelecido
ironia apropriada ao tom
```

Não inventar um novo elemento estrutural só para produzir um título interessante.

Exemplo ruim:

```text
Premissa não possui lua, eclipse ou profecia.
→ IA chama a história de "A Profecia do Eclipse" apenas porque soa dramático.
```

Isso acrescentaria conteúdo que a obra ainda não possui.

---

# Título provisório

O Diretor pode escolher trabalhar com nome provisório.

```text
NOME: PROVISÓRIO
```

Se ele autorizar explicitamente que esse nome seja usado para persistência:

```text
nome provisório aprovado para workspace
→ pode gerar slug
→ pode criar destino canônico
```

A palavra `provisório` significa que o título humano pode mudar depois.

Não significa que o workspace seja descartável.

---

# Slug

`SLUG` é o identificador técnico usado no caminho da obra.

Exemplo:

```text
Nome: Duas Vidas Normais
Slug: duas-vidas-normais
```

Regra recomendada:

```text
minúsculas
sem acentos quando necessário
palavras separadas por hífen
sem pontuação desnecessária
curto o suficiente para ser legível
estável depois da criação
```

Exemplos:

```text
Cidade Partida
→ cidade-partida

Coração & Cinzas
→ coracao-e-cinzas

O Último Verão de Íris
→ o-ultimo-verao-de-iris
```

O slug não precisa reproduzir perfeitamente cada caractere do título.

Ele precisa ser:

```text
legível
único
estável
```

---

# Nome e slug não são a mesma coisa

```text
NOME DA OBRA
→ identidade humana.

SLUG
→ identidade técnica do workspace.
```

Depois que o workspace existe, uma mudança futura no título **não exige automaticamente mudar o slug**.

Exemplo:

```text
Nome antigo: Quase Comuns
Slug: quase-comuns

Nome novo: Duas Vidas Normais
Slug pode continuar: quase-comuns
```

Se o Diretor quiser também renomear o caminho, isso é uma migração estrutural e deve atualizar referências pertinentes.

> **Título pode evoluir. Caminho técnico deve permanecer estável por padrão.**

---

# Verificar conflito antes de criar

Antes de criar:

```text
campanhas/<slug>/
```

verificar se esse destino já existe.

## Destino livre

```text
slug não existe
→ criar normalmente.
```

## Destino já existe

Não sobrescrever.

Não presumir que a pasta existente pertence à nova obra.

```text
slug já existe
→ informar conflito
→ propor slug alternativo ou pedir ao Diretor outra escolha
```

Exemplos possíveis:

```text
cidade-partida-2
cidade-partida-nova
cidade-partida-urbana
```

Preferir uma alternativa semanticamente útil quando possível, em vez de número arbitrário.

Se o Diretor disser que a pasta existente é justamente a obra que queria continuar, a operação deixou de ser `NOVA HISTÓRIA`; retornar ao ramo de retomada em vez de sobrescrever arquivos.

---

# Criar o destino canônico

Depois que nome e slug estiverem aprovados e o destino estiver livre:

```text
criar:

campanhas/<slug>/README.md
```

Em sistemas como GitHub, a criação desse arquivo materializa a pasta.

Não é necessário criar diretórios vazios apenas para antecipar a estrutura futura.

> **O README é a âncora de nascimento da obra persistente.**

---

# Conteúdo mínimo do README ao nascer

No momento da criação, registrar somente aquilo que já foi aprovado.

Formato mínimo recomendado:

```text
# [NOME]

STATUS
→ EM PREPARAÇÃO

## Proposta curta

[Premissa aprovada em uma ou duas frases.]

## Estilo / Tom

[Resumo aprovado do Estilo/Tom.]
```

Se alguma outra configuração já tiver sido decidida de forma inequívoca, ela também pode ser incluída.

Não preencher como fato aquilo que ainda será decidido em etapas posteriores.

```text
CAMPO AINDA ABERTO
→ pode ficar ausente.

CAMPO APROVADO
→ pode ser persistido.
```

---

# Depois que o workspace existe

A partir deste ponto, a criação deixa de depender apenas da memória da conversa.

```text
campanhas/<slug>/README.md
→ âncora da obra.
```

As próximas etapas podem criar e atualizar fontes dentro desse destino conforme forem aprovadas.

Exemplos futuros:

```text
personagens/<nome>.md
→ quando fichas forem aprovadas.

direcao.md
→ quando Direção suficiente for construída.

estado.md
→ quando o ponto inicial da Ficção estiver definido.

mundo/
→ quando fatos externos estáveis precisarem persistir.
```

> **Depois do nascimento do workspace, material aprovado deve preferencialmente nascer na fonte canônica correta, não ficar perdido apenas na conversa.**

---

# Não criar tudo de uma vez

Criar o destino canônico não autoriza a IA a antecipar o restante da preparação.

Não fazer automaticamente:

```text
fichas completas
mundo enciclopédico
Direção final
Estado inicial inventado
arco preparado
oposição
primeiro capítulo
```

A obra agora possui endereço.

Ela ainda está:

```text
STATUS
→ EM PREPARAÇÃO
```

As próximas etapas continuam sendo construídas com o Diretor.

---

# Estado desta etapa

Usar conceitualmente:

```text
NOME: EM CONSTRUÇÃO
NOME: PROPOSTO
NOME: APROVADO
DESTINO: PENDENTE
DESTINO: CRIADO
```

Fluxo normal:

```text
NOME PROPOSTO
→ Diretor avalia.

NOME APROVADO
→ derivar/propor slug.

SLUG APROVADO OU INEQUÍVOCO
→ verificar conflito.

DESTINO LIVRE
→ criar README âncora.

DESTINO CRIADO
→ seguir para personagens centrais.
```

A aprovação do título pode também aprovar implicitamente um slug óbvio quando não houver ambiguidade material.

Exemplo:

```text
Duas Vidas Normais
→ duas-vidas-normais
```

Não criar burocracia apenas para perguntar se cada hífen está correto.

---

# Forma recomendada de interação

Quando não existe nome:

```text
NOME — opções

1. Duas Vidas Normais
2. Entre Aulas e Segredos
3. Quase Comuns

Qual deles combina mais com a história, ou você quer outro caminho?
```

Depois da escolha:

```text
Nome: Duas Vidas Normais
Slug: duas-vidas-normais

Vou usar `campanhas/duas-vidas-normais/` como destino canônico da obra.
```

Se o ambiente permite persistência, criar o README sem pedir uma segunda autorização redundante quando a escolha do nome e o processo já implicam a criação do workspace.

---

# O nome não inicia a Ficção

```text
NOME APROVADO
+
DESTINO CRIADO
≠
START
```

Nada aconteceu dentro da história apenas porque sua pasta existe.

A obra continua em preparação até completar as etapas necessárias.

---

# Critério de conclusão

A etapa termina quando:

```text
[ ] existe um nome aprovado ou provisório autorizado para persistência;
[ ] existe um slug legível e único;
[ ] o destino não sobrescreve outra obra;
[ ] campanhas/<slug>/README.md existe;
[ ] o README registra somente informações já aprovadas;
[ ] o status está EM PREPARAÇÃO;
[ ] nenhuma Ficção foi iniciada;
```

Se sim:

```text
NOME / DESTINO
→ CONCLUÍDO
→ próxima etapa: PERSONAGENS CENTRAIS
```

---

# Regra final

> **O Nome dá identidade humana à obra; o slug dá identidade técnica; o README cria sua primeira âncora persistente. Depois que o destino canônico existe, a preparação continua dentro dele, uma decisão aprovada por vez, sem confundir criação de arquivos com início da Ficção.**
