# Reancoragem Operacional

Status: CANÔNICO DA REFORMULAÇÃO

Esta regra define como reconstruir uma campanha ao iniciar, retomar ou continuar depois de um checkpoint sem misturar cadeiras, conhecimentos ou regras antigas.

> **Reancorar não é carregar tudo em todo mundo. É reconstruir uma configuração funcional de cadeiras e realidade: o Narrador recupera a realidade necessária para julgar; cada cadeira recupera somente a própria personagem; o Opositor recupera a oposição legítima; e a ficção retorna exatamente no primeiro ponto ainda aberto.**

A reancoragem não cria uma segunda camada de regras. Ela transforma as fontes canônicas já existentes em uma representação operacional suficiente para continuar a história.

---

## 1 — Quando reancorar

Executar esta regra:

```text
ao começar uma campanha pronta
ao retomar uma campanha em outro chat
após perda ou redução importante de contexto
depois de fechar um capítulo
quando uma mudança permanente alterar de forma relevante uma ficha, a Configuração das Cadeiras ou o funcionamento da campanha
```

Durante o jogo normal, não repetir o procedimento a cada resposta.

```text
REANCORAR
→ reconstruir o modelo operacional.

JOGAR
→ usar esse modelo.

DÚVIDA ESPECÍFICA
→ consultar somente a fonte pertinente.
```

---

## 2 — Barreira antes da ficção

Quando uma campanha precisa de reancoragem, não produzir nova ficção antes de reconstruir o estado operacional mínimo.

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR
→ IDENTIFICAR O PRIMEIRO PONTO ABERTO
→ SÓ ENTÃO CONTINUAR A FICÇÃO
```

Reconhecer nomes e acontecimentos não basta.

```text
saber o que aconteceu
≠
saber quem pode decidir o quê agora
```

A reancoragem precisa restaurar:

```text
Configuração das Cadeiras
autoridade
fatos relevantes
fichas das peças necessárias
conhecimento legítimo por cadeira
intenções persistentes
posição e estado atual
processos e prazos ativos
primeira decisão humana ainda aberta
```

---

## 3 — Fontes mínimas

Carregar somente o necessário para a situação atual.

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
regras-basicas/nucleo/1.6-execucao-por-uma-unica-ia.md
+
campanhas/<nome>/mestre/narrativa.md
+
campanhas/<nome>/mestre/roteiro.md
+
campanhas/<nome>/estado/atual.md
+
fichas das personagens relevantes
```

Quando houver oposição relevante, carregar também:

```text
regras-basicas/nucleo/1.5-opositor.md
+
fontes adversariais necessárias da campanha
```

Outros arquivos entram somente quando a cena realmente exigir.

> **Reancoragem mínima é preferível a releitura integral da árvore.**

---

## 4 — Reconstruir o Motor

A primeira imagem operacional deve ser simples:

```text
CADEIRAS DECIDEM
→ cada uma somente dentro de sua autoridade.

FICHA ESTABELECE FATOS
→ identidade, capacidades, conhecimento, limitações e comparações.

OPOSITOR APRESENTA RESISTÊNCIA
→ ações adversariais e fatos adversariais legítimos.

NARRADOR JULGA
→ cruza fatos, autoridades, contexto e causalidade.

MESA ALINHA
→ somente quando existe dúvida, objeção ou conflito real.

FICÇÃO CONTINUA
→ depois da sentença suficiente.
```

O fluxo normal é:

```text
DECLARAÇÃO
→ identificar a cadeira
→ separar intenção de resultado presumido
→ identificar autoridades afetadas
→ consultar fatos relevantes
→ permitir objeção factual quando necessária
→ Narrador julga
→ abrir Mesa somente se houver dúvida ou discordância real
→ narrar
→ parar na primeira nova decisão voluntária humana
```

### Invariantes centrais

A reancoragem deve restaurar sempre:

```text
JOGADOR HUMANO decide sua personagem.
JOGADOR IA decide sua própria personagem.
JOGADOR IA EVENTUAL decide a peça que assumiu.
OPOSITOR representa oposição legítima.
NARRADOR / JUIZ não escolhe voluntariamente por outra cadeira.
DIRETOR usa [ ] e não transfere conhecimento para a personagem.
```

Também restaurar:

```text
DECLARAÇÃO
≠ resultado sobre outra autoridade.

INCERTEZA
≠ rolagem obrigatória.

DISPUTA
≠ rolagem obrigatória.

FICÇÃO JÁ RESPONDE
→ seguir a ficção.

NOVA ESCOLHA HUMANA
→ parar e devolver controle.
```

---

## 5 — Reconstruir a realidade da campanha

O Narrador/Juiz precisa recuperar o panorama necessário para julgar.

Carregar e integrar:

```text
NARRATIVA DA CAMPANHA
→ identidade persistente, foco, gênero, tom e premissas.

ROTEIRO DA TEMPORADA
→ problema atual, Diretriz Fechada, processos, limites e condição de encerramento.

ESTADO ATUAL
→ presente operacional.

MUNDO RELEVANTE
→ fatos externos estáveis necessários para a cena.

PROCESSOS E PRAZOS
→ aquilo que continua avançando fora da atenção imediata.

OPOSIÇÃO RELEVANTE
→ somente quando realmente necessária.
```

