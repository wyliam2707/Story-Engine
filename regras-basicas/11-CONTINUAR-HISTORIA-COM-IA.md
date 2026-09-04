# 11 — Continuar uma História com IA

Este arquivo define a experiência operacional do ramo `CONTINUAR HISTÓRIA EXISTENTE`.

Ele entra em uso **depois** que o BOOT já identificou que o Diretor quer retomar uma obra existente.

> **Continuar é localizar a obra correta, validar suas fontes, reconstruir o ponto real de retorno e só então retomar a camada que estava ativa.**

Este arquivo coordena a retomada. As regras normativas de persistência, conhecimento e reancoragem continuam em `06-REGISTRO-E-RETOMADA.md`.

---

# Fluxo completo

```text
CONTINUAR HISTÓRIA EXISTENTE
↓
IDENTIFICAR A OBRA
↓
VALIDAR O WORKSPACE
↓
CARREGAR AS FONTES NECESSÁRIAS
↓
RECONSTRUIR A REALIDADE FICCIONAL
↓
RECONSTRUIR AS CADEIRAS
↓
RECONSTRUIR A OPERAÇÃO PENDENTE, SE HOUVER
↓
AUDITAR O PONTO DE RETORNO
↓
RETOMAR A CAMADA CORRETA
```

```text
RETOMAR
≠ RECRIAR
```

Não pedir novamente premissa, estilo, personagens, relações ou regras que já estejam preservadas nas fontes da obra.

---

# Passo 1 — Identificar a obra

## Obra nomeada pelo Diretor

Se o Diretor já identifica a obra:

```text
"continue Duas Vidas Normais"
"retome a campanha cidade partida"
"continue campanhas/duas-vidas-normais"
```

então:

```text
identificar a pasta correspondente
→ não perguntar o nome novamente
→ seguir para validação
```

Não substituir a obra nomeada por outra apenas porque outra foi modificada mais recentemente.

## Diretor não informa o nome

Se ele disser apenas:

```text
"quero continuar uma história"
"retome uma antiga"
"vamos continuar"
```

examinar as obras disponíveis em `campanhas/`.

### Nenhuma obra disponível

```text
0 obras localizadas
→ informar que não existe história persistida para retomar
→ perguntar se o Diretor quer criar uma nova
```

Não inventar uma campanha perdida.

### Uma única obra disponível

```text
1 obra disponível
→ identificá-la
→ informar brevemente qual foi encontrada
→ prosseguir para validação sem exigir escolha redundante
```

### Mais de uma obra disponível

Não escolher silenciosamente por recência, preferência da IA ou semelhança temática.

Mostrar lista curta suficiente para o Diretor reconhecer cada obra, usando quando disponível:

```text
nome
status
proposta curta
```

A data de modificação pode ordenar a lista; não decide pela pessoa.

> **Recência ajuda a localizar. Não concede autoridade para escolher.**

---

# Passo 2 — Ler primeiro o README da obra

Depois de identificar a pasta, carregar primeiro:

```text
campanhas/<slug>/README.md
```

O README deve permitir reconhecer pelo menos:

```text
nome da obra
status
autoridades e executores
Personagem do Diretor, se houver
política de Mesa
módulos ativos
convenções operacionais relevantes
cânone externo, quando houver
```

O README da obra é a porta de entrada da história existente.

Não começar lendo capítulos aleatórios para inferir configuração atual.

---

# Passo 3 — Interpretar o status

Estados recomendados:

```text
EM PREPARAÇÃO
→ retomar o processo de criação; não abrir Ficção ainda.

PRONTA
→ estrutura suficiente; pode existir Ficção a iniciar ou retomar.

EM EXECUÇÃO
→ obra em andamento; reancorar normalmente.

PAUSADA
→ obra em andamento interrompida; reancorar normalmente.

ENCERRADA
→ não reabrir automaticamente a Ficção;
→ informar o estado e aguardar o Diretor dizer se quer reabrir, continuar depois do encerramento ou apenas consultar.
```

Se obra antiga usar nomenclatura equivalente como `PRONTA PARA JOGAR`, interpretar semanticamente sem exigir migração antes da retomada.

Status desconhecido não autoriza a IA a inventar significado. Tratar como ponto de Auditoria documental.

---

# Passo 4 — Validar o workspace

Para obra em Ficção, verificar primeiro:

```text
README.md
→ obrigatório.

direcao.md
→ esperado.

estado.md
→ obrigatório para retomada precisa.

personagens/
→ deve conter fichas necessárias para as Cadeiras que serão reconstruídas.
```

