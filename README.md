# W4D — Story Engine

W4D é uma **arquitetura de autoria narrativa distribuída**.

Ele nasceu como RPG puramente narrativo, mas evoluiu para uma estrutura mais ampla de construção de ficção com humanos e IAs.

Pode ser usado como:

```text
RPG narrativo
coautoria de histórias com IA
sala de roteiro distribuída
fanfic assistida
motor para ficção seriada
ferramenta de continuidade narrativa
```

A ideia central é simples:

> **O Diretor conduz. As Cadeiras preservam as personagens. O Narrador emite parecer na Mesa e sentença na Ficção. O Registro preserva.**

---

# Se você é uma IA: comece aqui

Leia primeiro:

```text
regras-basicas/README.md
```

Essa pasta é a especificação operacional vigente do W4D.

Ela explica:

```text
Mesa de Autoria
políticas de consulta
Diretor e Direção
Cadeiras e Executores
Resolução causal
Ficha
Narrador/Juiz
Plausibilidade e ritmo
Estado operacional
Registro e retomada
Criação de história
Inicialização de uma história com IA
```

Não use como regra versões antigas recuperadas do histórico do Git, memória de conversas anteriores ou hábitos genéricos de outros RPGs quando os arquivos atuais definirem a questão.

A branch `main` representa o sistema vigente.

---

# O ciclo do W4D

## Mesa

O Diretor pode testar uma ideia antes de colocá-la na ficção.

```text
PROPOSTA OU DECISÃO EM EXAME
→ Cadeiras envolvidas opinam
→ Narrador emite PARECER
→ Diretor altera, cancela ou autoriza execução
```

Enquanto a Mesa estiver aberta:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO DA CADEIRA ≠ DECISÃO FICCIONAL
PARECER DO NARRADOR ≠ SENTENÇA
```

A política de cada obra define quando a Mesa é acionada.

## Ficção

Depois da autorização:

```text
Cadeiras exercem autoria no espaço aberto
→ Narrador cruza fatos, intenções e Direção
→ Narrador produz SENTENÇA causal
→ prosa apresenta o que aconteceu
```

## Registro

Quando solicitado:

```text
ficção estabelecida
→ fontes canônicas são atualizadas
```

> **Registrar preserva. Não cria.**

---

# Estado e Operação

O W4D separa o presente ficcional do processo autoral pendente.

```text
estado.md
→ realidade atual da Ficção.

operacao.md
→ Mesa, Auditoria, Correção ou outra operação transitória ainda pendente.
```

`operacao.md` é opcional e não canônico.

> **Operação preserva a pergunta; não cria a resposta.**

---

# Autoridades principais

```text
DIRETOR
→ conduz a obra e pode deixar aberto, alinhar ou determinar.

CADEIRA
→ autoria voluntária de uma personagem dentro do espaço aberto.

EXECUTOR
→ humano, IA ou outro participante que opera uma autoridade.

NARRADOR / JUIZ
→ na Mesa emite parecer; na Ficção sentencia causalidade e narra.

AUDITORIA
→ verifica fatos, coerência, autoridade e escopo; informa sem governar o Diretor.
```

Uma única IA pode executar várias Cadeiras e o Narrador, desde que mantenha os escopos separados.

```text
MESMO EXECUTOR
≠
MESMA CADEIRA
```

---

# Criar uma história

Se ainda não existe uma obra pronta, siga:

```text
regras-basicas/10-INICIAR-HISTORIA-COM-IA.md
```

No W4D, `campanha` ainda é o nome técnico atual da pasta persistente da obra. A obra pode ou não ser um RPG.

A estrutura mínima recomendada continua:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

`operacao.md` aparece somente quando uma operação transitória precisa persistir.

Modelos estão em:

```text
regras-basicas/modelos/
```

---

# Retomar uma história

Para continuar uma obra existente:

```text
README da obra
→ direcao.md
→ estado.md
→ operacao.md, se houver
→ fichas relevantes
→ módulos ativos
→ reancorar
→ identificar a camada e o ponto corretos
→ continuar
```

Detalhes em:

```text
regras-basicas/06-REGISTRO-E-RETOMADA.md
```

---

# Módulos opcionais

```text
regras-basicas/modulos/ARCO-PREPARADO.md
regras-basicas/modulos/OPOSITOR.md
regras-basicas/modulos/ROMANCE.md
regras-basicas/modulos/LIVRO.md
```

Módulo inativo não participa da obra.

---

# Princípio documental

> **Uma ideia, uma definição, uma fonte principal.**

Quando duas leituras parecerem competir, use o arquivo cuja função é definir especificamente aquela questão e abra Auditoria se necessário.

---

## Lema

> **Propor para ouvir. Emitir parecer para entender. Determinar para fechar. Executar para existir. Registrar para preservar.**