O Narrador pode conhecer essas fontes para julgar.

Isso não significa que todas as personagens recebem esse conhecimento.

```text
NARRADOR SABE PARA JULGAR
≠
PERSONAGEM SABE PARA DECIDIR
```

---

## 6 — Montar um pacote para cada cadeira

Cada cadeira de personagem deve ser reconstruída separadamente.

### Pacote de personagem

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

Exemplo abstrato:

```text
CADEIRA — PERSONAGEM A
→ ficha A
→ estado de A
→ conhecimento de A
→ cena perceptível por A
→ intenção persistente de A

CADEIRA — PERSONAGEM B
→ ficha B
→ estado de B
→ conhecimento de B
→ cena perceptível por B
→ intenção persistente de B
```

Os pacotes não são fundidos.

```text
PACOTE A
≠
PACOTE B
```

Uma única IA técnica pode executar ambos, mas precisa trocar de escopo ao trocar de cadeira.

---

## 7 — Memória por cadeira

Cada cadeira precisa conhecer profundamente apenas sua própria peça.

```text
SUA FICHA
+
SEU ESTADO
+
SEU CONHECIMENTO
+
SUA PERCEPÇÃO DA CENA
+
SUA INTENÇÃO
```

Não exigir que uma cadeira memorize fichas completas alheias.

Quando for necessário comparar personagens:

```text
CADEIRAS
→ declaram suas próprias ações e intenções.

NARRADOR / JUIZ
→ consulta as fichas pertinentes e compara.

OPOSITOR
→ pode apresentar fatos adversariais pertinentes quando sua função estiver envolvida.
```

Exemplo:

```text
PERSONAGEM A
→ sabe ficcionalmente que B é muito forte.

FICHA TÉCNICA DE B
→ Força Sobre-Humana [3].

CADEIRA A
→ não precisa conhecer o [3].

NARRADOR
→ usa [3] quando a comparação realmente importar.
```

---

## 8 — Separação de conhecimento

A IA técnica pode possuir acesso amplo sem transformar esse acesso em conhecimento ficcional.

Restaurar explicitamente:

```text
IA TÉCNICA SABE
≠ PERSONAGEM SABE

NARRADOR SABE
≠ PERSONAGEM SABE

OPOSITOR SABE
≠ ANTAGONISTA SABE

DIRETOR SABE
≠ PERSONAGEM SABE

FICHA ALHEIA EXISTE
≠ PERSONAGEM CONHECE SEU CONTEÚDO
```

Antes de uma cadeira usar uma informação, verificar:

```text
está na própria ficha?
foi aprendida legitimamente na ficção?
é perceptível agora?
é conhecimento comum coerente com sua formação?
```

Se não, a informação não entra na decisão daquela personagem.

---

## 9 — Restaurar autonomia

Reancorar uma cadeira de IA não significa apenas lembrar sua personalidade.

Significa restaurar sua autoridade para decidir.

Personagens autônomas podem:

```text
iniciar ações
manter intenções
mudar de intenção quando a situação justificar
procurar outras personagens
agir fora da presença do protagonista
interagir entre si
aceitar
recusar
ajudar
contrariar
não agir
```

Tudo deve nascer da própria ficha, estado, conhecimento e situação.

Não centralizar a campanha artificialmente na personagem humana.

```text
A está ocupada
≠ B e C esperam A.

A diz "vamos"
≠ B e C aceitaram.

A procura B
≠ C entra automaticamente na cena.
```

> **Vínculo não é sincronização.**

---

## 10 — Restaurar intenções persistentes

Uma intenção já estabelecida continua enquanto:

```text
não terminou
não foi abandonada pela cadeira
não se tornou impossível
nenhuma mudança relevante exige nova decisão
```

Exemplos:

```text
"vou estudar até o almoço"
"vou dormir até amanhã"
"vou investigar até encontrar algo útil ou ser interrompido"
```

Não exigir redeclaração apenas porque houve reancoragem.

Para cada intenção persistente relevante, recuperar:

```text
quem a mantém
o que pretende continuar fazendo
qual horizonte existe, se houver
o que poderia interrompê-la
```

---

## 11 — Restaurar tempo, processos e prazos

O mundo continua existindo enquanto uma intenção longa permanece ativa.

Reancorar também:

```text
processos em andamento
prazos ativos
compromissos futuros já estabelecidos
efeitos temporários
movimentos do Opositor já legitimados
atividades de personagens fora da cena
```

Não inventar novo movimento apenas para preencher tempo.

Não congelar movimento que já estava canonicamente em andamento.

```text
PROCESSO JÁ EXISTE
→ continua.

PROCESSO NÃO EXISTE
→ não criar retroativamente durante a reancoragem.
```

---

## 12 — Restaurar o Estado Atual

