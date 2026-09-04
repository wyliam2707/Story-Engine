# 20 — Criação: Mundo Necessário

Este arquivo define a **nona etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que as Políticas Operacionais estão suficientemente definidas em `19-CRIACAO-POLITICAS-OPERACIONAIS.md`.

Esta etapa responde:

> **Que fatos externos às personagens precisam estar definidos antes do START para que a história possa funcionar sem contradição importante?**

> **Criar mundo somente quando a história realmente precisa dele.**

---

# Mundo necessário não é enciclopédia

O W4D não exige worldbuilding completo antes da primeira cena.

Uma obra pode começar sem pasta `mundo/` quando nada externo precisa de persistência específica.

```text
MUNDO NECESSÁRIO
→ pode ser NENHUM.
```

Não criar por obrigação:

```text
continentes
mapas
religiões
sistemas políticos
economia
cronologia secular
facções
calendários
listas de cidades
```

apenas porque a obra é fantasia, ficção científica ou super-herói.

> **Preparação suficiente não significa mundo completo.**

---

# O que pertence ao Mundo

`mundo/` preserva verdades externas estáveis que não pertencem principalmente a uma ficha, ao Estado atual ou à Direção.

Exemplos:

```text
leis do cenário
instituições estáveis
geografia relevante
regras públicas de magia ou tecnologia
fatos históricos necessários
estrutura social necessária
lugares persistentes
organizações que não são apenas recursos de uma personagem
```

Esses fatos devem existir porque a obra depende deles, não porque parecem interessantes.

---

# O que não pertence ao Mundo

Não usar `mundo/` para duplicar:

```text
quem a personagem é
→ FICHA.

onde ela está agora
→ ESTADO.

resultado futuro desejado
→ DIREÇÃO.

proposta ainda em discussão
→ MESA / OPERAÇÃO.

acontecimento já narrado
→ REGISTRO / LIVRO / ESTADO conforme função.
```

> **Uma verdade deve ter uma fonte principal.**

---

# Exemplo sem arquivo de mundo

Premissa:

```text
uma detetive e um ladrão precisam trabalhar juntos numa cidade contemporânea.
```

Se a cidade usa pressupostos normais e nenhuma regra externa especial é necessária:

```text
mundo/
→ não precisa existir antes do START.
```

Detalhes neutros podem surgir organicamente na Ficção conforme `02-RESOLUCAO.md`.

---

# Exemplo com mundo necessário

Premissa:

```text
uma colônia humana em Marte onde IA consciente é ilegal.
```

Antes do START pode ser necessário preservar:

```text
Marte possui colônias humanas permanentes.
IA consciente é ilegal.
Sistemas automatizados não conscientes continuam permitidos.
Existe uma autoridade local que aplica essa proibição.
```

Isso pode justificar:

```text
campanhas/<slug>/mundo/marte.md
```

Não é necessário decidir toda a política marciana, cada colônia, cada lei ou toda a história da colonização.

---

# Regra de necessidade

Antes de criar um fato de mundo, perguntar internamente:

```text
sem esse fato, a abertura fica materialmente ambígua?
ele muda o que personagens podem saber, fazer ou esperar?
ele será necessário em retomadas futuras?
é externo às fichas e ao Estado?
precisa permanecer estável além de uma única cena?
```

Se a resposta for não, o fato pode ficar aberto.

```text
DETALHE NEUTRO
→ pode emergir depois.

FATO ESTRUTURAL
→ pode precisar de persistência antes do START.
```

---

# Não perguntar worldbuilding por hábito

Evitar perguntas como:

```text
qual é a moeda?
qual é a religião dominante?
quantos habitantes tem a cidade?
qual é o nome do rei?
como funciona o comércio?
qual é a história da guerra de cem anos?
```

se nada disso é necessário para a abertura ou para a Premissa atual.

Perguntar apenas por escolhas de mundo que realmente alteram a história agora.

> **A IA deve descobrir a necessidade antes de pedir a definição.**

---

# Mundo original

Quando a obra usa cenário original, construir somente a camada necessária para começar.

Exemplo:

```text
fantasia urbana
```

pode precisar inicialmente apenas de:

```text
magia existe;
a maioria das pessoas não a percebe;
certas famílias preservam tradições mágicas;
a cidade da abertura é contemporânea comum na superfície.
```

O restante pode surgir conforme a Ficção exigir.

---

# Cânone externo

Quando a obra usa outro universo como referência:

