# Fontes da Campanha

Status: CANÔNICO DA REFORMULAÇÃO

Este arquivo define **onde salvar cada tipo de verdade** dentro de `campanhas/<nome>/`.

> **Cada verdade deve ter uma fonte principal.**

## Regra de roteamento

```text
QUEM É A PERSONAGEM E O QUE ELA PRECISA LEVAR CONSIGO?
→ personagens/<nome>.md

SOBRE O QUE A CAMPANHA É AO LONGO DAS TEMPORADAS?
→ mestre/narrativa.md

QUAL É O ARCO ATIVO?
→ mestre/roteiro.md

COMO A CAMPANHA ESTÁ AGORA?
→ estado/atual.md

O QUE É VERDADE ESTÁVEL DO CENÁRIO?
→ mundo/

O QUE O OUTRO LADO DA TRAMA ESTÁ FAZENDO?
→ opositor/

O QUE REALMENTE ACONTECEU?
→ livro/
```

## `personagens/`

Guarda as fichas reais.

A ficha pode conter:

```text
identidade
Descrição Física
Conceito
Habilidades e Conhecimentos
Traços e Poderes
Equipamentos e Recursos relevantes
Descrição Emocional / Personalidade
relações
Histórico
Estado Atual pessoal
```

O bloco `Estado Atual` da ficha é apenas o recorte pessoal temporário daquela personagem.

A ficha não é diário completo nem cópia do Estado global.

## Conhecimento relevante

Quando esquecer uma informação provavelmente faria a personagem interpretar ou decidir de forma incoerente, consolidar esse conhecimento na própria ficha ou na fonte específica apropriada.

```text
PERSONAGEM A SABE
≠
PERSONAGEM B SABE
```

Arquivos tecnicamente acessíveis não concedem conhecimento ficcional automático.

## Relações e ponto de vista

Relações registradas na ficha pertencem ao ponto de vista íntimo daquela personagem.

```text
FICHA DE A
→ como A entende o vínculo.

FICHA DE B
→ como B entende o vínculo.
```

As leituras podem divergir sem que uma esteja errada.

## `estado/atual.md`

É a fonte canônica global da realidade presente.

Pode registrar, quando necessário:

```text
momento e local
quem está presente
posição das peças
condições temporárias
efeitos ativos
transformações em curso
Equipamentos ou Recursos indisponíveis
intenções persistentes
ações interrompidas
processos e prazos próximos
fatos recentes que ainda alteram a situação
primeiro ponto ainda aberto
```

Não registrar `Vida`, `Mente` ou `Mana` como estruturas universais.

```text
RECURSO OU CONDIÇÃO ESPECÍFICA FOI DEFINIDO
→ acompanhar conforme sua própria regra.

NADA DEFINIU
→ não inventar barra, reserva ou trilho genérico.
```

## `mundo/`

Guarda verdades estáveis externas às personagens.

Exemplos:

```text
localização de uma cidade
regra política estabelecida
organização existente
característica permanente de um local
evento que alterou duradouramente o cenário
```

Não usar `mundo/` para estados temporários pessoais nem planos secretos adversariais.

## `mestre/`

### `mestre/narrativa.md`

Fonte da identidade persistente da campanha:

```text
foco
gênero e tom
experiência desejada
temas e conflitos recorrentes
o que não deve dominar
premissas gerais
```

### `mestre/roteiro.md`

Fonte da temporada ativa:

```text
problema estrutural
Diretriz Fechada
processos preparados
limites do arco
condição de encerramento
```

O roteiro não determina decisões voluntárias nem resultados futuros.

### `mestre/temporadas/`

Guarda roteiros de temporadas encerradas.

## `opositor/`

Guarda oposição sem cadeira própria e processos adversariais legitimamente existentes.

Pode conter:

```text
objetivos
planos
preparação
prazos
conhecimento adversarial
recursos disponíveis
processos em andamento
```

Plano não é acontecimento.

## `livro/`

Guarda o histórico canônico do que efetivamente aconteceu.

Não registrar como acontecimento:

```text
intenção ainda não executada
hipótese
plano futuro
metaconversa
versão anulada
resultado ainda aberto
```

Temporadas encerradas seguem `arquivo-de-temporada.md`.

## Duplicação legítima

Uma mesma realidade pode aparecer em mais de uma fonte quando cada ocorrência possui função diferente.

Exemplo:

```text
LIVRO
→ registra que a personagem sofreu um ferimento.

ESTADO DA CAMPANHA
→ registra que o ferimento continua presente.

FICHA / ESTADO ATUAL PESSOAL
→ registra somente o recorte necessário para aquela cadeira.
```

Outro:

```text
LIVRO
→ registra que Ravena descobriu um fato.

FICHA DE RAVENA
→ preserva o conhecimento que ela precisa continuar possuindo.
```

Duplicação funcional não significa autoridade concorrente.

## Vida, Mente, Mana e outros mecanismos antigos

Os arquivos legados podem mencionar estruturas antigas, mas as fontes de campanha novas não devem tratá-las como padrão.

```text
Vida universal
Mente universal
Mana universal
→ não fazem parte do modelo ativo.
```

Se uma campanha ou personagem possuir uma condição, reserva, carga, transformação ou custo particular realmente estabelecido, registrar o elemento específico em sua fonte correta.

Exemplos:

```text
Condição: envenenado até receber antídoto.

Recurso: 2 cargas restantes do artefato.

Limitação: voo indisponível enquanto as asas estiverem feridas.
```

> **A fonte registra a verdade concreta; não converte toda verdade em uma estatística universal.**

## Evitar cópia sem função

Não repetir por padrão:

```text
cena inteira no Estado
ficha inteira no README
segredos em vários arquivos
todo o Livro na ficha
toda a lore do mundo em cada personagem
todo plano do Opositor no Estado
Narrativa inteira dentro do Roteiro
```

Quando uma fonte principal já basta, consultar essa fonte quando necessário.

## Regra final

> **Escolha a fonte pela função da verdade: ficha guarda a personagem; Narrativa guarda a identidade da campanha; Roteiro guarda o arco ativo; Estado guarda o presente global; mundo guarda contexto estável; Opositor guarda oposição legítima; Livro guarda o que aconteceu. Vida, Mente e Mana não são campos universais dessas fontes.**