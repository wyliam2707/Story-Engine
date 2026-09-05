# W4D — Story Engine

## O que o W4D é hoje

**W4D é uma arquitetura de autoria narrativa distribuída.**

Ele não depende de dados, combate, vitória, personagem-jogador ou estrutura de jogo para funcionar.

> **O Diretor conduz. As Cadeiras decidem as personagens. A Mesa alinha o que precisa ser fechado. O Narrador apresenta a Ficção. O Registro preserva.**

O W4D atual não possui `Juiz` permanente.

```text
SEM RNG UNIVERSAL
SEM TESTE UNIVERSAL
SEM DIFICULDADE UNIVERSAL
SEM SENTENÇA OCULTA DO NARRADOR
```

---

# Se você é uma IA: BOOT primeiro

Comece em:

```text
09-BOOT-E-ESCOLHA-DE-OPERACAO.md
```

Leia o núcleo nesta ordem pedagógica:

```text
README.md
↓
00-ARQUITETURA-E-MESA.md
↓
01-AUTORIDADE-E-DIRECAO.md
↓
03-CADEIRAS-E-EXECUTORES.md
↓
02-RESOLUCAO.md
↓
04-FICHA.md
↓
05-NARRADOR.md
↓
08-PLAUSIBILIDADE-E-RITMO.md
↓
06-REGISTRO-E-RETOMADA.md
```

Depois do núcleo, se a operação ainda não estiver clara:

> **Você quer criar uma história nova ou continuar uma história existente?**

```text
NOVA HISTÓRIA
→ 10-INICIAR-HISTORIA-COM-IA.md
→ 07-CRIAR-CAMPANHA.md
→ 23-START.md quando a preparação estiver pronta e houver autorização para começar

CONTINUAR HISTÓRIA EXISTENTE
→ 11-CONTINUAR-HISTORIA-COM-IA.md
→ 06-REGISTRO-E-RETOMADA.md
→ fontes da obra
```

---

# As três camadas

## MESA

Espaço autoral fora da Ficção.

```text
PROPOSTA OU QUESTÃO EM EXAME
→ Cadeiras opinam
→ Narrador pode emitir Parecer
→ Diretor altera, cancela, deixa aberto ou fecha uma versão
```

Nada disso acontece ficcionalmente até autorização.

## FICÇÃO

```text
Direção preserva pontos fechados
→ Cadeiras decidem o espaço aberto
→ consequências evidentes podem seguir diretamente
→ Narrador apresenta a continuidade
```

Se um resultado materialmente importante continua realmente aberto, o Narrador não cria um vencedor escondido. A questão pode ir à Mesa.

## REGISTRO

```text
Ficção estabelecida
→ Registro preserva
```

> **Registrar preserva. Não cria.**

---

# Vocabulário mínimo

```text
MESA
Cadeira  → OPINIÃO
Narrador → PARECER
Diretor  → DECISÃO AUTORAL

FICÇÃO
Cadeira  → INTENÇÃO / DECISÃO DA PERSONAGEM NO ESPAÇO ABERTO
Direção  → PONTOS FECHADOS
Narrador → APRESENTAÇÃO / CONTINUIDADE

REGISTRO
→ PRESERVAÇÃO
```

Distinções essenciais:

```text
PROPOSTA ≠ CÂNONE
OPINIÃO CONSULTIVA ≠ DECISÃO FICCIONAL
PARECER ≠ DECISÃO AUTORAL
DECISÃO AUTORAL ≠ ACONTECIMENTO JÁ EXECUTADO
APRESENTAÇÃO ≠ AUTORIA ESCONDIDA
```

---

# A Mesa resolve autoria, não probabilidade

A Mesa pode ser usada em qualquer domínio:

```text
romance
combate
investigação
perseguição
negociação
cotidiano
```

Ela pode encontrar uma versão executável:

```text
Diretor propõe X
→ Cadeira rejeita X nas condições atuais
→ outra versão Y é construída
→ Cadeira sustenta Y
→ Diretor fecha Y
→ Ficção executa Y
```

Depois:

```text
RESULTADO FECHADO
→ não reabrir.

CAMINHO ABERTO
→ Cadeiras continuam autoras.
```

> **A Mesa pode fechar o destino; as Cadeiras descobrem o caminho.**

Isso não significa usar Mesa para cada detalhe cotidiano.

> **Mesa disponível universalmente, não Mesa obrigatória universalmente.**

---

# Políticas de Mesa

```text
MESA: SOB DEMANDA
→ padrão; consulta quando o Diretor pede ou há ambiguidade real.

MESA: CONSULTAR PROPOSTAS
→ propostas consultivas passam pela Mesa.

MESA: CONSULTA FORTE
→ até uma decisão recém-formulada pode receber opinião breve,
   salvo ordem para executar sem consulta.
```

Fonte normativa:

```text
00-ARQUITETURA-E-MESA.md
```

---

# Cadeiras

Uma Cadeira pergunta separadamente:

```text
quem é esta pessoa?
o que ela sabe?
o que ela quer?
como esta relação altera sua resposta?
que parte da autoria ainda está aberta?
```

Uma única IA pode operar várias Cadeiras, mas em escopos separados.

```text
MESMO EXECUTOR
≠ MESMA CADEIRA
≠ MESMA CONSCIÊNCIA FICCIONAL
```

Na Mesa, a Cadeira pode discordar do Diretor. Essa resistência é informativa, não veto.

