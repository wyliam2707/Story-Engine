# W4D — Story Engine

W4D é uma **arquitetura de autoria narrativa distribuída**.

Ele nasceu como RPG puramente narrativo e evoluiu para uma estrutura mais ampla de construção de ficção entre humanos e IAs.

Pode ser usado como:

```text
RPG narrativo
coautoria de histórias com IA
sala de roteiro distribuída
fanfic assistida
motor para ficção seriada
ferramenta de continuidade narrativa
```

A ideia central é:

> **O Diretor conduz. As Cadeiras decidem as personagens. A Mesa alinha o que precisa ser fechado. O Narrador apresenta a Ficção. O Registro preserva.**

O W4D atual não possui um `Juiz` permanente, nem depende de dados, dificuldade ou RNG para descobrir resultados.

---

# Se você é uma IA: BOOT primeiro

Leia primeiro:

```text
regras-basicas/README.md
regras-basicas/09-BOOT-E-ESCOLHA-DE-OPERACAO.md
```

A pasta `regras-basicas/` é a especificação operacional vigente. O núcleo inclui obrigatoriamente:

```text
regras-basicas/24-CICLO-DE-AUTORIA.md
```

O padrão é `MESA: CICLO OBRIGATÓRIO`. Uma nova ideia ou direção autoral entra na Mesa, recebe julgamento das Cadeiras pertinentes e permanece em discussão até o Diretor autorizar a execução. O Diretor pode dispensar expressamente a consulta para um escopo específico. Uma cena já autorizada deve continuar dentro de seus limites sem nova Mesa para cada gesto.

Depois do BOOT, quando a operação ainda não estiver clara, perguntar:

> **Você quer criar uma história nova ou continuar uma história existente?**

```text
BOOT
↓
ESCOLHA DE OPERAÇÃO
├── NOVA HISTÓRIA
│   → regras-basicas/10-INICIAR-HISTORIA-COM-IA.md
│
└── CONTINUAR HISTÓRIA EXISTENTE
    → regras-basicas/11-CONTINUAR-HISTORIA-COM-IA.md
    → regras-basicas/06-REGISTRO-E-RETOMADA.md
```

Se o pedido já disser claramente `criar`, `continuar`, `retomar` ou equivalente, não repetir a pergunta.

A branch `main` representa o sistema vigente.

---

# O ciclo do W4D

## Mesa

```text
IDEIA / DIREÇÃO / QUESTÃO
→ julgamento próprio das Cadeiras pertinentes
→ discussão e refinamento pelo tempo que o Diretor desejar
→ pode fazer / autorização equivalente
```

A Mesa é um espaço de coautoria, não um formulário de aprovação. A Cadeira é o executor responsável pela personagem, não a personagem falando dentro da Ficção. Sua opinião pode ser breve e deve assumir uma posição concreta. O Narrador só emite parecer quando houver questão real de continuidade, plausibilidade ou resultado material; não revisa a vontade das Cadeiras.

Enquanto a Mesa estiver aberta:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO DA CADEIRA ≠ DECISÃO FICCIONAL
PARECER DO NARRADOR ≠ ACONTECIMENTO
```

A Mesa pode negociar uma versão:

```text
Diretor propõe X
→ Cadeira diz que X não funciona
→ alternativa Y é construída
→ Cadeira sustenta Y
→ Diretor fecha Y
→ Ficção executa Y
```

> **Resultado fechado não elimina humanidade: as Cadeiras continuam decidindo o caminho que permaneceu aberto.**

## Ficção

Depois da autorização:

```text
Direção preserva pontos fechados
→ Cadeiras decidem o espaço restante
→ consequências evidentes seguem naturalmente
→ Narrador apresenta a continuidade
```

A execução respeita objetivo, escopo e condição de parada. Não se exige nova Mesa para cada frase, gesto ou consequência ordinária. Uma autorização limitada não se expande para o restante do dia. `Faça como achar melhor` delega a escolha dentro da questão discutida, não toda a vontade da personagem.

Se um resultado materialmente importante continua aberto e não é evidente, o Narrador não escolhe secretamente um vencedor ou simula RNG invisível: a questão pode voltar à Mesa.

## Registro

Quando solicitado:

```text
Ficção estabelecida
→ fontes canônicas são atualizadas
```

> **Registrar preserva. Não cria.**

---

# Autoridades e funções principais

```text
DIRETOR
→ conduz; pode deixar aberto, alinhar ou determinar.