Fontes condicionais:

```text
operacao.md
→ quando existe operação transitória persistida.

arco.md
→ quando Arco Preparado está ativo e pertinente.

oposicao.md
→ quando Opositor está ativo e pertinente.

livro/
→ quando Livro está ativo.

mundo/
→ quando fatos externos persistentes exigirem consulta.
```

A validação não precisa ler tudo. Primeiro verifica integridade suficiente para retomada confiável.

---

# Falhas de integridade

## Falha bloqueante

Exemplos:

```text
estado.md ausente numa história já em andamento
não é possível identificar o último fato ficcional
não é possível saber qual personagem o Diretor controla
Cadeira necessária não possui informação suficiente para reconstrução
fontes existentes se contradizem exatamente no ponto de retorno
fluxo antigo ainda depende de Juiz para decidir resultado material aberto
```

Nesse caso:

```text
NÃO IMPROVISAR CONTINUIDADE
→ abrir Auditoria
→ informar o que falta ou contradiz
→ reparar somente a partir de fonte legítima ou decisão do Diretor
```

## Falha reparável sem inventar Ficção

Exemplos:

```text
README usa status antigo equivalente
README usa rótulo legado NARRADOR / JUIZ, mas sem depender de poder de Juiz
índice do Livro está desatualizado mas capítulos são identificáveis
arquivo opcional declarado não é pertinente à cena atual
formatação antiga não muda o significado
```

A IA pode normalizar sua leitura operacional sem interromper a retomada, desde que não altere fatos ou autoridade.

```text
NARRADOR / JUIZ
→ interpretar como NARRADOR
→ não reativar sentença causal, RNG oculto ou arbitragem soberana.
```

> **Tolerar formato antigo não significa preencher conteúdo ausente nem reativar função removida.**

---

# Passo 5 — Carregar somente o necessário

Seguir a ordem de reancoragem de `06-REGISTRO-E-RETOMADA.md`:

```text
1. README da obra
2. direcao.md
3. estado.md
4. operacao.md, se houver operação ativa
5. fichas das personagens relevantes
6. arco.md / oposicao.md, se ativos e pertinentes
7. mundo necessário
8. Livro somente para passado que precise ser reconstruído
```

```text
CONTEXTO NECESSÁRIO
≠ TODO O MATERIAL DISPONÍVEL
```

Capítulos ajudam a reconstruir passado, mas não substituem `estado.md` como fonte do presente.

---

# Passo 6 — Reconstruir a realidade presente

A IA deve ser capaz de responder internamente:

```text
quando estamos?
onde estamos?
quem está presente ou materialmente envolvido?
qual é a situação atual?
quais condições temporárias importam?
quais intenções persistentes continuam ativas?
quais processos ou prazos continuam correndo?
qual foi o último fato realmente estabelecido?
```

Se não consegue responder o suficiente para continuar corretamente, a reancoragem ainda não terminou.

---

# Passo 7 — Reconstruir as Cadeiras

Para cada Cadeira necessária ao próximo bloco:

```text
ficha própria
+
conhecimento legítimo
+
recorte pertinente do Estado
+
relações relevantes
+
Direções que realmente incidem sobre ela
+
intenção atual, se já estabelecida
```

Não entregar automaticamente a uma Cadeira:

```text
ficha alheia
segredo de mundo não descoberto
pensamento mostrado ao leitor
informação conhecida apenas na Mesa
plano do Opositor
Direção futura que a personagem não conhece
```

```text
EXECUTOR RECONSTRÓI TUDO
≠ PERSONAGEM PASSA A SABER TUDO
```

---

# Passo 8 — Reconstruir a camada operacional

Depois de reconstruir a Ficção, verificar `operacao.md`, quando existir.

## Mesa pendente

```text
operacao.md → MESA
```

Então:

```text
restaurar proposta em exame
restaurar Cadeiras já consultadas
restaurar opiniões condensadas
restaurar Parecer do Narrador
identificar o que o Diretor ainda precisa decidir
→ permanecer na Mesa
```

Não executar a proposta durante a retomada.

## Auditoria pendente

```text
operacao.md → AUDITORIA
```

Continuar a verificação antes de qualquer Ficção dependente dela.

## Correção pendente

Reconstruir exatamente o que estava sendo corrigido e qual versão continua vigente até conclusão.

## Nenhuma operação pendente

