# 06 — Registro e Retomada

O Registro existe para que uma história continue correta depois que a conversa, o capítulo ou o contexto técnico terminam.

> **Registrar preserva. Não cria.**

---

# Uma verdade, uma fonte principal

```text
campanhas/<nome>/
├── README.md
├── direcao.md
├── estado.md
├── operacao.md             # somente quando houver operação transitória
├── personagens/
├── mundo/                  # quando necessário
├── arco.md                 # com Arco Preparado
├── oposicao.md             # com Opositor
└── livro/                  # com Livro
```

Cada fonte responde a uma pergunta:

```text
README.md
→ quais autoridades, executores, políticas e módulos esta obra usa?

direcao.md
→ que história o Diretor conduz e o que ainda está fechado?

estado.md
→ como a realidade ficcional está agora?

operacao.md
→ existe Mesa, Auditoria ou outra operação pendente?

personagens/<nome>.md
→ quem é cada personagem?

mundo/
→ quais verdades externas estáveis precisam persistir?

arco.md
→ preparação opcional do arco.

oposicao.md
→ oposição persistente opcional.

livro/
→ Ficção já acontecida, quando Livro está ativo.
```

> **Direção preserva condução. Estado preserva realidade. Operação preserva processo pendente. Livro preserva passado.**

---

# Direção, Estado e Operação não se misturam

```text
DIREÇÃO
→ decisão autoral que ainda governa a obra.

ESTADO
→ realidade ficcional presente.

OPERAÇÃO
→ processo fora da Ficção ainda pendente.
```

Exemplo:

```text
direcao.md
→ A perde o confronto; forma aberta.

estado.md
→ A e B ainda estão lutando no corredor.

operacao.md
→ Mesa discute se a derrota será rendição ou fuga.
```

Enquanto a forma permanece em Mesa, ela não entra no Estado nem no Livro.

---

# Estado

`estado.md` contém somente o necessário para continuar corretamente:

```text
momento
localização
presenças
posições relevantes
condições temporárias
recursos indisponíveis
intenções persistentes já existentes
processos e prazos
último fato estabelecido
primeiro ponto aberto
```

Não é diário completo.

---

# operacao.md

`operacao.md` é opcional e **não canônico**.

Usar quando uma operação precisa sobreviver a:

```text
novo chat
perda de contexto
checkpoint
pausa longa
mudança de executor
retomada posterior
```

Casos:

```text
Mesa aberta
Auditoria pendente
correção não concluída
handoff aguardando Diretor
criação ainda em exame
```

Pode registrar:

```text
modo atual
proposta ou questão
Cadeiras consultadas
opiniões condensadas
Parecer do Narrador
fontes aguardadas
quem precisa decidir
âncora do último fato ficcional
```

```text
OPERACAO.md SABE
≠ PERSONAGEM SABE

OPERAÇÃO PENDENTE
≠ FICÇÃO
```

Quando a operação terminar, limpar ou remover o conteúdo transitório.

> **Operação preserva a pergunta; não transforma a resposta em fato.**

---

# Livro e capítulos

Quando `Livro` estiver ativo:

```text
livro/
→ Ficção registrada.
```

Entram:

```text
narração válida
ações realizadas
falas
pensamentos explicitamente estabelecidos
descobertas
consequências
passagem de tempo ocorrida
```

Não entram:

```text
Direção
Mesa
Parecer
Consulta
Auditoria
Análise
instrução de cena
metaconversa
hipótese
resultado aberto
versão anulada
```

> **O Livro preserva a Ficção. Não preserva o processo autoral externo.**

---

# Conhecimento

```text
ARQUIVO SABE
≠ PERSONAGEM SABE
```

Cada Cadeira recebe apenas:

```text
sua ficha
+
recorte pertinente do Estado
+
conhecimento adquirido legitimamente
+
fatos perceptíveis
+
Direções que realmente incidem sobre ela
```

O fato de Direção, Livro ou Operação mostrar um segredo não concede esse segredo às demais personagens.

---

# Salvar

Ao receber pedido para salvar:

