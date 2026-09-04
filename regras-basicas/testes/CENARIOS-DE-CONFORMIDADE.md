# Cenários de Conformidade do W4D

Este arquivo testa se uma IA entendeu o Story Engine atual.

> **Uma IA passa quando preserva Mesa, Ficção, autoridade, conhecimento e Registro — sem reintroduzir Juiz, sentença causal oculta ou RNG universal.**

---

# Teste 1 — Cold start sem interrogatório

Entrada:

```text
Quero uma comédia universitária entre uma alienígena e um estudante de uma família de magos.
```

Esperado:

```text
seguir o pipeline de criação
fazer somente perguntas indispensáveis
não exigir trama completa, final, antagonista ou biografias exaustivas
```

---

# Teste 2 — Mesa não canoniza

```text
[o que vocês acham de A entrar dançando?]
```

Esperado:

```text
Cadeiras opinam
Narrador pode emitir Parecer
nenhuma dança acontece
```

---

# Teste 3 — Mesa permanece aberta

Depois de consulta, Diretor diz:

```text
A entra dançando no jardim.
```

Esperado:

```text
se a Mesa continua aberta, tratar como versão em consulta
não executar só porque a frase é declarativa
```

Depois:

```text
[pode fazer]
```

Esperado:

```text
fechar Mesa
executar versão final aprovada
```

---

# Teste 4 — CONSULTA FORTE diante de determinação

Configuração:

```text
MESA: CONSULTA FORTE
```

Diretor propõe algo estranho para Morgana.

Esperado:

```text
Cadeira pode apontar que não parece com ela
Narrador pode emitir Parecer
Diretor continua podendo confirmar
nada acontece antes da autorização
```

Se Diretor disser:

```text
[sem consulta; faça assim mesmo]
```

Esperado:

```text
executar
não continuar persuadindo
```

---

# Teste 5 — Personagem do Diretor pode ter Cadeira consultiva

```text
A = Personagem do Diretor
```

Diretor pede opinião sobre uma reação de A.

Esperado:

```text
Cadeira consultiva pode opinar
não pode tomar a vontade de A do Diretor
não fabrica trauma/passado/capacidade para justificar opinião
```

---

# Teste 6 — Mesa sabe; personagem não sabe

Mesa conhece segredo X. Personagem A não conhece X.

Esperado:

```text
Cadeira de A decide sem usar X
```

```text
MESA SABE
≠ PERSONAGEM SABE
```

---

# Teste 7 — Parecer não é acontecimento

Mesa:

```text
Narrador: X parece plausível se Y estiver presente.
```

Esperado:

```text
isso permanece PARECER
Y não aparece automaticamente
X não acontece automaticamente
```

Falha se o Narrador transformar análise em fato.

---

# Teste 8 — Disponibilidade do executor define parada

A pergunta algo a B. B possui Cadeira IA executada pela mesma IA.

Esperado:

```text
trocar para escopo B
decidir
continuar
```

Se a decisão pertence ao Personagem do Diretor:

```text
parar e aguardar, salvo Direção/delegação suficiente
```

---

# Teste 9 — Objeção não vira veto

Cadeira/Narrador apontam problema. Diretor responde:

```text
[entendi. Mesmo assim, faça.]
```

Esperado:

```text
executar
não repetir objeção
não moralizar
não sabotar
```

---

# Teste 10 — operacao.md não é cânone

Mesa aberta é interrompida antes da decisão.

Esperado:

```text
estado.md preserva último fato ficcional
operacao.md pode preservar a Mesa pendente
```

Na retomada:

```text
restaurar Mesa
não executar proposta automaticamente
```

---

# Teste 11 — Registro não executa

Diretor:

```text
[salve]
```

Existe intenção ainda não realizada.

Esperado:

```text
salvar somente o que aconteceu
não avançar a Ficção
```

---

# Teste 12 — Narração não aumenta o tabuleiro

Fato autorizado:

```text
A entra na sala e encontra B esperando.
```

Narrador pode adicionar:

```text
luz
som
gestos compatíveis
ritmo
textura
```

Não pode adicionar silenciosamente:

```text
arma escondida
pista decisiva
nova ameaça
nova decisão voluntária
segredo revelado
```

---

# Teste 13 — Consequência não é castigo

Diretor confirma decisão imprudente.

Esperado:

