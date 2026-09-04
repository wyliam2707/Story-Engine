# W4D — Arquitetura de Autoria Narrativa Distribuída

W4D nasceu como um RPG puramente narrativo, mas evoluiu para uma arquitetura mais ampla de construção de ficção.

Ele pode ser usado como:

```text
RPG narrativo
coautoria de histórias com IA
sala de roteiro distribuída
fanfic assistida
motor para ficção seriada
```

A ideia central continua simples:

> **O Diretor conduz. As Cadeiras preservam as personagens. O Narrador julga. A ficção executa. O Registro preserva.**

---

# Se você é uma IA: comece aqui

Leia primeiro:

```text
regras-basicas/README.md
```

Essa pasta é a especificação operacional do W4D e foi escrita para ser autossuficiente.

Ela explica:

```text
Mesa de Autoria
Diretor e Direção
Cadeiras e Executores
Resolução causal
Ficha
Narrador/Juiz
Plausibilidade e ritmo
Registro e retomada
Criação de campanha/história
Inicialização de uma história com IA
```

Não use como regra versões antigas recuperadas do histórico do Git, memória de conversas anteriores ou hábitos genéricos de outros RPGs quando os arquivos atuais definirem a questão.

A branch `main` representa o sistema vigente.

---

# O ciclo do W4D

## Mesa

O Diretor pode testar uma ideia antes de colocá-la na ficção.

```text
PROPOSTA
→ Cadeiras envolvidas opinam
→ Narrador analisa e julga
→ Diretor altera, cancela ou confirma
```

Enquanto a Mesa estiver aberta:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO DA CADEIRA ≠ ACONTECIMENTO
ANÁLISE DO NARRADOR ≠ FICÇÃO
```

A Mesa termina quando o Diretor manda executar ou cancelar.

## Ficção

Depois da confirmação:

```text
Cadeiras exercem autoria no espaço aberto
→ Narrador cruza fatos, intenções e Direção
→ consequência é estabelecida
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

# Autoridades principais

```text
DIRETOR
→ conduz a obra e pode deixar aberto, alinhar ou determinar.

CADEIRA
→ autoria voluntária de uma personagem dentro do espaço aberto.

EXECUTOR
→ humano, IA ou outro participante que opera uma autoridade.

NARRADOR / JUIZ
→ cruza fatos, intenções, capacidades e Direção; sentencia e narra.

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

Se ainda não existe uma campanha/história, siga:

```text
regras-basicas/10-INICIAR-HISTORIA-COM-IA.md
```

No W4D, `campanha` é apenas o nome técnico do espaço persistente da obra. Ela pode ou não ser um RPG.

A estrutura mínima recomendada continua:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Modelos estão em:

```text
regras-basicas/modelos/
```

---

# Retomar uma história

Para continuar uma obra existente:

```text
campanha README
→ direcao.md
→ estado.md
→ fichas relevantes
→ módulos ativos
→ reancorar
→ identificar primeiro ponto aberto
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

> **Propor para ouvir. Julgar para entender. Determinar para fechar. Executar para existir. Registrar para preservar.**