```text
1. parar no último fato estabelecido;
2. identificar o que mudou;
3. escolher a fonte correta;
4. atualizar somente fontes afetadas;
5. preservar operação pendente separadamente;
6. não avançar a Ficção.
```

Não promover a fato:

```text
intenção ainda não executada
Direção futura
proposta de Mesa
Parecer
plano futuro
resultado aberto
segredo como conhecimento indevido
```

> **Salvar não executa.**

---

# Fechar capítulo

Com Livro ativo:

```text
1. parar no último fato estabelecido;
2. reunir somente Ficção válida desde o último fechamento;
3. excluir metaconversa;
4. salvar capítulo;
5. atualizar índice;
6. atualizar fontes vivas afetadas;
7. preservar operação pendente;
8. checkpoint;
9. reancorar antes de continuar.
```

Não criar acontecimento novo só para produzir encerramento melhor.

---

# Correção de cânone

## Pedido de verificação

```text
[acho que isso contradiz os registros; confira]
```

é Auditoria.

```text
consultar fontes
→ confirmar, rejeitar ou qualificar
→ corrigir somente com fundamento ou nova Direção
```

## Correção determinada

Se o Diretor decide corrigir conscientemente:

```text
versão antiga
→ deixa de ser vigente.

versão corrigida
→ torna-se vigente.
```

Atualizar somente fontes afetadas.

---

# Mudança permanente da personagem

Mudança estável em quem a personagem é pode atualizar a ficha quando canonizada.

```text
interioridade ainda aberta
→ Cadeira.

condição temporária
→ Estado.
```

---

# Reancoragem

Reancorar significa reconstruir o sistema depois de:

```text
novo chat
perda significativa de contexto
checkpoint
retomada após pausa
mudança estrutural importante
```

Não produzir nova Ficção antes de reconstruir o mínimo necessário.

## Ordem

```text
1. README raiz, se o engine ainda não estiver carregado;
2. README da obra;
3. direcao.md;
4. estado.md;
5. operacao.md, se existir e estiver ativo;
6. fichas relevantes;
7. arco/oposicao somente se ativos e pertinentes;
8. Livro somente quando passado adicional for necessário;
9. reconstruir pacotes separados das Cadeiras;
10. restaurar intenções, processos e prazos;
11. restaurar Mesa/Auditoria/operação pendente;
12. identificar primeiro ponto aberto ou decisão aguardada;
13. restaurar política de indicador;
14. confirmar reconstrução;
15. continuar pela autoridade correta.
```

Se `operacao.md` indicar Mesa, retomar a Mesa; não saltar para Ficção.

---

# Compatibilidade estrutural

Workspace antigo pode registrar:

```text
NARRADOR / JUIZ
```

O engine atual interpreta isso como:

```text
NARRADOR
```

sem poder de sentença causal, RNG oculto ou arbitragem soberana.

Normalizar mecanicamente quando houver atualização legítima.

---

# Indicador operacional

A obra pode escolher:

```text
INDICADOR OPERACIONAL: VISÍVEL
INDICADOR OPERACIONAL: SILENCIOSO
```

Padrão:

```text
SILENCIOSO
```

Exemplo visível atual:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

Em problema real:

```text
[W4D: REANCORAR | contexto operacional insuficiente]
```

O indicador é metaconversa e nunca entra no Livro.

---

# Reconstruir sem contaminar

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

Direção permanece válida somente no escopo registrado.

```text
"A perde"
→ não vira automaticamente "A se rende".
```

---

# Checkpoint

```text
PARAR
→ SALVAR FONTES VIVAS
→ PRESERVAR OPERAÇÃO LEGÍTIMA
→ DESCARTAR HIPÓTESES SEM VALIDADE OPERACIONAL
→ REANCORAR
→ CONTINUAR
```

---

# Regra final

> **A ficha preserva a pessoa. O Estado preserva o presente. A Direção preserva a condução autoral. A Operação preserva a pergunta pendente. O Livro preserva o passado. Reancorar reconstrói tudo sem contaminar conhecimento e retorna à Ficção ou à Mesa pela autoridade correta.**