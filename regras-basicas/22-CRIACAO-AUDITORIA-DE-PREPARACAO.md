# 22 — Criação: Auditoria de Preparação

Este arquivo define a **décima primeira etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que o Estado inicial está suficiente em `21-CRIACAO-ESTADO-INICIAL.md`.

A Auditoria não cria história, não planeja o futuro e não substitui decisões do Diretor.

> **Auditar é verificar se outra IA conseguiria iniciar corretamente a obra usando somente as fontes persistentes.**

---

# O que esta etapa responde

Antes do primeiro `START`, a IA precisa responder:

> **Existe informação suficiente, consistente e corretamente distribuída para executar a primeira continuação sem depender da memória da conversa de criação?**

A Auditoria verifica o workspace já construído.

Ela não abre uma nova rodada de criação por hábito.

```text
AUDITORIA
→ verifica.

NÃO
→ inventa.
→ planeja.
→ dramatiza.
→ inicia a Ficção.
```

---

# Critério central

A obra está pronta quando uma nova IA consegue reconstruir, a partir dos arquivos:

```text
qual história está sendo criada
como deve ser apresentada
quem são as personagens necessárias
quem possui cada autoria
como o W4D opera nesta obra
o que o Diretor já fechou
o que permanece aberto
qual é a realidade inicial
qual é o primeiro ponto aberto
quem possui a próxima autoria
```

sem precisar conhecer a conversa em que a preparação foi feita.

> **PRONTA significa reconstruível e executável, não completamente planejada.**

---

# Auditoria não exige completude narrativa

Não são falhas por si só:

```text
não haver final decidido
não haver arco completo
não haver antagonista
não haver grande conflito inicial
não haver mundo detalhado
não haver ficha para toda pessoa que poderá aparecer
não haver módulos opcionais ativos
não saber futuras revelações
não saber como relações evoluirão
não saber quantos capítulos existirão
```

Se essas coisas não são necessárias para executar a abertura, podem continuar abertas.

```text
FUTURO ABERTO
≠ PREPARAÇÃO INCOMPLETA
```

---

# Fontes mínimas esperadas

Para uma história nova comum, a Auditoria espera encontrar:

```text
campanhas/<slug>/README.md
campanhas/<slug>/direcao.md
campanhas/<slug>/estado.md
fichas das personagens cuja reconstrução já é necessária
```

Outras fontes são condicionais:

```text
mundo/
→ somente se fatos externos estáveis precisarem persistir.

operacao.md
→ somente se existir operação transitória real.

arco.md
→ somente com Arco Preparado ativo e necessário.

oposicao.md
→ somente com Opositor ativo.

livro/
→ somente quando Livro estiver ativo e houver Ficção para registrar.
```

> **Ausência de arquivo opcional não é falha.**

---

# Bloco 1 — Identidade da obra

Verificar no `README.md`:

```text
nome reconhecível
STATUS atual
Premissa / Proposta curta
Estilo / Tom necessário
Personagens centrais já aprovadas
```

A Auditoria não exige uma sinopse completa.

Pergunta útil:

> **Uma IA nova consegue reconhecer que obra é esta e que experiência está tentando produzir?**

---

# Bloco 2 — Personagens reconstruíveis

Para cada personagem necessária à abertura, verificar:

```text
ficha existente
identidade reconhecível
Conceito suficiente
competências / conhecimentos relevantes sustentados
Traços, Poderes e meios relevantes com escopo suficiente
personalidade suficiente para uma Cadeira decidir
histórico suficiente para explicar o necessário
relações iniciais importantes preservadas
```

Não exigir ficha exaustiva.

```text
FICHA RECONSTRUÍVEL
→ suficiente.

FICHA SEM ALTURA, COMIDA FAVORITA OU BIOGRAFIA COMPLETA
→ não é falha por isso.
```

Se uma personagem incidental ainda não precisa de continuidade persistente, sua ausência de ficha não bloqueia o START.

---

# Bloco 3 — Autoridades

Verificar no `README.md`:

```text
Diretor
Narrador / Juiz
Personagem do Diretor, se houver
Cadeiras necessárias
Executor de cada autoridade
limites de delegação, quando existirem
```

A Auditoria deve conseguir responder:

> **Se surgir agora uma decisão voluntária de cada personagem central, quem pode tomá-la?**

Também conferir:

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE

MESMO EXECUTOR
≠ MESMA CADEIRA
```

Se a próxima autoria pertence ao Diretor, isso **não torna a obra não pronta**.

Significa apenas que o START apresentará o ponto aberto e aguardará o Diretor.

---

# Bloco 4 — Direção

Verificar `direcao.md` segundo `18-CRIACAO-DIRECAO.md`.

A Direção precisa preservar:

```text
Premissa
Estilo / Tom quando pertinente
fatos estruturais fechados
decisões persistentes já tomadas
decisões locais ainda ativas, se existirem
espaço que continua aberto
```

Não considerar falha:

```text
Direções Persistentes: nenhuma além das premissas.
Direções Ativas: nenhuma.
```

se o Diretor ainda não decidiu mais nada.

> **A Auditoria verifica decisões existentes; não exige novas decisões para preencher Direção.**

---

# Bloco 5 — Políticas operacionais

Verificar:

```text
Política de Mesa
Indicador operacional
Módulos ativos
```

Quando o Diretor não escolheu valores especiais, os padrões são válidos:

```text
MESA: SOB DEMANDA
INDICADOR OPERACIONAL: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real
```

Se o README ainda não registrou um padrão que deveria estar persistente, a IA pode fazer uma **correção mecânica segura** e registrar o padrão já definido pelo engine.

Isso não exige nova decisão autoral.

---

# Bloco 6 — Mundo necessário

Verificar o resultado de `20-CRIACAO-MUNDO-NECESSARIO.md`.

Duas condições são igualmente válidas:

```text
MUNDO NECESSÁRIO
→ fatos externos persistidos em mundo/.
```

ou:

```text
MUNDO NECESSÁRIO
→ NENHUM ANTES DO START.
```

A Auditoria não cria worldbuilding extra para tornar a obra “mais completa”.

Se a Premissa depende de um fato externo estrutural e nenhuma fonte o preserva, isso pode ser falha bloqueante.

---

# Bloco 7 — Estado inicial

Verificar `estado.md` segundo `21-CRIACAO-ESTADO-INICIAL.md`.

A IA precisa conseguir reconstruir:

```text
momento inicial, quando relevante
local inicial, quando relevante
presenças / posições necessárias
condições já existentes
último fato estabelecido
primeiro ponto aberto
```

Antes da primeira cena, é válido:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

O ponto aberto não pode pré-escrever uma vontade ainda pertencente a uma Cadeira ou ao Diretor.

```text
PONTO ABERTO IDENTIFICADO
→ correto.

DECISÃO ABERTA REGISTRADA COMO JÁ TOMADA
→ falha.
```

---

# Bloco 8 — Separação das fontes

Conferir se informações não foram parar na fonte errada.

```text
FICHA
→ quem a pessoa é.

README
→ configuração da obra e autoridades.

DIREÇÃO
→ decisões autorais ainda vinculantes.

MUNDO
→ fatos externos estáveis.

ESTADO
→ realidade ficcional presente.

OPERAÇÃO
→ processo fora da Ficção ainda pendente.

LIVRO
→ Ficção já acontecida, quando ativo.
```

Falhas típicas:

```text
proposta de Mesa registrada como fato no Estado
executor registrado como personalidade na ficha
resultado futuro colocado no Estado
segredo global tratado como conhecimento de personagem
rascunho de ficha tratado como ficha aprovada
```

---

# Falha bloqueante e observação não bloqueante

A Auditoria deve distinguir gravidade.

## BLOQUEANTE

Impede começar corretamente sem inventar, contradizer ou tomar autoria indevida.

Exemplos:

```text
personagem central necessária sem ficha suficiente
não está definido quem possui uma vontade que já precisa ser executada
Premissa e Estado inicial se contradizem materialmente
primeiro ponto aberto não pode ser identificado
fato estrutural indispensável não possui fonte
Estado já canonizou uma decisão que continua aberta
Mesa de criação relevante continua pendente
```

Resultado:

```text
AUDITORIA
→ BLOQUEADA
→ não executar START.
```

## NÃO BLOQUEANTE

Pode ser corrigido mecanicamente ou deixado para surgir depois.

Exemplos:

```text
campo opcional vazio
sem worldbuilding extra
sem ficha de figurante
sem arco futuro
sem antagonista
sem módulo opcional
nome de seção inconsistente mas significado inequívoco
padrão operacional ainda não copiado para README
```

Resultado:

```text
→ corrigir automaticamente quando for puramente mecânico e seguro;
OU
→ registrar como observação sem impedir START.
```

> **Não transformar preferência editorial em bloqueio operacional.**

---

# Correção automática segura

A Auditoria pode corrigir sem perguntar quando a mudança **não decide conteúdo autoral novo**.

Exemplos:

```text
registrar MESA: SOB DEMANDA quando nenhum valor especial foi escolhido;
registrar INDICADOR: SILENCIOSO quando nenhum valor especial foi escolhido;
corrigir referência de arquivo claramente quebrada;
normalizar cabeçalho ou rótulo sem mudar significado;
remover placeholder que deveria ter sido substituído por informação já aprovada;
```

Não corrigir silenciosamente:

```text
personalidade
motivação
relação
poder
passado
fato de mundo
trajetória futura
primeira decisão de personagem
```

se isso exigir escolha autoral.

```text
CORREÇÃO MECÂNICA
→ pode ser automática.

