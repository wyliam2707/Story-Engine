# 06 — Registro e Retomada

O Registro existe para que a campanha continue correta depois que a conversa, o capítulo ou o contexto técnico terminam.

> **Registrar preserva. Não cria.**

## Uma verdade, uma fonte principal

A estrutura recomendada de campanha é:

```text
campanhas/<nome>/
├── README.md
├── direcao.md
├── estado.md
├── personagens/
├── mundo/                 # quando necessário
├── arco.md                # somente com módulo Arco Preparado
├── oposicao.md            # somente com módulo Opositor
└── livro/                 # somente com módulo Livro
```

Cada fonte responde a uma pergunta diferente.

```text
README.md
→ quais autoridades, executores e módulos esta campanha usa?

direcao.md
→ que história o Diretor está conduzindo e o que ainda está autoralmente fechado?

estado.md
→ como a realidade ficcional está agora?

personagens/<nome>.md
→ quem é cada personagem?

mundo/
→ que verdades externas estáveis precisam persistir?

arco.md
→ que preparação opcional existe para o arco atual?

oposicao.md
→ que oposição persistente opcional continua agindo?

livro/
→ que ficção já aconteceu, organizada em capítulos, quando o módulo Livro estiver ativo?
```

## Direção e Estado são diferentes

Não misturar:

```text
DIREÇÃO
→ para onde a obra deve ir / o que está fechado autoralmente.

ESTADO
→ o que já é verdade agora dentro da ficção.
```

Exemplo:

```text
direcao.md
→ A perde o confronto atual; forma aberta.

estado.md
→ A e B ainda estão lutando no corredor.
```

Enquanto a derrota não aconteceu, ela não entra no Estado como fato consumado.

Depois que acontecer:

```text
estado.md
→ registra a nova situação presente, se ainda relevante.

direcao.md
→ remove a Direção local já consumida.

livro/
→ pode registrar como aconteceu, se o módulo Livro estiver ativo.
```

## Estado

`estado.md` deve conter somente o necessário para continuar corretamente agora:

```text
momento
localização
presenças
posições relevantes
condições temporárias
indisponibilidade de equipamentos ou recursos
intenções persistentes
processos e prazos próximos
último fato estabelecido
primeiro ponto ainda aberto
```

Não é diário completo.

A ficha não duplica esse estado.

## Livro e capítulos

Quando o módulo Livro estiver ativo, o Livro preserva a ficção já acontecida.

```text
livro/
→ obra completa registrada.

livro/001-....md
→ primeiro capítulo.

livro/002-....md
→ segundo capítulo.
```

O capítulo registra ficção, não a Direção usada para conduzi-la.

Entram:

```text
narração válida
ações realmente realizadas
falas
pensamentos explicitamente estabelecidos
descobertas
consequências
passagem de tempo ocorrida
```

Não entram:

```text
Direção
Consulta
Auditoria
Análise
instrução de cena
metaconversa
hipótese
resultado aberto
versão anulada ou refeita
```

Quando a origem estiver estabelecida, preservar marcadores como:

```text
NARRADOR
KARA
KARA — pensamento
DANIEL
DANIEL — pensamento
```

Isso permite reconstruir o passado sem transformar conhecimento do leitor em conhecimento universal das personagens.

> **O Livro preserva a ficção. Não preserva o processo autoral que ficou fora da ficção.**

## Conhecimento

```text
ARQUIVO SABE
≠
PERSONAGEM SABE
```

Cada Cadeira recebe apenas:

```text
sua ficha
+
recorte do Estado pertinente
+
conhecimento que adquiriu legitimamente
+
fatos perceptíveis da cena
```

Conhecimento recorrente importante pode ser consolidado na ficha da personagem quando fizer parte estável de seu repertório.

O fato de um capítulo mostrar um pensamento, segredo ou narração externa não concede esse conhecimento a outra Cadeira.

## Salvar

Ao receber pedido para salvar:

```text
1. parar no último fato estabelecido;
2. identificar o que mudou;
3. escolher a fonte correta;
4. atualizar somente fontes afetadas;
5. não avançar a ficção durante o salvamento.
```

Não promover a fato consumado:

```text
intenção ainda não executada
Direção futura
hipótese
plano futuro
resultado aberto
segredo como conhecimento de quem não o descobriu
```

