# 06 — Registro e Retomada

O Registro existe para que uma história continue correta depois que a conversa, o capítulo ou o contexto técnico terminam.

> **Registrar preserva. Não cria.**

## Uma verdade, uma fonte principal

A estrutura recomendada é:

```text
campanhas/<nome>/
├── README.md
├── direcao.md
├── estado.md
├── operacao.md             # somente quando houver operação transitória que precise persistir
├── personagens/
├── mundo/                  # quando necessário
├── arco.md                 # somente com módulo Arco Preparado
├── oposicao.md             # somente com módulo Opositor
└── livro/                  # somente com módulo Livro
```

Cada fonte responde a uma pergunta diferente.

```text
README.md
→ quais autoridades, executores, políticas e módulos esta obra usa?

direcao.md
→ que história o Diretor está conduzindo e o que ainda está autoralmente fechado?

estado.md
→ como a realidade ficcional está agora?

operacao.md
→ existe uma Mesa, Auditoria ou outra operação transitória ainda pendente?

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

> **Direção preserva condução. Estado preserva realidade. Operação preserva processo pendente. Livro preserva passado.**

## Direção, Estado e Operação são diferentes

Não misturar:

```text
DIREÇÃO
→ para onde a obra deve ir / o que está fechado autoralmente.

ESTADO
→ o que já é verdade agora dentro da ficção.

OPERAÇÃO
→ o que a Mesa ou o sistema ainda está discutindo/verificando fora da ficção.
```

Exemplo:

```text
direcao.md
→ A perde o confronto atual; forma aberta.

estado.md
→ A e B ainda estão lutando no corredor.

operacao.md
→ Mesa aberta discutindo se a forma da derrota deve envolver rendição ou fuga.
```

Enquanto a forma ainda está apenas em Mesa, ela não entra no Estado nem no Livro.

## Estado

`estado.md` deve conter somente o necessário para continuar corretamente a realidade ficcional:

```text
momento
localização
presenças
posições relevantes
condições temporárias
indisponibilidade de equipamentos ou recursos
intenções persistentes já existentes na ficção
processos e prazos próximos
último fato estabelecido
primeiro ponto ainda aberto
```

Não é diário completo.

A ficha não duplica esse Estado.

## Estado operacional — operacao.md

`operacao.md` é opcional e **não canônico**.

Use-o somente quando uma operação fora da ficção precisa sobreviver a:

```text
novo chat
perda de contexto
checkpoint
pausa longa
mudança de executor
retomada posterior
```

Casos típicos:

```text
Mesa de Autoria ainda aberta
Auditoria ainda pendente
correção ainda não concluída
handoff aguardando decisão do Diretor
```

Modelo:

```text
modelos/OPERACAO.md
```

Pode registrar:

```text
modo atual
proposta ou questão em consulta
Cadeiras consultadas
opiniões condensadas
parecer do Narrador
fontes ainda aguardadas
quem precisa decidir a próxima etapa
âncora do último fato ficcional
```

Não colocar nele invenções novas para “lembrar depois”. Ele preserva somente uma operação já iniciada.

```text
OPERACAO.md SABE
≠ PERSONAGEM SABE

OPERAÇÃO PENDENTE
≠ FICÇÃO
```

Quando a Mesa for cancelada ou executada, quando a Auditoria terminar ou quando a operação deixar de existir, limpar o arquivo ou remover o conteúdo transitório.

> **Operação preserva a pergunta; não transforma a resposta em fato.**

## Livro e capítulos

Quando o módulo Livro estiver ativo, o Livro preserva a ficção já acontecida.

```text
livro/
→ obra registrada.

livro/001-....md
→ primeiro capítulo.

