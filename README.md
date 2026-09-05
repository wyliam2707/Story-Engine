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

A pasta `regras-basicas/` é a especificação operacional vigente.

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

O Diretor pode testar uma ideia, um resultado ou uma trajetória antes de colocá-la na Ficção.

```text
PROPOSTA OU QUESTÃO EM EXAME
→ Cadeiras envolvidas opinam
→ Narrador pode emitir PARECER
→ Diretor altera, cancela, deixa aberto ou fecha uma versão
```

Enquanto a Mesa estiver aberta:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO DA CADEIRA ≠ DECISÃO FICCIONAL
PARECER DO NARRADOR ≠ ACONTECIMENTO
```

A Mesa pode inclusive negociar uma versão:

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

Se um resultado materialmente importante continua aberto e não é evidente, o Narrador não escolhe secretamente um vencedor ou simula RNG invisível: a questão pode ir à Mesa.

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
→ espaço autoral onde propostas e resultados podem ser testados e alinhados.

NARRADOR
→ na Mesa pode emitir Parecer; na Ficção apresenta continuidade e consequências evidentes.

AUDITORIA
→ verifica fatos, coerência, autoridade e escopo sem governar o Diretor.
```

Uma única IA pode executar várias Cadeiras e o Narrador, mantendo os escopos separados.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

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

Não existe subsistema obrigatório de teste.

Quando o resultado importa, a Mesa pode discutir **qual resultado serve à obra e que condições o tornam plausível**.

Quando o Diretor o fecha, as Cadeiras executam o caminho e o Narrador apresenta.

---

# Ruptura deliberada

Uma Cadeira pode dizer:

```text
"eu normalmente não faria isso."
```

Essa objeção informa o Diretor.

Se ele reconhece a ruptura como deliberada e autoriza a execução:

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
→ realidade atual da Ficção.

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

Quando duas leituras parecerem competir, use a fonte normativa específica e abra Auditoria se necessário.

---

## Lema

> **Aprender antes de operar. Escolher antes de criar ou retomar. Propor para ouvir. Alinhar para construir. Determinar para fechar. Narrar para existir. Registrar para preservar.**