> **Salvar não joga.**

## Fechar capítulo

Quando o módulo Livro estiver ativo, `fechar o capítulo` é uma operação de registro e checkpoint.

```text
1. parar no último fato realmente estabelecido;
2. reunir somente a ficção válida desde o último capítulo fechado;
3. excluir Direção, consultas, auditorias, instruções de cena e demais metaconversas;
4. preservar quem narrou, falou, agiu ou pensou quando essa origem estiver definida;
5. salvar o novo capítulo dentro de livro/;
6. atualizar o índice do Livro;
7. atualizar somente as fontes vivas realmente afetadas;
8. executar checkpoint operacional;
9. reancorar antes de continuar.
```

Não criar um acontecimento novo apenas para produzir um encerramento melhor.

Se uma cena foi corrigida ou refeita, entra somente a versão final válida.

> **Fechar capítulo registra onde a ficção parou. Não joga o fechamento.**

## Correção de cânone

Quando uma inconsistência é identificada, distinguir duas situações.

### Pedido de verificação

```text
DIRETOR
→ [acho que isso contradiz os registros; confira]
```

Isso é Auditoria, não determinação de que a hipótese está correta.

```text
consultar fontes
→ confirmar, rejeitar ou qualificar
→ responder
→ corrigir somente com fundamento ou nova Direção.
```

### Correção determinada

Se o Diretor decide corrigir o cânone conscientemente:

```text
versão antiga
→ deixa de ser vigente.

versão corrigida
→ torna-se vigente.
```

Atualizar somente as fontes que realmente dependem da mudança.

O histórico do Git pode preservar a versão técnica antiga; a campanha ativa não mantém duas verdades concorrentes.

## Mudança permanente da personagem

Se a ficção produz mudança estável em quem a personagem é, atualizar a ficha quando essa mudança for canonizada.

Interioridade ainda aberta pertence à Cadeira até ser decidida ou fechada pelo Diretor.

Condição temporária permanece apenas no Estado.

## Reancoragem

Reancorar significa reconstruir o sistema operacional depois de:

```text
novo chat
perda significativa de contexto
checkpoint
retomada depois de pausa
mudança estrutural importante
```

Não produzir nova ficção antes de reconstruir o mínimo necessário.

### Ordem de reancoragem

```text
1. ler README.md da raiz do repositório se o sistema não estiver carregado;
2. carregar README.md da campanha;
3. carregar direcao.md;
4. carregar estado.md;
5. carregar fichas relevantes;
6. carregar arco.md/oposicao.md somente se ativos e pertinentes;
7. usar capítulos anteriores apenas para reconstruir passado quando necessário, sem universalizar conhecimento;
8. reconstruir pacotes separados das Cadeiras;
9. restaurar intenções, processos e prazos;
10. identificar Auditoria pendente;
11. identificar o primeiro ponto ainda aberto;
12. só então continuar a ficção.
```

## Reconstruir sem contaminar

Ao retomar:

```text
DIRETOR SABE
≠ PERSONAGEM SABE

ESTADO GLOBAL EXISTE
≠ TODAS AS PERSONAGENS SABEM

LIVRO MOSTRA
≠ TODAS AS PERSONAGENS SABEM

MESMO EXECUTOR
≠ MESMA CADEIRA
```

Direção vinculante permanece válida somente no escopo registrado.

```text
"A perde"
→ não vira automaticamente "A se rende".
```

## Checkpoint

Um checkpoint operacional pode ser usado para limpar ruído acumulado mesmo sem módulo Livro.

```text
PARAR
→ SALVAR FONTES VIVAS
→ DESCARTAR HIPÓTESES E INTERPRETAÇÕES PROVISÓRIAS
→ REANCORAR
→ CONTINUAR
```

Com o módulo Livro ativo, `fechar o capítulo` consolida primeiro a ficção do capítulo e então executa esse checkpoint.

## Regra final

> **A ficha preserva a pessoa. O Estado preserva o presente. A Direção preserva a condução autoral. O mundo preserva fatos externos. O Livro preserva a ficção passada em capítulos. Reancorar reconstrói essas fontes sem transformá-las em conhecimento universal e retorna exatamente ao primeiro ponto ainda aberto.**