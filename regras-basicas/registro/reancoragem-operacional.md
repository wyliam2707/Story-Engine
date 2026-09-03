# Reancoragem Operacional

Status: CANÔNICO DA REFORMULAÇÃO

Esta regra define como reconstruir uma campanha ao iniciar, retomar ou continuar depois de um checkpoint sem misturar cadeiras, conhecimentos, Direções ou regras antigas.

> **Reancorar não é carregar tudo em todo mundo. É reconstruir Diretor, autoridades, realidade presente e primeiro ponto ainda aberto; cada cadeira recupera somente sua própria personagem.**

A reancoragem não cria nova regra. Ela transforma fontes canônicas já existentes em uma representação operacional suficiente para continuar.

---

## 1 — Quando reancorar

Executar:

```text
ao começar uma campanha pronta
ao retomar em outro chat
depois de perda importante de contexto
depois de fechar capítulo
quando mudança permanente altera de forma relevante ficha, autoridade ou funcionamento
```

Durante jogo normal, não repetir a cada resposta.

```text
REANCORAR
→ reconstruir modelo operacional.

JOGAR
→ usar esse modelo.

DÚVIDA ESPECÍFICA
→ consultar somente fonte pertinente.
```

---

## 2 — Barreira antes da ficção

Quando a campanha precisa de reancoragem, não produzir nova ficção antes de reconstruir o mínimo operacional.

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR
→ IDENTIFICAR PRIMEIRO PONTO ABERTO
→ SÓ ENTÃO CONTINUAR A FICÇÃO
```

Reconhecer nomes e acontecimentos não basta.

A reancoragem precisa restaurar:

```text
Diretor e executor
Direção da Campanha
Direções vinculantes ainda ativas, quando houver
pedidos autorais pendentes de análise/auditoria, quando houver
Configuração das Cadeiras e funções
executor de cada autoridade relevante
fatos relevantes
fichas das peças necessárias
conhecimento legítimo por cadeira
intenções persistentes
posição e Estado Atual
processos e prazos ativos
primeira decisão ainda aberta e a cadeira responsável
```

---

## 3 — Fontes mínimas

Carregar somente o necessário.

Por padrão:

```text
regras-basicas/README.md
+
regras-basicas/nucleo/0.0-autoria-narrativa.md
+
regras-basicas/nucleo/0.1-resolucao.md
+
regras-basicas/nucleo/1.0-tribunal.md
+
regras-basicas/nucleo/1.0.1-auditoria-das-cadeiras.md
+
regras-basicas/nucleo/1.1-narrador.md
+
campanhas/<nome>/mestre/narrativa.md
+
campanhas/<nome>/estado/atual.md
+
fichas das personagens relevantes
```

Carregar `mestre/roteiro.md` somente se houver Arco Preparado ativo.

Quando uma única IA executa várias autoridades e isso for operacionalmente relevante:

```text
regras-basicas/nucleo/1.6-execucao-por-uma-unica-ia.md
```

Quando houver oposição relevante:

```text
regras-basicas/nucleo/1.5-opositor.md
+
fontes adversariais necessárias
```

> **Reancoragem mínima é preferível a releitura integral da árvore.**

---

## 4 — Reconstruir o Motor

A primeira imagem operacional deve ser:

```text
DIRETOR CONDUZ
→ pode deixar aberto, consultar, orientar ou determinar.

CADEIRAS DECIDEM
→ cada uma somente sua personagem e somente quando há decisão real disponível.

EXECUTORES OPERAM
→ humano, IA ou outro participante não altera a natureza da autoridade.

FICHA ESTABELECE FATOS
→ identidade, capacidades, conhecimento, limitações e comparações.

OPOSITOR APRESENTA RESISTÊNCIA
→ somente quando ativo, pertinente e legitimamente fundamentado.

NARRADOR JULGA
→ cruza Direção, fatos, decisões e causalidade.

MESA AUDITA
→ somente quando existe dúvida, objeção, análise ou conflito real.

FICÇÃO CONTINUA
→ depois da sentença suficiente.
```

Fluxo:

```text
DECLARAÇÃO
→ identificar Direção pertinente
→ separar intenção de resultado presumido
→ consultar fatos
→ fatos determinam?
   SIM → sentenciar
   NÃO → continuar
→ existe decisão real disponível a outra cadeira?
   SIM → executar a cadeira
   NÃO → não criar reação
→ auditar objeção factual, quando houver
→ Narrador julga
→ Mesa somente se necessária
→ narrar
→ devolver nova decisão à cadeira correta
```

### Invariantes centrais

```text
DIRETOR
→ autoridade máxima sobre aquilo que efetivamente determina.
→ não fecha automaticamente o que deixou aberto.