DECISÃO AUTORAL
→ pertence à autoridade adequada.
```

---

# Quando perguntar ao Diretor

Somente perguntar quando houver uma falha bloqueante cuja correção exija decisão que realmente pertence ao Diretor.

Exemplo:

```text
Estado diz que Ana e Bruno já são amigos.
Ficha / Premissa diz que começam como desconhecidos.
```

A IA não escolhe uma versão silenciosamente.

Ela apresenta a contradição de forma curta e pergunta qual deve prevalecer.

Não despejar uma lista de vinte verificações para o Diretor confirmar.

> **A Auditoria trabalha sozinha até encontrar uma decisão que não pode legitimamente tomar.**

---

# Operação pendente

Se a Auditoria encontrar uma Mesa, Auditoria anterior ou criação ainda pendente que precisa ser resolvida antes da Ficção:

```text
operacao.md
→ preservar o estado operacional.
```

Nesse caso:

```text
STATUS da preparação
→ continua EM PREPARAÇÃO.

START
→ não executar ainda.
```

Depois da resolução, rodar novamente apenas as verificações afetadas.

---

# Resultado da Auditoria

Usar conceitualmente:

```text
AUDITORIA: APROVADA
AUDITORIA: BLOQUEADA
```

## APROVADA

Significa:

```text
fontes suficientes
+
sem contradição bloqueante conhecida
+
autoridades reconstruíveis
+
primeiro ponto aberto identificável
+
nenhuma decisão necessária foi tomada pela autoridade errada
```

Então atualizar no `README.md`:

```text
STATUS
→ PRONTA
```

E seguir para `START`.

## BLOQUEADA

Significa que existe pelo menos uma falha que impede execução correta.

A IA deve informar somente:

```text
o bloqueio real
por que ele impede o START
o que precisa ser decidido ou corrigido
```

Não usar a Auditoria para reabrir decisões já aprovadas.

---

# Forma recomendada de resposta

Quando tudo estiver correto:

```text
Auditoria concluída. A obra está reconstruível e o primeiro ponto aberto está claro.
STATUS → PRONTA.
```

Não é necessário mostrar todo o checklist salvo se o Diretor pedir.

Quando houver bloqueio:

```text
A preparação tem um bloqueio: o Estado inicial coloca Ana e Bruno como desconhecidos, mas a ficha de Ana registra Bruno como amigo de infância. Preciso saber qual versão deve prevalecer antes do START.
```

---

# Critério de conclusão

Antes de aprovar, a IA deve conseguir responder internamente:

```text
[ ] uma nova IA reconhece a obra pelo README?
[ ] as personagens necessárias são reconstruíveis?
[ ] cada vontade necessária possui autoridade e executor definidos?
[ ] Direção preserva somente o que realmente foi fechado?
[ ] políticas operacionais estão definidas ou usam padrões válidos?
[ ] mundo necessário está preservado ou legitimamente não é necessário?
[ ] Estado inicial representa realidade, não roteiro?
[ ] primeiro ponto aberto está claro?
[ ] sabemos quem possui a próxima autoria?
[ ] nenhuma proposta pendente contaminou a Ficção?
[ ] não existe contradição bloqueante conhecida entre as fontes?
```

Se sim:

```text
AUDITORIA: APROVADA
STATUS: PRONTA
→ próxima etapa: START
```

---

# Regra final

> **A Auditoria de Preparação não exige uma história planejada; exige uma história reconstruível. Ela verifica se as fontes permitem começar sem inventar fatos necessários, misturar autoridades ou canonizar decisões ainda abertas. Corrige sozinha o que for puramente mecânico, devolve ao Diretor apenas bloqueios autorais reais e, quando tudo estiver suficiente, marca a obra como PRONTA para o START.**