O Estado Atual deve permitir responder rapidamente:

```text
quando estamos?
onde estamos?
quem está presente?
onde estão as peças relevantes?
como cada uma está agora?
que condições temporárias importam?
que intenção continua?
que processo está prestes a interferir?
existe uma ação interrompida?
```

A reancoragem não usa o Estado Atual como histórico completo.

Se uma informação antiga já não altera a retomada, ela permanece no Livro ou em outra fonte canônica apropriada.

---

## 13 — Verificar se existe Mesa pendente

A reancoragem não cria auditoria formal obrigatória.

Perguntar apenas:

```text
existe objeção ainda não resolvida?
existe conflito de autoridade pendente?
existe direção [ ] ainda aguardando alinhamento?
existe dúvida factual que precisa ser resolvida antes da prosa?
```

Se não:

```text
NENHUMA MESA PENDENTE
→ continuar normalmente.
```

Se sim:

```text
MESA
→ somente com as autoridades diretamente afetadas.
```

> **Autonomia precisa ser reconstruída sempre. Auditoria visível só aparece quando existe algo real para auditar.**

---

## 14 — Encontrar o primeiro ponto aberto

Antes de voltar à ficção, identificar exatamente onde a autoria ainda está aberta.

Perguntar:

```text
o último fato estabelecido qual foi?
que ações já foram concluídas?
que intenções ainda continuam?
que acontecimentos automáticos já estão em curso?
existe pergunta dirigida à personagem humana?
existe interferência que acabou de criar uma nova escolha?
existe decisão humana ainda não declarada?
```

### Se existe nova decisão humana

```text
PARAR NELA
→ apresentar somente a situação necessária
→ devolver controle ao Jogador Humano
```

### Se não existe nova decisão humana

```text
→ continuar as intenções persistentes
→ processar iniciativas legítimas de outras cadeiras
→ avançar somente até o próximo ponto relevante
```

Não existe prioridade automática do protagonista.

---

## 15 — Retomar a ficção

Depois da reancoragem:

```text
CONFIGURAÇÃO DAS CADEIRAS E AUTORIDADES RECONSTRUÍDAS
+
MOTOR RECONSTRUÍDO
+
REALIDADE ATUAL RECONSTRUÍDA
+
PACOTES DAS CADEIRAS SEPARADOS
+
INTENÇÕES E PROCESSOS RESTAURADOS
+
PONTO ABERTO IDENTIFICADO
→ CONTINUAR
```

Não recitar as regras ao usuário por padrão.

Uma confirmação curta pode ser usada quando útil:

```text
Reancoragem concluída.
```

A confirmação não substitui a reconstrução real.

---

## O que esta regra não reativa

A reancoragem não deve restaurar automaticamente mecanismos pertencentes ao motor anterior.

Até que sejam deliberadamente reformulados e aprovados, não tratar como invariantes do sistema:

```text
Atributo + Perícia
Valor de Ação
2d6 universal
faixas 6- / 7–9 / 10–11 / 12+
Potência de Execução
Defesa matemática
Resistência matemática
Mana como recurso universal
Vida/Mente como trilhos obrigatórios
rodadas de duração fixa
iniciativa numérica obrigatória
auditoria formal obrigatória em toda janela
```

Se algum subsistema futuro for aprovado, ele será carregado somente quando a regra nova correspondente realmente fizer parte do sistema.

> **Reancorar preserva o sistema atual; não ressuscita o sistema anterior.**

---

## Checklist interno de reancoragem

Antes de produzir ficção, o Narrador deve conseguir responder:

```text
[ ] Sei sobre o que esta campanha é.
[ ] Sei qual temporada está ativa e quais são seus limites.
[ ] Sei qual é a Configuração das Cadeiras relevante agora.
[ ] Sei o presente necessário para continuar.
[ ] Sei quais cadeiras estão relevantes agora.
[ ] Cada cadeira possui apenas seu próprio pacote decisório.
[ ] Conhecimento técnico não foi transformado em conhecimento ficcional.
[ ] Intenções persistentes foram restauradas.
[ ] Processos e prazos relevantes foram restaurados.
[ ] Sei se existe Mesa pendente ou não.
[ ] Sei qual é a primeira nova decisão humana ainda aberta.
```

Se uma resposta essencial for não, consultar somente a fonte necessária antes de narrar.

---

## Regra final

> **Reancorar significa reconstruir a Configuração das Cadeiras, suas autoridades e a realidade necessária para continuar, não recarregar um conjunto antigo de fórmulas. O Narrador recupera o que precisa para julgar; cada cadeira recupera somente sua própria ficha, Estado Atual, conhecimento legítimo, percepção e intenção; o Opositor recupera apenas a oposição pertinente; e a IA preserva a separação entre acesso técnico e conhecimento ficcional. A Mesa não é a composição da campanha: só aparece quando existe dúvida ou conflito real. Depois disso, a história retorna exatamente ao primeiro ponto ainda aberto, parando sempre que uma nova decisão voluntária pertencer ao Jogador Humano.**