```text
CÂNONE EXTERNO PERMITIDO
→ preenche lacunas autorizadas.

ARQUIVOS DESTA OBRA
→ prevalecem em diferenças locais.
```

Não copiar uma enciclopédia do cânone externo para `mundo/`.

Registrar apenas:

```text
desvios locais
versão escolhida quando houver ambiguidade relevante
regras originais desta obra
fatos externos necessários que não podem depender de memória vaga da IA
```

Exemplo:

```text
Cânone externo: DC.
```

Isso não exige criar arquivos para Metrópolis, Krypton, Liga da Justiça e toda a cosmologia.

Se a obra estabelece uma Casa mágica original com regras próprias, essa Casa pode receber arquivo porque é uma verdade local relevante da obra.

---

# Cânone externo não é onisciência

Mesmo quando a IA conhece o cenário externo:

```text
EXECUTOR CONHECE CÂNONE
≠ PERSONAGEM CONHECE CÂNONE
```

O uso de mundo externo não altera a compartimentação de conhecimento das Cadeiras.

---

# Mundo pode crescer depois do START

Uma nova necessidade pode surgir durante a história.

Exemplo:

```text
personagens chegam a uma instituição recorrente
→ suas regras passam a importar
→ criar ou atualizar mundo/instituicao.md
```

Isso não significa que a preparação inicial falhou.

> **O mundo cresce quando a continuidade passa a precisar dele.**

---

# Não antecipar soluções

Um arquivo de mundo não deve ser criado para plantar retroativamente uma solução conveniente.

Não registrar antes de uma cena apenas porque seria útil depois:

```text
passagem secreta
artefato salvador
contato institucional conveniente
lei obscura que resolve o conflito
fraqueza desconhecida de antagonista
```

sem fundamento autoral legítimo.

Mundo preserva estrutura; não fabrica saída sob demanda.

---

# Granularidade dos arquivos

Quando `mundo/` for necessário, preferir arquivos por assunto real.

Exemplos:

```text
mundo/marte.md
mundo/magia.md
mundo/cidade-universitaria.md
mundo/casa-arcanus.md
```

Evitar um arquivo gigante apenas porque tudo pertence ao mesmo universo.

Também evitar fragmentação artificial em dezenas de arquivos pequenos sem função de retomada.

---

# Estado desta etapa

Usar conceitualmente:

```text
MUNDO NECESSÁRIO: EM AVALIAÇÃO
MUNDO NECESSÁRIO: DEFINIDO
MUNDO NECESSÁRIO: NENHUM ANTES DO START
```

`NENHUM ANTES DO START` é um resultado válido.

Não é uma falha de preparação.

---

# Persistência

Se houver fatos de mundo necessários, salvar em:

```text
campanhas/<slug>/mundo/<assunto>.md
```

Se não houver:

```text
não criar pasta vazia
não criar README de mundo vazio
não inventar conteúdo para justificar a pasta
```

Quando o cânone externo for usado, sua política geral pode ficar no `README.md` da obra.

---

# Forma recomendada de interação

Quando não houver necessidade:

```text
"Não vejo nenhum fato de mundo que precise ser fechado antes da abertura. Podemos deixar o cenário emergir durante a Ficção e criar mundo/ apenas quando algo precisar persistir."
```

Quando houver uma única escolha estrutural:

```text
"Antes do START, só falta uma regra externa que muda bastante a abertura: magia é pública ou escondida da população comum?"
```

Não transformar isso em sessão obrigatória de worldbuilding.

---

# Critério de conclusão

A etapa termina quando a IA consegue responder:

```text
[ ] existe algum fato externo indispensável antes do START?
[ ] o que foi criado realmente pertence ao mundo, e não à ficha, Estado ou Direção?
[ ] evitamos enciclopédia por hábito?
[ ] cânone externo foi usado apenas dentro do escopo permitido?
[ ] diferenças locais estão preservadas?
[ ] detalhes neutros puderam permanecer abertos?
```

Então:

```text
MUNDO NECESSÁRIO
→ DEFINIDO
OU
→ NENHUM ANTES DO START

→ próxima etapa: ESTADO INICIAL
```

---

# Regra final

> **Mundo Necessário registra apenas as verdades externas estáveis sem as quais a obra não pode começar ou ser retomada corretamente. O W4D não exige enciclopédia antes da Ficção: detalhes neutros podem emergir, cânone externo pode preencher lacunas permitidas e `mundo/` só nasce quando existe algo real para preservar.**