livro/002-....md
→ segundo capítulo.
```

O capítulo registra ficção, não a Direção nem a Mesa usada para produzi-la.

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
Mesa de Autoria
Parecer
Consulta
Auditoria
Análise
instrução de cena
metaconversa
hipótese
resultado aberto
versão anulada ou refeita
```

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
+
Direções que realmente incidem sobre ela
```

`operacao.md` pode conter informação de Mesa que nenhuma personagem conhece.

O fato de um capítulo, Direção ou Operação mostrar um segredo não concede esse conhecimento a outra Cadeira.

## Salvar

Ao receber pedido para salvar:

```text
1. parar no último fato estabelecido;
2. identificar o que mudou;
3. escolher a fonte correta;
4. atualizar somente fontes afetadas;
5. preservar operação pendente separadamente, se existir;
6. não avançar a ficção durante o salvamento.
```

Não promover a fato consumado:

```text
intenção ainda não executada
Direção futura
proposta de Mesa
Parecer
plano futuro
resultado aberto
segredo como conhecimento de quem não o descobriu
```

> **Salvar não executa.**

## Fechar capítulo

Quando o módulo Livro estiver ativo, `fechar o capítulo` é uma operação de registro e checkpoint.

```text
1. parar no último fato realmente estabelecido;
2. reunir somente a ficção válida desde o último capítulo fechado;
3. excluir Direção, Mesa, Parecer, auditorias e demais metaconversas;
4. preservar quem narrou, falou, agiu ou pensou quando essa origem estiver definida;
5. salvar o novo capítulo dentro de livro/;
6. atualizar o índice do Livro;
7. atualizar somente as fontes vivas realmente afetadas;
8. preservar operacao.md se uma operação ainda estiver legitimamente pendente;
9. executar checkpoint operacional;
10. reancorar antes de continuar.
```

Não criar um acontecimento novo apenas para produzir um encerramento melhor.

Se uma cena foi corrigida ou refeita, entra somente a versão final válida.

> **Fechar capítulo registra onde a ficção parou. Não executa o fechamento.**

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

Se a Auditoria precisar ser interrompida e retomada depois, `operacao.md` pode preservar o que ainda está pendente.

### Correção determinada

Se o Diretor decide corrigir o cânone conscientemente:

```text
versão antiga
→ deixa de ser vigente.

versão corrigida
→ torna-se vigente.
```

Atualizar somente as fontes que realmente dependem da mudança.

O histórico do Git pode preservar a versão técnica antiga; a obra ativa não mantém duas verdades concorrentes.

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
2. carregar README.md da obra;
3. carregar direcao.md;
4. carregar estado.md;
5. carregar operacao.md se existir e estiver ativo;
6. carregar fichas relevantes;
7. carregar arco.md/oposicao.md somente se ativos e pertinentes;
8. usar capítulos anteriores apenas para reconstruir passado quando necessário, sem universalizar conhecimento;
9. reconstruir pacotes separados das Cadeiras;
10. restaurar intenções, processos e prazos ficcionais;
11. restaurar Mesa/Auditoria/operação pendente, se houver;
12. identificar o primeiro ponto ainda aberto ou a decisão autoral aguardada;
13. restaurar a política de indicador operacional;
14. confirmar operacionalmente a reconstrução conforme a configuração da obra;
15. só então continuar.
```

Se `operacao.md` indicar `MESA`, retomar a Mesa; não saltar diretamente para a Ficção.

## Indicador operacional

O indicador `[W4D: ...]` é útil para depuração e reancoragem, mas não precisa aparecer em toda resposta de toda obra.

A configuração pode escolher:

```text
INDICADOR OPERACIONAL: VISÍVEL
→ mostrar status curto durante a execução conforme útil.

INDICADOR OPERACIONAL: SILENCIOSO
→ omitir em respostas normais;
→ mostrar somente em reancoragem, erro operacional, perda de contexto ou quando solicitado.
```

Se a obra não configurar, usar `SILENCIOSO` como padrão de Story Engine.

Exemplo visível:

```text
[W4D: OK | Narrador/Juiz ✓ | Cadeiras IA ✓]
```

Quando existir problema real:

```text
[W4D: REANCORAR | contexto operacional insuficiente]
```

Mesmo no modo silencioso, uma falha que impede execução correta deve ser informada; o sistema não deve fingir `OK`.

O indicador é metaconversa operacional. Não entra no Livro nem se torna fato ficcional.

## Reconstruir sem contaminar

Ao retomar:

```text
DIRETOR SABE
≠ PERSONAGEM SABE

MESA SABE
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
→ PRESERVAR OPERAÇÃO LEGÍTIMA AINDA PENDENTE
→ DESCARTAR HIPÓTESES SEM VALIDADE OPERACIONAL
→ REANCORAR
→ CONTINUAR
```

Com o módulo Livro ativo, `fechar o capítulo` consolida primeiro a ficção do capítulo e então executa esse checkpoint.

## Regra final

> **A ficha preserva a pessoa. O Estado preserva o presente ficcional. A Direção preserva a condução autoral. A Operação preserva Mesa, Auditoria ou outra pergunta transitória sem canonizá-la. O Livro preserva o passado ficcional. Reancorar reconstrói essas fontes sem contaminar conhecimento e retorna ao ponto correto da Ficção ou da Mesa.**