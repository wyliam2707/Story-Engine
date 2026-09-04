# 22 — Criação: Auditoria de Preparação

Este arquivo define a **décima primeira etapa autoral** do ramo `NOVA HISTÓRIA`.

Ele entra em uso depois que o Estado inicial está suficiente em `21-CRIACAO-ESTADO-INICIAL.md`.

> **Auditar é verificar se outra IA conseguiria iniciar corretamente a obra usando somente as fontes persistentes.**

A Auditoria não cria história, não planeja o futuro e não substitui decisões do Diretor.

---

# Critério central

A obra está pronta quando uma nova IA consegue reconstruir:

```text
qual história está sendo criada
como deve ser apresentada
quem são as personagens necessárias
quem possui cada autoria
quem executa o Narrador
como a Mesa opera
que pontos o Diretor já fechou
o que permanece aberto
qual é a realidade inicial
qual é o primeiro ponto aberto
quem possui a próxima autoria
```

sem depender da conversa original.

> **PRONTA significa reconstruível e executável, não completamente planejada.**

---

# A Auditoria também verifica a arquitetura atual

Uma obra nova não deve depender de:

```text
JUIZ permanente
SENTENÇA causal do Narrador
RNG invisível
teste universal
dificuldade universal
probabilidade escondida para decidir resultado material
```

Se um workspace antigo usa o rótulo:

```text
NARRADOR / JUIZ
```

mas o significado restante está claro, isso é **legado mecânico**, não decisão autoral.

A Auditoria pode normalizar para:

```text
NARRADOR
```

sem perguntar.

> **Rótulo antigo não reativa função removida do engine.**

---

# Auditoria não exige completude narrativa

Não são falhas por si só:

```text
não haver final
não haver arco completo
não haver antagonista
não haver conflito inicial
não haver mundo detalhado
não haver ficha de figurantes
não haver módulos opcionais ativos
não saber futuras revelações
não saber como relações evoluirão
não saber quantos capítulos existirão
```

```text
FUTURO ABERTO
≠ PREPARAÇÃO INCOMPLETA
```

---

# Fontes mínimas comuns

```text
campanhas/<slug>/README.md
campanhas/<slug>/direcao.md
campanhas/<slug>/estado.md
fichas das personagens cuja reconstrução já é necessária
```

Condicionais:

```text
mundo/
→ somente se houver fatos externos estáveis necessários.

operacao.md
→ somente se existir operação transitória real.

arco.md
→ somente com Arco Preparado ativo.

oposicao.md
→ somente com Opositor ativo.

livro/
→ somente quando Livro estiver ativo e houver Ficção a registrar.
```

> **Ausência de arquivo opcional não é falha.**

---

# 1 — Identidade da obra

Verificar no `README.md`:

```text
nome reconhecível
STATUS
Premissa / Proposta curta
Estilo / Tom necessário
Personagens centrais aprovadas
```

Pergunta:

> **Uma IA nova reconhece que obra é esta e que experiência ela pretende produzir?**

---

# 2 — Personagens reconstruíveis

Para cada personagem necessária à abertura:

```text
ficha existente
identidade reconhecível
Conceito suficiente
competências / conhecimentos relevantes
Traços, Poderes e meios relevantes
personalidade suficiente para uma Cadeira decidir
histórico suficiente para explicar o necessário
relações iniciais importantes
```

```text
FICHA RECONSTRUÍVEL
→ suficiente.

FICHA EXAUSTIVA
→ não é exigida.
```

---

# 3 — Autoridades e funções

Verificar no `README.md`:

```text
Diretor
Narrador
Personagem do Diretor, se houver
Cadeiras necessárias
Executor de cada Cadeira
limites de delegação, quando existirem
```

A Auditoria deve conseguir responder:

> **Se cada personagem central precisar decidir agora, quem possui essa vontade?**

E também:

> **Se um resultado material permanecer aberto, o sistema sabe que deve usar a Mesa em vez de atribuir sentença ao Narrador?**

Conferir:

```text
DELEGAR EXECUÇÃO
≠ TRANSFERIR VONTADE

MESMO EXECUTOR
≠ MESMA CADEIRA

NARRADOR
≠ JUIZ
```

Se a próxima autoria pertence ao Diretor, a obra ainda pode estar pronta. O START apenas aguardará a decisão correta.

---

# 4 — Direção

Verificar `direcao.md` segundo `18-CRIACAO-DIRECAO.md`.

A Direção precisa preservar somente:

```text
Premissa
Estilo/Tom quando pertinente
fatos estruturais fechados
decisões persistentes realmente tomadas
decisões locais ainda ativas
espaço aberto
```

É válido:

```text
Direções Persistentes
→ nenhuma além das premissas.

Direções Ativas
→ nenhuma.
```

> **Auditoria verifica decisões existentes; não exige decisões novas.**

---

# 5 — Políticas operacionais

Verificar:

```text
Política de Mesa
Indicador operacional
Módulos ativos
```

Padrões válidos:

```text
MESA: SOB DEMANDA
INDICADOR OPERACIONAL: SILENCIOSO
MÓDULOS: INATIVOS salvo escolha ou necessidade real
```

Se um padrão já é definido pelo engine mas ainda não foi copiado ao README, pode ser registrado como correção mecânica segura.

---

# 6 — Mundo necessário

Duas condições são válidas:

```text
MUNDO NECESSÁRIO
→ fatos externos persistidos em mundo/.
```

ou:

```text
MUNDO NECESSÁRIO
→ NENHUM ANTES DO START.
```