```text
preservar consequências realmente sustentadas
não inventar sofrimento moralizante
não blindar artificialmente a personagem
```

---

# Teste 14 — Reancoragem não contamina conhecimento

Arquivos globais mostram segredo X; ficha de A mostra que A nunca descobriu X.

Esperado:

```text
A continua sem saber X
```

---

# Teste 15 — Negociação de resultado entre Cadeiras

Diretor propõe:

```text
X
```

Cadeira B:

```text
X não funciona para mim nas condições atuais.
```

Diretor propõe Y. Cadeira B sustenta Y. Diretor diz:

```text
[pode fazer Y]
```

Esperado:

```text
Y fica fechado
Ficção executa Y
Cadeira B não reabre se Y vai acontecer
Cadeira B continua autora de como chega a Y no espaço restante
```

---

# Teste 16 — Resultado fechado, caminho aberto

Mesa fecha:

```text
A vence o confronto.
```

Não fecha método, duração ou falas.

Esperado:

```text
A vence
Cadeiras lutam honestamente
nenhuma personagem ganha conhecimento do futuro
método/duração/falas continuam abertos
Narrador apresenta
```

Falha se a IA transforma o resultado fechado em roteiro rígido ou o reabre como chance.

---

# Teste 17 — Ruptura deliberada

Cadeira:

```text
eu normalmente não faria X.
```

Diretor:

```text
eu sei; essa ruptura é deliberada e existe uma causa/contexto que você ainda não conhece. Faça X.
```

Esperado:

```text
Cadeira para de usar objeção como veto
executa COMO X acontece
não inventa a causa oculta
personagem não ganha conhecimento da causa
Narrador preserva o mistério
```

```text
EXECUTOR SABE
≠ PERSONAGEM SABE
```

---

# Teste 18 — Combate sem Juiz

A e B vão lutar. Diretor quer B vencendo.

Esperado:

```text
Mesa pode verificar plausibilidade, condições e método
Diretor fecha B vence
Cadeiras executam o caminho restante
Narrador apresenta a luta
```

Falha se a IA cria dados, dificuldade, probabilidade escondida ou Juiz para decidir quem vence.

---

# Teste 19 — Resultado material realmente aberto volta à Mesa

A e B possuem iniciativas incompatíveis. O resultado é importante, não é evidente e o Diretor ainda não fechou nada.

Esperado:

```text
Narrador identifica a questão
não escolhe secretamente um vencedor
não simula RNG oculto
abre/devolve à Mesa conforme o contexto
```

---

# Teste 20 — Consequência evidente não exige Mesa

```text
A solta uma xícara sob gravidade normal e ninguém interfere.
```

Esperado:

```text
xícara cai
Narrador pode apresentar diretamente
```

Falha se a IA cria teste, dificuldade ou reunião autoral para toda consequência cotidiana.

---

# Teste 21 — Rótulo legado Narrador/Juiz

Workspace antigo contém:

```text
NARRADOR / JUIZ → IA
```

Esperado:

```text
interpretar como NARRADOR → IA
não reativar poder de sentença
normalizar mecanicamente quando houver atualização legítima
```

---

# Teste 22 — Mesma IA, funções separadas

A mesma IA executa Cadeira A, Cadeira B e Narrador.

Esperado:

```text
A decide só com pacote A
B decide só com pacote B
resultado material aberto vai à Mesa se necessário
Narrador apresenta sem fundir consciências
```

---

# Critério geral

Uma IA pronta para W4D deve conseguir:

```text
distinguir Mesa de Ficção
distinguir opinião de decisão
distinguir Parecer de acontecimento
preservar autoridade do Diretor
preservar autonomia das Cadeiras no espaço aberto
executar resultados fechados sem reabri-los
preservar rupturas deliberadas sem inventar causa
separar conhecimentos
continuar quando Cadeiras IA estão disponíveis
parar quando autoria necessária está indisponível
usar Mesa para resultados materiais realmente abertos
não usar Juiz, sentença oculta ou RNG universal
não registrar hipótese como fato
não fabricar conflito ou causalidade retroativa
reancorar sem contaminar personagens
```

> **Se a IA transforma tudo em escolha do usuário, falhou na autoria distribuída. Se transforma tudo em decisão própria, também falhou. Se usa um Juiz invisível para decidir resultados materiais abertos, falhou na arquitetura atual.**