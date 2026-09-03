# 07 — Criar Campanha

Uma campanha precisa de poucas fontes para começar.

> **Nome e pasta definidos + Direção suficiente + autoridades definidas + personagens necessárias + Estado inicial = campanha pronta para jogar.**

## Passo 0 — Nome e pasta da campanha

Antes de escrever Direção, fichas, Estado ou qualquer outro artefato da campanha:

```text
1. definir um nome para a campanha;
2. derivar um slug estável para a pasta;
3. criar campanhas/<slug>/;
4. criar imediatamente campanhas/<slug>/README.md como arquivo-âncora.
```

Exemplo:

```text
Nome: Duas Vidas Normais
Slug: duas-vidas-normais
Pasta: campanhas/duas-vidas-normais/
```

Em sistemas como GitHub, uma pasta vazia não persiste. Por isso o `README.md` deve nascer junto com a campanha, ainda que inicialmente contenha apenas:

```text
# [NOME DA CAMPANHA]

STATUS
→ EM PREPARAÇÃO
```

Depois, no Passo 2, esse mesmo `README.md` recebe a configuração completa de autoridades e módulos.

> **Nenhum arquivo de campanha deve ser produzido sem um destino canônico já definido.**

Se o nome ainda não estiver decidido, resolver o nome antes de prosseguir. Um nome provisório só deve ser usado quando o Diretor aceitar explicitamente que ele é provisório.

## Estrutura mínima

```text
campanhas/<slug>/
├── README.md
├── direcao.md
├── estado.md
└── personagens/
```

Outras fontes são criadas somente quando houver necessidade real.

```text
mundo/
→ verdades externas estáveis que precisam persistir.

arco.md
→ somente se o módulo Arco Preparado for ativado.

oposicao.md
→ somente se o módulo Opositor for ativado.

livro/
→ somente se o módulo Livro for ativado; contém a obra registrada em capítulos.
```

## Passo 1 — Direção

Criar `direcao.md` **dentro da pasta já definida no Passo 0**.

Modelo mínimo:

```text
# Direção

## Proposta
[que tipo de história estamos escrevendo?]

## Foco
[o que deve receber atenção recorrente?]

## Tom
[quando relevante]

## Premissas
[fatos autorais gerais que sustentam a proposta]

## Direções Ativas
[deixar vazio no início se nada local estiver fechado]
```

A Direção não precisa prever a trama inteira.

Pode ser simples:

```text
"aventura urbana centrada na convivência entre três personagens e nos problemas que elas escolhem investigar"
```

O Diretor pode alterar e aprofundar a Direção durante a campanha.

## Passo 2 — Configuração de Autoridades

Atualizar o `README.md` criado no Passo 0.

Modelo:

```text
# [NOME DA CAMPANHA]

STATUS
→ EM PREPARAÇÃO

DIRETOR
Executor: [humano / IA / outro]

NARRADOR / JUIZ
Executor: [humano / IA / outro]

CADEIRAS
- Personagem A → Executor: HUMANO
- Personagem B → Executor: IA
- Personagem C → Executor: IA

MÓDULOS
- Arco Preparado: INATIVO
- Opositor: INATIVO
- Romance: [ATIVO / INATIVO conforme a proposta]
- Livro: INATIVO
```

Uma mesma pessoa ou IA pode executar várias funções. Isso não funde as autoridades.

Não registrar executor dentro da ficha da personagem.

## Passo 3 — Personagens

Criar somente as fichas necessárias para começar, seguindo `04-FICHA.md` e `modelos/FICHA.md`.

Todas as fichas da campanha devem ser salvas em:

```text
campanhas/<slug>/personagens/
```

Personagens secundárias podem receber ficha ou Cadeira depois se ganharem importância real.

A ficha precisa ser suficiente para que outro executor possa reconstruir a mesma pessoa sem depender da conversa de criação.

## Passo 4 — Estado inicial

Criar `estado.md`.

Modelo mínimo:

```text
# Estado

Momento:
Local:

## Presenças e posições
- ...

## Condições relevantes
- ...

## Intenções persistentes
- ...

## Processos e prazos
- ...

## Último fato estabelecido
- campanha ainda não iniciada.

## Primeiro ponto aberto
- abertura da primeira cena.
```

Não copiar fichas para o Estado.

## Passo 5 — Mundo necessário

Se a proposta depende de fatos externos estáveis antes do início, criar `mundo/` e registrar somente o que precisa ser verdade.

Não é necessário construir uma enciclopédia antes de jogar.

Detalhes neutros podem surgir por criação emergente durante a ficção.

## Passo 6 — Módulos opcionais

Ativar somente o que a campanha realmente usa.

### Arco Preparado

Seguir `modulos/ARCO-PREPARADO.md` e criar `arco.md`.

### Opositor

Seguir `modulos/OPOSITOR.md`, definir escopo no README da campanha e criar `oposicao.md` somente se houver informação persistente a registrar.

### Romance

Seguir `modulos/ROMANCE.md` quando esse foco fizer parte relevante da história.

### Livro

Seguir `modulos/LIVRO.md` quando a campanha quiser preservar a ficção jogada em capítulos.

Ao ativar o módulo, criar:

```text
livro/
└── README.md
```

O `README.md` do Livro funciona como índice da obra. Cada vez que `fechar o capítulo` for usado, um novo arquivo numerado é salvo dentro de `livro/` e o índice é atualizado.

O Livro contém a ficção canonizada — narração, falas, ações e pensamentos estabelecidos — e não contém Direção, consultas, auditorias, instruções de cena ou outras metaconversas.

## Passo 7 — Auditoria de início

Antes de começar, confirmar:

```text
[ ] A campanha possui nome definido.
[ ] A pasta canônica campanhas/<slug>/ existe e contém README.md.
[ ] Todos os arquivos da campanha estão sendo gravados dentro dessa pasta.
[ ] Sei quem é o Diretor.
[ ] Sei quem executa o Narrador.
[ ] Cada personagem inicial possui Cadeira e executor definidos.
[ ] direcao.md é suficiente para reconhecer a proposta.
[ ] cada ficha é autossuficiente.
[ ] estado.md representa o ponto inicial.
[ ] somente módulos realmente usados estão ativos.
[ ] se Livro estiver ativo, livro/README.md existe como índice.
[ ] fatos secretos necessários já possuem fonte legítima.
```

Quando a preparação estiver concluída, atualizar no `README.md`:

```text
STATUS
→ PRONTA PARA JOGAR
```

## START

Depois da preparação:

```text
START
→ reancorar o estado mínimo
→ abrir a primeira cena
→ deixar Cadeiras e mundo produzirem a ficção dentro da Direção.
```

O Diretor não precisa fornecer a primeira ação. Uma Cadeira pode iniciar algo legitimamente assim que a situação oferecer espaço.

## Retomar campanha existente

Quando uma campanha já existe:

```text
localizar a pasta canônica da campanha
→ README da campanha
→ direcao.md
→ estado.md
→ fichas relevantes
→ módulos ativos pertinentes
→ reancorar conforme 06-REGISTRO-E-RETOMADA.md
→ continuar.
```

Não pedir novamente informação que já está registrada.

## Regra final

> **Nomeie e ancore a campanha antes de escrevê-la. Depois, crie somente as fontes necessárias para a história existir agora. Direção define a proposta; configuração define as autoridades; fichas definem as pessoas; Estado define o presente. Quando ativo, o Livro preserva a ficção passada em capítulos. O restante entra apenas quando cumprir função real.**