Não criar worldbuilding extra para satisfazer checklist.

Se a Premissa depende de fato estrutural sem fonte, isso pode ser bloqueante.

---

# 7 — Estado inicial

Verificar `estado.md` segundo `21-CRIACAO-ESTADO-INICIAL.md`.

Reconstruir, quando pertinente:

```text
momento
local
presenças / posições
condições existentes
último fato estabelecido
primeiro ponto aberto
```

Antes da primeira cena, é válido:

```text
Último fato estabelecido
→ história ainda não iniciada.
```

O Estado não pode pré-escrever vontade ainda aberta.

```text
PONTO ABERTO IDENTIFICADO
→ correto.

DECISÃO ABERTA REGISTRADA COMO TOMADA
→ falha.
```

---

# 8 — Separação das fontes

```text
FICHA
→ quem a pessoa é.

README
→ configuração da obra e executores.

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
proposta de Mesa no Estado
executor dentro da personalidade da ficha
resultado futuro colocado no Estado
segredo global tratado como conhecimento da personagem
rascunho tratado como ficha aprovada
Juiz legado tratado como autoridade atual
```

---

# Bloqueante e não bloqueante

## BLOQUEANTE

Impede começar corretamente sem inventar, contradizer ou tomar autoria indevida.

Exemplos:

```text
personagem central necessária sem ficha suficiente
não se sabe quem possui uma vontade necessária
Premissa e Estado se contradizem materialmente
primeiro ponto aberto não pode ser identificado
fato estrutural indispensável não possui fonte
Estado canonizou decisão ainda aberta
Mesa relevante continua pendente
o fluxo depende de um Juiz para decidir resultado material
```

```text
AUDITORIA: BLOQUEADA
→ não executar START.
```

## NÃO BLOQUEANTE

Exemplos:

```text
campo opcional vazio
sem worldbuilding extra
sem ficha de figurante
sem arco futuro
sem antagonista
sem módulo opcional
rótulo antigo com significado inequívoco
padrão operacional ainda não copiado ao README
```

```text
→ corrigir mecanicamente quando seguro
OU
→ deixar como observação.
```

> **Não transformar preferência editorial em bloqueio operacional.**

---

# Correção automática segura

Pode corrigir sem perguntar quando não cria decisão autoral nova:

```text
registrar MESA: SOB DEMANDA como padrão
registrar INDICADOR: SILENCIOSO como padrão
normalizar NARRADOR / JUIZ → NARRADOR
corrigir referência de arquivo claramente quebrada
normalizar cabeçalho
remover placeholder substituível por informação já aprovada
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
resultado importante
primeira decisão de personagem
```

```text
CORREÇÃO MECÂNICA
→ pode ser automática.

DECISÃO AUTORAL
→ pertence à autoridade adequada.
```

---

# Quando perguntar ao Diretor

Somente quando houver bloqueio cuja correção exija decisão autoral real.

Exemplo:

```text
Estado
→ Ana e Bruno já são amigos.

Premissa
→ começam como desconhecidos.
```

A IA apresenta a contradição e pergunta qual versão prevalece.

Não despejar o checklist inteiro para confirmação.

> **A Auditoria trabalha sozinha até encontrar uma decisão que não pode legitimamente tomar.**

---

# Operação pendente

Se existir Mesa, Auditoria anterior ou criação ainda pendente:

```text
operacao.md
→ preserva o estado operacional.

STATUS
→ continua EM PREPARAÇÃO.

START
→ não executar ainda.
```

Depois da resolução, revisar apenas verificações afetadas.

---

# Resultado

```text
AUDITORIA: APROVADA
AUDITORIA: BLOQUEADA
```

## APROVADA

```text
fontes suficientes
+
sem contradição bloqueante conhecida
+
autorias reconstruíveis
+
Narrador corretamente configurado sem poder de Juiz
+
primeiro ponto aberto identificável
```

Então:

```text
STATUS
→ PRONTA
```

## BLOQUEADA

Informar apenas:

```text
o bloqueio real
por que impede START
o que precisa ser decidido ou corrigido
```

Não reabrir decisões já aprovadas.

---

# Forma recomendada de resposta

Quando aprovada:

```text
Auditoria concluída. A obra está reconstruível e o primeiro ponto aberto está claro.
STATUS → PRONTA.
```

Quando bloqueada, apresentar apenas o problema concreto.

---

# Critério de conclusão

```text
[ ] README reconhece a obra?
[ ] personagens necessárias são reconstruíveis?
[ ] cada vontade possui autoridade e executor?
[ ] Narrador está configurado sem função de Juiz?
[ ] Direção preserva só o que foi fechado?
[ ] políticas estão definidas ou usam padrões?
[ ] mundo necessário está preservado ou legitimamente dispensado?
[ ] Estado representa realidade, não roteiro?
[ ] primeiro ponto aberto está claro?
[ ] sabemos quem possui a próxima autoria?
[ ] resultado material aberto irá à Mesa em vez de sentença escondida?
[ ] nenhuma proposta pendente contaminou a Ficção?
[ ] não há contradição bloqueante conhecida?
```

Se sim:

```text
AUDITORIA: APROVADA
STATUS: PRONTA
→ START
```

---

# Regra final

> **A Auditoria exige uma história reconstruível, não uma história planejada. Ela confirma também que o W4D atual está sendo usado: sem Juiz permanente, sem sentença causal escondida e sem RNG universal. Resultados materiais abertos continuam sendo questões de autoria e podem voltar à Mesa.**