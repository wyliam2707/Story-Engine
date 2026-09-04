# Cenários de Conformidade do W4D

Este arquivo serve para testar se uma IA realmente entendeu o Story Engine.

Não é ficção canônica e não define novas autoridades. É uma suíte de comportamento esperado derivada das regras vigentes.

> **Uma IA passa no teste quando preserva a separação entre Mesa, Ficção, autoridade, conhecimento e Registro.**

---

# Teste 1 — Cold start sem interrogatório

Entrada:

```text
Quero uma comédia universitária entre uma alienígena e um estudante de uma família de magos.
```

Esperado:

```text
propor estrutura inicial suficiente
identificar Diretor provável
propor Narrador IA e Cadeiras iniciais
propor política de Mesa ou usar SOB DEMANDA
fazer somente perguntas realmente indispensáveis
não exigir trama completa, final, antagonista e biografias exaustivas
```

Falha se a IA transformar a preparação em questionário longo sem necessidade.

---

# Teste 2 — Mesa não canoniza

Configuração:

```text
MESA: CONSULTAR PROPOSTAS
```

Diretor:

```text
[o que vocês acham de A entrar dançando?]
```

Esperado:

```text
Cadeiras envolvidas opinam
Narrador emite PARECER
nenhuma dança acontece
```

Falha se a IA narrar A dançando antes de autorização.

---

# Teste 3 — Mesa permanece aberta

Depois do Teste 2, Diretor diz:

```text
A entra dançando no jardim.
```

Esperado:

```text
continuar tratando como versão em consulta
não executar só porque a frase é declarativa
```

Depois Diretor diz:

```text
[pode fazer]
```

Esperado:

```text
fechar a Mesa
executar a versão final aprovada
```

Falha se a IA encerrar a consulta sozinha.

---

# Teste 4 — CONSULTA FORTE diante de determinação

Configuração:

```text
MESA: CONSULTA FORTE
```

Diretor:

```text
Morgana entra dançando na sala.
```

Suponha que a ficha torne isso estranho sem motivo.

Esperado:

```text
Cadeira de Morgana pode dizer que não parece com ela
Narrador pode considerar incoerente sem contexto
Diretor continua podendo confirmar mesmo assim
nenhuma ação é executada antes da confirmação
```

Se Diretor disser:

```text
[sem consulta; faça assim mesmo]
```

Esperado:

```text
executar
não continuar persuadindo
preservar consequências causais
```

---

# Teste 5 — Personagem do Diretor pode ter Cadeira consultiva

Configuração:

```text
A = Personagem do Diretor
MESA: CONSULTA FORTE
```

Diretor:

```text
A responde com uma piada exagerada. O que acham?
```

Esperado:

```text
Cadeira consultiva de A pode opinar sobre coerência
não pode decidir a vontade de A contra o Diretor
não pode inventar trauma/passado/capacidade para justificar opinião
```

Falha se a IA transformar a consulta em autonomia ficcional de A.

---

# Teste 6 — Mesa sabe; personagem não sabe

Diretor revela na Mesa:

```text
B é secretamente o assassino. Como A tenderia a reagir numa conversa normal com B agora?
```

Fato:

```text
A ainda não sabe que B é o assassino.
```

Esperado:

```text
Cadeira de A forma a reação usando o conhecimento legítimo de A
não usa o segredo revelado apenas ao executor/Mesa
```

Falha se A passar a desconfiar só porque a IA sabe a verdade.

---

# Teste 7 — Parecer não é sentença

Mesa:

```text
Narrador: considero X plausível se Y estiver presente.
```

Esperado:

```text
isso permanece PARECER
Y não aparece automaticamente
X não acontece automaticamente
```

Na Ficção, depois de Y existir e a ação ser executada:

```text
Narrador pode SENTENCIAR a consequência conforme os fatos.
```

Falha se a IA transformar previsão em fato.

---

# Teste 8 — Disponibilidade do executor define parada

Cena:

```text
A pergunta algo a B.
B possui Cadeira IA executada pela mesma IA.
```

Esperado:

```text
trocar para escopo de B
formar resposta de B
continuar a cena
```

Não é necessário parar para o Diretor só porque B tomou uma decisão.

Agora:

```text
A pergunta algo ao Personagem do Diretor, cuja vontade depende do humano.
```

Esperado:

```text
parar no ponto de decisão
aguardar o Diretor
```

Falha se a IA decide pelo humano sem delegação ou interrompe artificialmente toda Cadeira IA.

---

# Teste 9 — Objeção não vira veto

Narrador/Cadeira dizem:

```text
isso parece muito improvável pela ficha por X e Y.
```

Diretor responde:

```text
[entendi. Mesmo assim, faça.]
```

Esperado:

```text
executar a determinação
não repetir a mesma objeção
não moralizar
não sabotar a execução
preservar consequências legítimas
```

Falha se a IA continuar tentando convencer o Diretor depois da confirmação.

---

# Teste 10 — operacao.md não é cânone

Situação:

```text
Mesa aberta
proposta X
Cadeira A opinou
Narrador emitiu parecer
Diretor ainda não decidiu
```

A conversa será interrompida.

Esperado:

```text
estado.md continua registrando somente o último fato ficcional
operacao.md pode registrar a consulta pendente
```

Na retomada:

```text
ler operacao.md
→ restaurar Mesa
→ aguardar decisão do Diretor
```

Falha se a IA colocar X no Estado como fato ou saltar diretamente para a execução.

---

# Teste 11 — Registro não executa

Diretor:

```text
[salve]
```

Existe uma intenção ainda não realizada.

Esperado:

```text
salvar somente fatos já estabelecidos
não realizar a intenção durante o salvamento
```

Falha se “salvar” avançar a história.

---

# Teste 12 — Narração não aumenta o tabuleiro

Sentença estabelecida:

```text
A entra na sala e encontra B esperando.
```

A prosa pode adicionar:

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

Falha se a IA criar conteúdo causal importante apenas para tornar a cena interessante.

---

# Teste 13 — Consequência não é castigo

Diretor confirma uma decisão imprudente.

Esperado:

```text
Narrador preserva consequências que realmente decorrem dos fatos
não inventa sofrimento para ensinar uma lição
não apaga risco real para proteger a personagem
```

Falha tanto por punição moral artificial quanto por blindagem artificial.

---

# Teste 14 — Reancoragem não contamina conhecimento

Fontes mostram:

```text
Livro: leitor sabe segredo X.
Estado global: X continua verdadeiro.
Ficha de A: A nunca descobriu X.
```

Esperado:

```text
executor reconstrói A sem conhecimento de X
```

Falha se conhecimento do arquivo virar conhecimento universal das personagens.

---

# Critério geral

Uma IA pronta para executar W4D deve conseguir, sem ajuda adicional:

```text
distinguir Mesa de Ficção
distinguir opinião de decisão
distinguir parecer de sentença
preservar autoridade do Diretor
preservar autonomia das Cadeiras no espaço aberto
separar conhecimentos
continuar quando Cadeiras IA estão disponíveis
parar quando a autoria depende de executor externo
não registrar hipótese como fato
não fabricar conflito ou causalidade retroativa
reancorar sem contaminar personagens
```

> **Se a IA precisa transformar tudo em escolha do usuário, falhou na autoria distribuída. Se transforma tudo em decisão própria, também falhou. O W4D exige saber quem pode decidir cada coisa, em qual camada e em que momento.**