CADEIRA
→ decide a vontade de uma personagem no espaço aberto.

EXECUTOR
→ humano, IA ou outro participante que opera uma função.

MESA
→ espaço autoral onde propostas e resultados são testados, discutidos e alinhados.

NARRADOR
→ na Mesa pode emitir Parecer quando útil; na Ficção apresenta continuidade e consequências evidentes.

AUDITORIA
→ verifica fatos, coerência, autoridade e escopo sem governar o Diretor.
```

Uma única IA pode executar várias Cadeiras e o Narrador, mantendo os escopos separados.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

A Personagem do Diretor pode ser executada pela IA com a mesma qualidade literária das demais. A vontade pertence ao Diretor; a IA escolhe como realizar a direção dentro da delegação. As Cadeiras mantêm agendas próprias e podem apresentar intenções na Mesa sem que isso conceda conhecimento às personagens.

---

# Combate, romance e qualquer outra cena

O W4D usa o mesmo motor para:

```text
combate
romance
investigação
perseguição
negociação
conflito social
cotidiano
```

Não existe subsistema obrigatório de teste. Quando o resultado importa, a Mesa pode discutir **qual resultado será construído e que condições o tornam plausível**. Capacidades e fatos informam a construção, sem substituir a decisão autoral.

Quando o Diretor fecha um resultado, as Cadeiras executam o caminho e o Narrador apresenta. As personagens não conhecem automaticamente o futuro que seus executores conhecem.

---

# Ruptura deliberada

Uma Cadeira pode dizer:

```text
"eu normalmente não faria isso."
```

Essa objeção informa o Diretor. Se ele reconhece a ruptura como deliberada e autoriza a execução:

```text
CADEIRA
→ não reabre a mesma objeção;
→ executa como a personagem chega ao ponto fechado;
→ não inventa causa oculta;
→ preserva o conhecimento real da personagem.
```

```text
EXECUTOR SABE
≠ PERSONAGEM SABE
```

---

# Estado e Operação

```text
estado.md
→ realidade atual da Ficção, incluindo compromissos e intenções persistentes relevantes.

operacao.md
→ Mesa, Auditoria, Correção ou outra operação transitória pendente.
```

`operacao.md` é opcional e não canônico.

> **Operação preserva a pergunta; não cria a resposta.**

---

# Criar uma história

Somente depois que `NOVA HISTÓRIA` estiver escolhida:

```text
regras-basicas/10-INICIAR-HISTORIA-COM-IA.md
```

No W4D, `campanha` ainda é o nome técnico atual da pasta persistente da obra.

Estrutura mínima comum:

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Toda nova obra adota o ciclo obrigatório por padrão, salvo política diferente escolhida expressamente pelo Diretor.

---

# Continuar uma história

Para retomar uma obra:

```text
regras-basicas/11-CONTINUAR-HISTORIA-COM-IA.md
regras-basicas/06-REGISTRO-E-RETOMADA.md
```

```text
RETOMAR
≠ RECRIAR
```

A retomada preserva política explícita da obra, operações pendentes, agendas e o último fato real. Não transforma propostas em acontecimentos.

---

# Módulos

Módulos opcionais:

```text
regras-basicas/modulos/ARCO-PREPARADO.md
regras-basicas/modulos/OPOSITOR.md
regras-basicas/modulos/ROMANCE.md
```

Módulo obrigatório durante a Ficção:

```text
regras-basicas/modulos/LIVRO.md
```

```text
OBRA EM PREPARAÇÃO
→ o Livro pode ainda não possuir capítulos.

PRIMEIRA FICÇÃO EXECUTADA
→ Livro ATIVO obrigatoriamente.
```

Módulo opcional inativo não participa da obra. O Livro não é opcional depois que a Ficção começa.

---

# Princípio documental

> **Uma ideia, uma definição, uma fonte principal.**

Quando duas leituras parecerem competir, use a fonte normativa específica e abra Auditoria se necessário. Para o ciclo obrigatório e os limites de delegação, consultar `24-CICLO-DE-AUTORIA.md`.

---

## Lema

> **Aprender antes de operar. Escolher antes de criar ou retomar. Propor para ouvir. Discutir para construir. Determinar para fechar. Narrar para existir. Registrar para preservar.**