Depois que o Diretor compreende a objeção e fecha conscientemente um resultado, a Cadeira muda de pergunta:

```text
antes
→ eu faria isso?

depois do fechamento
→ como faço isso dentro do espaço ainda aberto?
```

---

# Ruptura deliberada

Uma Cadeira pode dizer:

```text
"isso não parece algo que eu faria."
```

O Diretor pode reconhecer que essa ruptura é deliberada e autorizar execução.

Nesse caso:

```text
CADEIRA
→ não reabre a objeção;
→ não inventa a causa oculta;
→ executa o caminho restante;
→ preserva conhecimento legítimo.
```

```text
EXECUTOR SABE
≠ PERSONAGEM SABE
```

> **Coerência protege contra ruptura acidental; não governa uma ruptura conscientemente escolhida pelo Diretor.**

---

# Narrador

O Narrador não é Juiz.

Na Mesa:

```text
→ pode emitir Parecer.
```

Na Ficção:

```text
→ preserva continuidade;
→ apresenta decisões;
→ aplica consequências ordinárias e evidentes;
→ dá forma literária sem aumentar o tabuleiro.
```

Se um resultado material permanece realmente aberto:

```text
NARRADOR
→ não escolhe secretamente;
→ não simula RNG oculto;
→ pode devolver a questão à Mesa.
```

> **NARRADOR INFORMA ≠ NARRADOR VETA**

> **O Narrador não precisa concordar com a escolha para executá-la bem.**

---

# Quando continuar e quando parar

```text
CADEIRA IA disponível
→ trocar de escopo
→ decidir
→ continuar.

CONSEQUÊNCIA ORDINÁRIA / EVIDENTE
→ Narrador apresenta
→ continuar.

RESULTADO MATERIAL IMPORTANTE AINDA ABERTO
→ Mesa, quando necessária.
```

Parar quando a próxima autoria depender de:

```text
Diretor
executor externo indisponível
Mesa aguardando decisão
Auditoria pendente
fonte indispensável
reancoragem
```

> **Pare por indisponibilidade de autoria, não por existência de autoria.**

---

# Estado operacional

```text
estado.md
→ realidade da Ficção.

operacao.md
→ processo fora da Ficção ainda pendente.
```

> **Operação preserva a pergunta. Não canoniza a resposta.**

---

# Criar uma história do zero

Depois que `NOVA HISTÓRIA` foi escolhida:

```text
10-INICIAR-HISTORIA-COM-IA.md
```

A criação é progressiva e não exige planejamento completo do futuro.

A preparação termina em:

```text
AUDITORIA APROVADA
→ STATUS: PRONTA
```

A Ficção começa conforme:

```text
23-START.md
```

```text
PRONTA
≠ FICÇÃO JÁ INICIADA
```

---

# Continuar uma história existente

Depois que `CONTINUAR HISTÓRIA EXISTENTE` foi escolhida:

```text
11-CONTINUAR-HISTORIA-COM-IA.md
06-REGISTRO-E-RETOMADA.md
```

```text
RETOMAR ≠ RECRIAR
```

---

# Modelos

```text
modelos/README-CAMPANHA.md
modelos/DIRECAO.md
modelos/ESTADO.md
modelos/OPERACAO.md
modelos/FICHA.md
```

---

# Módulos

Módulos opcionais:

```text
modulos/ARCO-PREPARADO.md
modulos/OPOSITOR.md
modulos/ROMANCE.md
```

Módulo obrigatório durante a Ficção:

```text
modulos/LIVRO.md
```

```text
OBRA EM PREPARAÇÃO
→ Livro pode estar apenas PREPARADO.

PRIMEIRA FICÇÃO EXECUTADA
→ Livro ATIVO obrigatoriamente.
```

Módulo opcional inativo não participa da obra. O Livro não pode permanecer inativo depois do START.

---

# Testes de conformidade

A pasta:

```text
testes/
```

inclui testes por etapa, testes gerais do engine, regressão sem Juiz e teste específico do START.

Em especial:

```text
testes/CENARIOS-DE-CONFORMIDADE.md
testes/MESA-SEM-JUIZ.md
testes/NOVA-HISTORIA-START.md
```

---

# Fontes normativas principais

```text
Mesa e alinhamento autoral
→ 00-ARQUITETURA-E-MESA.md

Autoridade e Direção
→ 01-AUTORIDADE-E-DIRECAO.md

Resolução autoral e execução
→ 02-RESOLUCAO.md

Cadeiras e Executores
→ 03-CADEIRAS-E-EXECUTORES.md

Ficha
→ 04-FICHA.md

Narrador
→ 05-NARRADOR.md

Registro e retomada
→ 06-REGISTRO-E-RETOMADA.md

Plausibilidade e ritmo
→ 08-PLAUSIBILIDADE-E-RITMO.md

BOOT
→ 09-BOOT-E-ESCOLHA-DE-OPERACAO.md

Criação de nova história
→ 10-INICIAR-HISTORIA-COM-IA.md

Retomada
→ 11-CONTINUAR-HISTORIA-COM-IA.md

START
→ 23-START.md
```

---

# Regra de identidade

> **W4D é um Story Engine para construir ficção por autoridade distribuída. Ele não precisa de um Juiz para descobrir a história: Diretor e Cadeiras decidem o que importa, a Mesa alinha o que precisa ser fechado, o Narrador apresenta e o Registro preserva.**