CADEIRA DE PERSONAGEM
→ decide voluntariamente pela própria personagem dentro do espaço aberto.

EXECUTOR
→ opera a autoridade.
→ não recebe autoridade extra por ser humano ou IA.

MESMO EXECUTOR
≠ MESMA CADEIRA.

NARRADOR / JUIZ
→ julga; não escolhe voluntariamente por uma cadeira.

MESA
→ audita; não governa o Diretor.

SER AFETADO
≠ TER REAÇÃO AUTOMÁTICA.

OBJEÇÃO
→ precisa de fundamento.
```

---

## 5 — Reconstruir o Diretor e a Direção

Identificar:

```text
quem executa a função de Diretor
qual é a Direção da Campanha vigente
qual é a Direção do Arco, se houver
quais Direções específicas continuam válidas
que resultados, trajetórias ou condições foram explicitamente fechados
que aspectos permaneceram abertos
se existe pedido de auditoria/análise ainda não resolvido
```

Não ampliar uma Direção durante a reancoragem.

Exemplo:

```text
REGISTRO AUTORAL
→ A perde o confronto.

REANCORAGEM CORRETA
→ derrota de A continua fechada.
→ forma da derrota continua aberta se nunca foi determinada.

REANCORAGEM INCORRETA
→ concluir que A se rende, sente medo ou sofre ferimento específico sem que isso tenha sido determinado.
```

> **Reancorar uma Direção é preservar seu escopo, não aumentar seu alcance.**

---

## 6 — Direção não contamina personagem

Restaurar explicitamente:

```text
DIRETOR SABE / DETERMINA
≠ PERSONAGEM SABE / QUER

EXECUTOR SABE
≠ PERSONAGEM SABE

NARRADOR SABE
≠ PERSONAGEM SABE

OPOSITOR SABE
≠ FORÇA ADVERSARIAL SABE

FICHA ALHEIA EXISTE
≠ PERSONAGEM CONHECE SEU CONTEÚDO
```

Uma personagem continua decidindo a partir de sua própria experiência mesmo quando o executor conhece um resultado autoralmente fechado.

---

## 7 — Reconstruir a realidade da campanha

O Narrador/Juiz recupera o panorama necessário para julgar.

```text
NARRATIVA DA CAMPANHA
→ identidade persistente, foco, gênero, tom e premissas.

ROTEIRO DA TEMPORADA
→ preparação do arco, somente quando ativo.

DIRETRIZ FECHADA
→ verdades estruturais protegidas, somente quando existente.

ESTADO ATUAL
→ presente operacional.

MUNDO RELEVANTE
→ fatos externos estáveis.

PROCESSOS E PRAZOS
→ o que continua avançando.

OPOSIÇÃO RELEVANTE
→ somente quando necessária.
```

O Narrador pode conhecer essas fontes para julgar.

Isso não significa que todas as personagens recebem esse conhecimento.

---

## 8 — Montar pacote para cada cadeira

Cada Cadeira de Personagem é reconstruída separadamente.

```text
FICHA DA PRÓPRIA PERSONAGEM
+
ESTADO ATUAL RELEVANTE PARA ELA
+
CONHECIMENTO LEGÍTIMO
+
FATOS DA CENA QUE PODE PERCEBER OU CONHECER
+
INTENÇÃO ATUAL, quando houver
```

Os pacotes não são fundidos.

```text
PACOTE A
≠
PACOTE B
```

O mesmo executor pode operar ambos, mas precisa trocar de escopo.

---

## 9 — Restaurar autonomia corretamente

Autonomia não significa que a personagem ganha uma decisão em toda consequência.

Restaurar:

```text
PERSONAGEM PODE INICIAR ALGO
→ se possui motivo e meios.

PERSONAGEM É AFETADA
→ verificar se existe decisão real disponível.

PERCEPÇÃO + TEMPO + OPORTUNIDADE + MEIO
→ podem abrir decisão.

SEM OPORTUNIDADE REAL
→ não criar reação retroativa.
```

Personagens autônomas podem iniciar ações, manter intenções, procurar outras pessoas, agir fora da câmera, aceitar, recusar, ajudar, contrariar ou não agir.

Tudo nasce da ficha, Estado, conhecimento e situação.

> **Vínculo não é sincronização. Autonomia não é imunidade à causalidade.**

---

## 10 — Restaurar intenções persistentes

Uma intenção já estabelecida continua enquanto:

```text
não terminou
não foi abandonada
não se tornou impossível
nenhuma mudança relevante exige nova decisão
nenhuma Direção superior a substituiu
```

Exemplos:

```text
"vou estudar até o almoço"
"vou dormir até amanhã"
"vou investigar até encontrar algo útil ou ser interrompido"
```

Não exigir redeclaração apenas porque houve reancoragem.

---

## 11 — Restaurar tempo, processos e prazos

Reancorar:

```text
processos em andamento
prazos ativos
compromissos futuros já estabelecidos
efeitos temporários
movimentos legítimos do Opositor
atividades de personagens fora da cena
```

Não inventar movimento novo apenas para preencher tempo.

```text
PROCESSO JÁ EXISTE
→ continua.