Retornar ao `primeiro ponto aberto` de `estado.md`.

> **Retomar a camada errada é erro de continuidade mesmo quando os fatos foram lidos corretamente.**

---

# Passo 9 — Auditar o ponto de retorno

Antes de continuar, responder internamente:

```text
CAMADA ATUAL
→ Mesa / Ficção / Auditoria / Preparação / outra operação legítima.

ÚLTIMO FATO FICCIONAL
→ qual foi?

PRÓXIMO PONTO REAL
→ o que ainda não foi decidido ou executado?

PRÓXIMA AUTORIA OU FUNÇÃO
→ existe decisão voluntária? De quem?
→ ou existe apenas consequência ordinária/evidente a apresentar?
→ ou existe resultado material importante ainda aberto que precisa de Mesa?
```

Se essas respostas entram em conflito, não continuar até resolver a inconsistência.

---

# Passo 10 — Como responder depois de reancorar

A retomada não precisa produzir relatório longo.

Formato recomendado quando a Ficção está pronta:

```text
[Nome] reancorada.

Último fato: [...]
Ponto atual: [...]
```

Depois aplicar:

```text
próxima autoria pertence a Cadeira IA disponível
→ trocar de escopo
→ decidir
→ continuar.

próximo passo é consequência ordinária e evidente
→ Narrador apresenta
→ continuar.

resultado material importante permanece realmente aberto
→ Narrador não escolhe secretamente
→ Mesa, quando necessária.

próxima autoria pertence ao Diretor ou executor externo indisponível
→ parar no ponto
→ aguardar.
```

O comando `continue` ou `retome` autoriza a retomada da obra; **não concede à IA autoridade sobre decisões que continuam pertencendo ao Diretor**.

## Mesa pendente

Formato recomendado:

```text
[Nome] reancorada em MESA.

Proposta em consulta: [...]
Parecer atual: [...]
Aguardando: decisão do Diretor.
```

Não narrar.

## Auditoria pendente

Informar resumidamente o que está sendo verificado e continuar a Auditoria quando possível.

## Preparação ainda não concluída

Retomar exatamente a etapa de criação pendente em vez de abrir a primeira cena.

---

# Continuar não significa pedir confirmação de tudo

Se o Diretor já disse:

```text
"continue Duas Vidas Normais"
```

não responder apenas:

```text
"Encontrei a campanha. Deseja que eu a carregue?"
```

A intenção de retomada já está dada.

Depois de reancorar uma cena cujo próximo movimento pertence a Cadeira IA disponível, não pedir `posso continuar?`.

Do mesmo modo, uma consequência evidente não exige permissão ou Mesa artificial.

Parar quando a próxima autoria legítima realmente depende do Diretor, de outro executor indisponível, ou quando uma operação autoral está pendente.

> **Não pedir permissão para executar autoridade que já foi atribuída. Não assumir autoridade que não foi atribuída.**

---

# Não atualizar fontes apenas por retomar

Reancoragem é leitura e reconstrução.

Atualizar fontes somente quando:

```text
uma correção foi legitimamente determinada
um fato novo foi executado
uma mudança persistente aconteceu
um salvamento/checkpoint foi solicitado
uma operação pendente precisa ser preservada
```

```text
RETOMAR
≠ SALVAR
≠ REESCREVER
```

---

# Protocolo mínimo para uma IA

```text
1. identificar a obra;
2. se houver múltiplas opções e nenhuma foi nomeada, deixar o Diretor escolher;
3. carregar README da obra;
4. interpretar o status;
5. validar fontes mínimas;
6. abrir Auditoria se houver falha bloqueante;
7. carregar Direção, Estado, Operação e fichas pertinentes;
8. reconstruir Cadeiras sem contaminar conhecimento;
9. restaurar módulos pertinentes;
10. identificar a camada atual;
11. identificar último fato e próximo ponto real;
12. identificar próxima autoria ou função;
13. informar brevemente a reancoragem;
14. continuar quando Cadeira IA ou continuidade evidente permitir;
15. usar Mesa quando resultado material importante continuar aberto;
16. parar quando a próxima autoria exigir Diretor ou executor externo indisponível.
```

---

# Regra final

> **Continuar uma história não é recontá-la, reconstruí-la do zero nem escolher por recência. A IA identifica a obra correta, valida suas fontes, reancora presente, personagens e operação, encontra a próxima autoria ou função legítima e retorna exatamente à camada em que a obra realmente parou — sem transformar o Narrador em Juiz.**