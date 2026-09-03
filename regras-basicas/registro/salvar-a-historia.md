# Salvar a História

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define **como salvar a campanha sem continuar jogando**.

> **Salvar preserva. Não cria. Direção pendente é preservada como Direção, não como acontecimento.**

## Quando registrar

O Registro pode ser atualizado em quatro escalas:

```text
DEPOIS DE UMA SENTENÇA
→ registrar somente mudanças que precisam persistir imediatamente.

SALVAR ESTADO
→ preservar o ponto atual para retomada.

FECHAR CAPÍTULO
→ consolidar o trecho no Livro e atualizar fontes afetadas.

FECHAR TEMPORADA
→ consolidar o arco, escrever epílogo, atualizar fontes e arquivar roteiro.
```

## Depois de uma sentença

Perguntar somente:

```text
algo mudou de forma persistente?
alguém aprendeu algo que precisa ser lembrado?
uma relação mudou de modo consolidado?
uma condição ou efeito continua ativo?
um Equipamento ou Recurso mudou de disponibilidade?
um processo começou, terminou ou mudou?
um prazo foi criado ou alterado?
um fato estável do mundo mudou?
um plano legítimo do Opositor mudou?
existe Direção do Diretor ainda não consumada que precisa sobreviver ao contexto?
```

Se nada precisa sobreviver, não criar registro por obrigação.

## Procedimento básico

```text
1. PARAR no último fato estabelecido.
2. IDENTIFICAR o que realmente mudou.
3. IDENTIFICAR Direções ainda ativas, se houver.
4. SEPARAR personagem, passado, presente, mundo, processos e Direção.
5. ESCOLHER a fonte principal correta.
6. ATUALIZAR somente os arquivos afetados.
7. NÃO avançar a ficção durante o salvamento.
```

## O que nunca deve ser promovido a fato consumado

Não salvar como realidade concluída:

```text
intenção ainda não executada
ação ainda não julgada
hipótese
suspeita como certeza
plano futuro como acontecimento
Direção ainda não consumada como se já tivesse acontecido
segredo como conhecimento de quem não o descobriu
resultado ainda aberto
```

## Direções Autorais Ativas

Se uma Direção do Diretor ainda precisa ser cumprida depois do salvamento, preservá-la em fonte apropriada conforme `fontes-da-campanha.md`.

Normalmente, uma Direção local ainda ativa vai para:

```text
campanhas/<nome>/estado/atual.md
```

Registrar:

```text
Direção
Escopo fechado
O que permanece aberto
```

Exemplo:

```text
Direção: A perde o confronto atual.
Escopo fechado: resultado do confronto.
Permanece aberto: método, falas e decisões intermediárias.
```

Não executar a Direção durante o salvamento apenas para transformá-la em fato e evitar registrá-la como pendente.

Quando a Direção já foi consumada:

```text
→ registrar somente o acontecimento real.
→ remover a Direção da lista ativa.
```

## Salvar no meio da cena

O usuário pode pedir para salvar em qualquer ponto.

Nesse caso:

```text
NÃO terminar a cena.
NÃO criar despedida.
NÃO concluir conflito pendente.
NÃO escolher próxima ação.
NÃO consumir Direção pendente por conveniência.
```

Registrar último estado fechado e deixar explícito o que continua aberto.

## Processos fora de cena

Quando ação estabelecida cria processo longo, registrar:

```text
PROCESSO
RESPONSÁVEL, quando pertinente
ESTADO
PRAZO, quando existir
RESULTADO FUTURO já estabelecido, se houver
```

Plano permanece plano até acontecer.

## Conhecimento adquirido

Se uma personagem aprende algo que deverá influenciar decisões futuras, consolidar na ficha quando necessário.

```text
SE ESQUECER PROVAVELMENTE GERARIA INTERPRETAÇÃO INCOERENTE
→ ficha.

IMPORTA APENAS AGORA
→ Estado, se pertinente.
```

Não copiar automaticamente para outras personagens.

Direção do Diretor nunca vira conhecimento de personagem apenas porque está registrada no Estado global.

## Evolução da personagem

Quando mudança se torna duradoura, atualizar o bloco estável apropriado da ficha conforme `canonizacao-e-correcoes.md`.

Pode afetar:

```text
Personalidade
Desejos e objetivos
Medos e limites
Relações
Conhecimentos
Habilidades
Traços e Poderes
Equipamentos e Recursos
Histórico
```

Emoção momentânea não reescreve ficha permanente.

## Mudança de Estado

Condições presentes entram, mudam e saem conforme a realidade.

O Livro preserva acontecimentos historicamente relevantes depois que deixam de alterar o presente.

### Sem trilhos universais

Não atualizar ou criar automaticamente:

```text
Vida
Mente
Mana
```

como reservas universais.

Se existir recurso, custo ou condição específica, acompanhar essa coisa concreta.

## Planos do Opositor

Planos legitimamente existentes ficam em:

```text
campanhas/<nome>/opositor/
```

Registrar intenção, preparação, prazo, conhecimento e recursos realmente disponíveis.

Plano permanece plano até acontecer.

## O Livro

O Livro não precisa ser atualizado a cada sentença.

Durante a sessão, o mais importante é não perder:

```text
Estado Atual
Direções Autorais Ativas
mudanças consolidadas da personagem
conhecimento relevante
processos e prazos
mudanças estáveis do mundo
oposição ainda viva
```

Capítulos podem consolidar várias sentenças depois.

## Fechar temporada

O fechamento começa somente quando condição de encerramento realmente foi alcançada ou o Diretor explicitamente encerra/redefine o arco.

### 1 — Parar no resultado real

Não criar automaticamente:

```text
nova ameaça para terminar com gancho
decisão futura das personagens
romance ainda não decidido
nova missão
próxima temporada
```

### 2 — Escrever epílogo

O epílogo registra como a temporada realmente terminou.

Não consome Direções futuras que ainda não se realizaram.

### 3 — Consolidar fontes

Atualizar somente o que realmente mudou:

```text
FICHAS
ESTADO
MUNDO
OPOSITOR
DIREÇÕES PERSISTENTES, se alguma continuar além do arco por decisão do Diretor
```

### 4 — Arquivar roteiro

Mover roteiro encerrado para:

```text
campanhas/<nome>/mestre/temporadas/temporada-[N].md
```

### 5 — Perguntar “E agora?”

Problema aberto não é próximo arco obrigatório.

## Checklist

```text
[ ] salvei somente fatos já estabelecidos?
[ ] preservei Direções ainda ativas sem tratá-las como acontecimento?
[ ] removi Direções já consumadas?
[ ] o Estado global representa o presente real?
[ ] condições e efeitos foram atualizados?
[ ] conhecimento importante ficou com a personagem certa?
[ ] processos e prazos continuam coerentes?
[ ] planos futuros não viraram acontecimentos?
[ ] não criei Vida, Mente ou Mana universais?
[ ] não avancei a ficção durante o salvamento?
```

## Regra final

> **Salvar a história distribui verdades já estabelecidas nas fontes corretas e preserva Direções ainda ativas sem executá-las. O Livro guarda o passado, o Estado guarda o presente e limites autorais locais ainda pendentes, e a ficha guarda a personagem. Salvar nunca joga por conta própria.**