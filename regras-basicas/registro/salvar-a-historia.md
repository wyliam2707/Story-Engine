# Salvar a História

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define **como salvar a campanha sem continuar jogando**.

> **Salvar preserva. Não cria.**

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
```

Se nada precisa sobreviver à resposta, não criar registro por obrigação.

## Procedimento básico

```text
1. PARAR no último fato estabelecido.
2. IDENTIFICAR o que realmente mudou.
3. SEPARAR personagem, passado, presente, mundo e processos.
4. ESCOLHER a fonte principal correta.
5. ATUALIZAR somente os arquivos afetados.
6. NÃO avançar a ficção durante o salvamento.
```

## O que nunca deve ser promovido a fato

Não salvar como realidade concluída:

```text
intenção ainda não executada
ação ainda não julgada
hipótese
suspeita como certeza
plano futuro como acontecimento
segredo como conhecimento de quem não o descobriu
resultado que ainda depende de uma nova decisão
```

## Salvar no meio da cena

O usuário pode pedir para salvar em qualquer ponto.

Nesse caso:

```text
NÃO terminar a cena.
NÃO criar despedida.
NÃO concluir conflito pendente.
NÃO escolher a próxima ação humana.
```

Registrar o último estado fechado e deixar explícito o que continua aberto.

Exemplo:

```text
Local: corredor da mansão
Situação: Corvin abriu a porta da biblioteca
Ravena está do outro lado
Próxima decisão humana ainda não foi declarada
```

## Processos fora de cena

Quando uma ação estabelecida cria um processo longo, registrar:

```text
PROCESSO
RESPONSÁVEL, quando pertinente
ESTADO
PRAZO, quando existir
RESULTADO FUTURO já estabelecido, se houver
```

Exemplo:

```text
Processo: investigação de Dick
Estado: em andamento
Prazo: primeiras pistas em 10 dias
```

Não é necessário reencenar Dick a cada janela para o processo continuar.

## Conhecimento adquirido

Se uma personagem aprende algo que deverá influenciar decisões futuras, consolidar na ficha quando necessário.

```text
SE ESQUECER PROVAVELMENTE GERARIA INTERPRETAÇÃO INCOERENTE
→ ficha.

IMPORTA APENAS AGORA
→ Estado Atual, se ainda pertinente.

CONTEXTO EXTERNO JÁ PRESERVADO
→ consultar a fonte externa quando necessário.
```

Não copiar automaticamente para outras personagens.

## Evolução da personagem

Quando uma mudança realmente se torna duradoura, atualizar o bloco estável apropriado da ficha.

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

Emoção momentânea não deve reescrever a ficha permanente.

## Mudança de Estado

Condições presentes entram, mudam e saem conforme a realidade.

```text
ANTES
→ braço fraturado.

DEPOIS DA RECUPERAÇÃO
→ condição removida do Estado.
```

O Livro continua preservando que o ferimento aconteceu quando isso for historicamente relevante.

### Sem trilhos universais

Não atualizar ou criar automaticamente:

```text
Vida
Mente
Mana
```

como reservas universais.

Esses mecanismos pertencem ao motor legado.

Se existir um recurso, custo ou condição específica definida por ficha, Poder, Traço, Equipamento ou regra canônica, acompanhar **essa coisa específica**.

Exemplo:

```text
Artefato: 2 cargas restantes.

Condição: exausto após sustentar o ritual.

Limitação: teleporte indisponível até o amanhecer.
```

> **Persistir a verdade concreta, não reconstruir a barra antiga.**

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
mudanças consolidadas da personagem
conhecimento relevante
processos e prazos
mudanças estáveis do mundo
oposição ainda viva
```

Capítulos podem consolidar várias sentenças depois.

# Fechar temporada

O fechamento de temporada começa somente quando a condição de encerramento registrada no roteiro foi realmente alcançada.

## 1 — Parar no resultado real

Não criar:

```text
nova ameaça para terminar com gancho
decisão futura das personagens
romance ainda não decidido
nova missão
próxima temporada
```

## 2 — Escrever o epílogo

O epílogo registra **como a temporada realmente terminou**.

Pode responder, conforme a campanha:

```text
onde as personagens terminaram?
quais relações mudaram?
que conhecimentos importantes foram adquiridos?
que objetivos foram concluídos?
que mudanças ficaram consolidadas?
que problemas realmente permanecem abertos?
```

> **Epílogo registra resultado. Não escolhe futuro.**

## 3 — Consolidar fontes

Atualizar somente o que realmente mudou:

```text
FICHAS
→ mudanças permanentes da personagem.

ESTADO
→ realidade presente deixada pelo encerramento.

MUNDO
→ mudanças estáveis.

OPOSITOR
→ processos ou planos ainda existentes.
```

## 4 — Arquivar roteiro

Mover o roteiro encerrado para:

```text
campanhas/<nome>/mestre/temporadas/temporada-[N].md
```

marcado como `ENCERRADA`.

## 5 — Perguntar “E agora?”

Depois do epílogo e da consolidação:

> **E agora?**

Problema aberto não é próximo arco obrigatório.

## Checklist

```text
[ ] salvei somente fatos já estabelecidos?
[ ] o Estado global representa o presente real?
[ ] condições e efeitos ativos foram atualizados?
[ ] Equipamentos e Recursos estão com disponibilidade correta?
[ ] conhecimento importante ficou com a personagem certa?
[ ] evolução consolidada atualizou a ficha correta?
[ ] processos e prazos continuam coerentes?
[ ] planos futuros não viraram acontecimentos?
[ ] removi condições que já terminaram?
[ ] não criei Vida, Mente ou Mana universais?
[ ] não avancei a ficção durante o salvamento?
```

Se for fechamento de temporada:

```text
[ ] condição de encerramento realmente alcançada?
[ ] epílogo descreve somente o resultado real?
[ ] fichas e Estado foram consolidados?
[ ] roteiro foi arquivado?
[ ] nenhuma nova temporada nasceu antes de “E agora?”?
```

## Regra final

> **Salvar a história é distribuir verdades já estabelecidas nas fontes corretas. O Livro preserva o passado, o Estado preserva o presente global e a ficha preserva a personagem. Vida, Mente e Mana não são recursos universais do salvamento; condições, custos e recursos só são acompanhados quando uma fonte canônica específica realmente os define.**