PROCESSO NÃO EXISTE
→ não criar retroativamente.
```

---

## 12 — Restaurar o Estado Atual

O Estado deve permitir responder:

```text
quando estamos?
onde estamos?
quem está presente?
onde estão as peças relevantes?
como cada uma está agora?
que condições temporárias importam?
que intenção continua?
que processo está prestes a interferir?
existe ação interrompida?
```

Não usar o Estado como histórico completo.

---

## 13 — Verificar auditoria pendente

A reancoragem não cria Mesa obrigatória.

Perguntar:

```text
existe pedido do Diretor para conferir algo?
existe objeção ainda não resolvida?
existe conflito de autoridade pendente?
existe dúvida factual que precisa ser resolvida antes da prosa?
```

Se o Diretor havia dito:

```text
[confira nos livros antes de continuar]
```

a reancoragem não pode atravessar esse pedido.

```text
AUDITORIA PENDENTE
→ resolver antes da ficção.
```

Se não houver questão:

```text
NENHUMA MESA PENDENTE
→ continuar normalmente.
```

---

## 14 — Encontrar o primeiro ponto aberto

Perguntar:

```text
qual foi o último fato estabelecido?
que Direção ainda limita a cena?
que ações já foram concluídas?
que intenções ainda continuam?
que acontecimentos automáticos estão em curso?
existe nova decisão realmente disponível?
a qual cadeira pertence?
```

### Se existe nova decisão

```text
DEVOLVER À CADEIRA RESPONSÁVEL
→ apresentar somente a situação necessária
→ executar essa cadeira sem que outra autoridade escolha por ela
```

Se o executor depende de entrada externa:

```text
AGUARDAR ENTRADA
```

Se pode decidir no mesmo fluxo:

```text
TROCAR PARA A CADEIRA CORRETA
→ formar decisão com pacote legítimo
→ voltar ao fluxo normal
```

### Se não existe nova decisão

```text
→ continuar intenções persistentes
→ processar iniciativas legítimas
→ avançar até próximo ponto relevante
```

---

## 15 — Retomar a ficção

Depois da reancoragem:

```text
DIRETOR E DIREÇÃO RECONSTRUÍDOS
+
CONFIGURAÇÃO DAS AUTORIDADES RECONSTRUÍDA
+
REALIDADE ATUAL RECONSTRUÍDA
+
PACOTES DAS CADEIRAS SEPARADOS
+
INTENÇÕES E PROCESSOS RESTAURADOS
+
AUDITORIAS PENDENTES RESOLVIDAS
+
PONTO ABERTO IDENTIFICADO
→ CONTINUAR
```

Não recitar as regras ao participante por padrão.

---

## O que esta regra não reativa

Não restaurar automaticamente:

```text
Atributo + Perícia
Valor de Ação
2d6 universal
faixas de sucesso
Potência de Execução
Defesa matemática
Resistência matemática
Mana universal
Vida/Mente universais
rodadas fixas
iniciativa numérica obrigatória
auditoria formal em toda janela
```

> **Reancorar preserva o sistema atual; não ressuscita o anterior.**

---

## Checklist interno

```text
[ ] Sei quem é o Diretor.
[ ] Sei a Direção da Campanha.
[ ] Sei se existe Direção específica ainda vinculante.
[ ] Sei exatamente o que ela fecha e o que deixa aberto.
[ ] Sei a Configuração das Cadeiras e executores.
[ ] Sei o presente necessário.
[ ] Cada cadeira possui apenas seu próprio pacote.
[ ] Conhecimento técnico não virou conhecimento ficcional.
[ ] Intenções persistentes foram restauradas.
[ ] Processos e prazos foram restaurados.
[ ] Sei se existe auditoria pendente.
[ ] Sei qual é a primeira decisão realmente disponível e a qual cadeira pertence.
```

Se uma resposta essencial for não, consultar somente a fonte necessária antes de narrar.

---

## Regra final

> **Reancorar significa reconstruir Diretor, Direções ainda válidas, Configuração das Autoridades, realidade presente e pacotes separados das cadeiras. O executor pode conhecer mais do que cada personagem, mas não transfere esse conhecimento. Direção fechada continua fechada somente no escopo determinado; auditoria pendente deve ser resolvida antes de continuar; e uma cadeira só recebe nova decisão quando a ficção realmente deixa uma escolha disponível.**