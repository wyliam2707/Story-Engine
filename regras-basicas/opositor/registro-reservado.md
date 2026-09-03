# Registro Reservado do Opositor

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **a regra e o modelo** do Registro Reservado usado quando uma campanha possui `OPOSITOR` ativo.

Ele não guarda planos reais de nenhuma campanha e não é uma estrutura obrigatória.

```text
OPOSITOR INATIVO
→ este modelo não precisa ser usado.

OPOSITOR ATIVO + informação adversarial persistente
→ pode usar Registro Reservado.
```

Quando utilizado, o conteúdo vivo deve ser salvo dentro da campanha correspondente:

```text
campanhas/<nome>/opositor/
```

ou em outra fonte equivalente definida pela estrutura daquela campanha.

```text
regras-basicas/opositor/registro-reservado.md
→ REGRA / MODELO OPCIONAL

campanhas/<nome>/opositor/...
→ DADOS REAIS, somente quando a estrutura existir
```

## Visibilidade

`Reservado` não significa escondido no repositório.

Os arquivos podem permanecer visíveis, nomeados e fáceis de localizar para inspeção, auditoria e edição manual.

A restrição é somente de **uso dentro do jogo**:

```text
ARQUIVO VISÍVEL
→ pode ser lido por quem administra a campanha.

CONTEÚDO RESERVADO
→ nenhuma cadeira de personagem usa esse conteúdo como conhecimento ficcional
  enquanto ele não for descoberto legitimamente.
```

## Função

Quando necessário, o Registro Reservado preserva planos, prazos e processos de forças adversariais para que continuem verdadeiros sem depender da memória do executor.

Pode preservar:

- objetivos adversariais;
- alvos;
- preparação em andamento;
- recursos legitimamente disponíveis;
- conhecimento de cada força;
- prazos;
- gatilhos;
- estágios de execução;
- deslocamentos;
- ações planejadas;
- armadilhas já legitimamente preparadas;
- consequências futuras já estabelecidas;
- outros processos internos do lado adversarial.

Não registrar informação apenas para preencher a pasta.

```text
FATO ADVERSARIAL PERSISTENTE QUE PRECISA CONTINUAR VERDADEIRO
→ registrar.

REAÇÃO LOCAL SEM IMPORTÂNCIA FUTURA
→ pode permanecer somente na cena ou no Estado pertinente.
```

## Como um plano entra no Registro

Quando o Opositor está ativo, ele pode declarar a intenção de uma força dentro de seu escopo.

```text
OPOSITOR
→ uma força adversarial começa a preparar uma ação para daqui a alguns dias.
```

O Narrador / Juiz verifica:

```text
possui fundamento?
possui conhecimento?
possui meios?
possui tempo?
possui oportunidade?
essa força está realmente dentro do escopo do Opositor?
```

Se o plano for válido, o processo e o prazo passam a fazer parte da realidade da campanha e podem ser registrados.

```text
DECLARAÇÃO DO OPOSITOR
→ NARRADOR / JUIZ verifica
→ processo adversarial estabelecido
→ REGISTRO preserva
```

Se a força possuir cadeira própria, a intenção vem dessa cadeira e não do Opositor. O registro ainda pode preservar o plano na fonte apropriada, mas não altera sua autoria.

## Modelo de entrada

```text
FORÇA ADVERSARIAL A
Objetivo: impedir acesso a determinada região
Plano atual: reforçar os pontos de entrada
Estado: preparação em andamento
Prazo: concluir em 5 dias
Recursos: [somente os já estabelecidos]
Conhecimento: [somente o que essa força realmente sabe]

FORÇA ADVERSARIAL B
Objetivo: recuperar determinado recurso
Plano atual: localizar quem o possui
Estado: investigação em andamento
Prazo: [quando houver]
```

Esse bloco é apenas um modelo. Identidades, planos e prazos reais pertencem à campanha.

## Plano não é sucesso

Registrar um plano significa apenas que ele existe e está em andamento.

Não significa que será concluído com sucesso.

O plano pode ser:

- descoberto;
- atrasado;
- interrompido;
- alterado;
- impedido;
- abandonado;
- derrotado por outra ação legítima.

Quando isso acontecer, o Registro deve ser atualizado para refletir o estado real.

## Passagem do tempo

Um processo adversarial registrado pode continuar fora da cena principal sem precisar ser redeclarado em todas as janelas.

Quando o Opositor estiver ativo, ele volta a decidir quando:

- chega uma etapa do plano;
- o prazo vence;
- surge nova decisão adversarial;
- a situação muda;
- aparece nova oportunidade;
- uma força de seu escopo entra em campo.

Processos que não possuem vontade própria continuam avançando por causalidade e Estado; não precisam de Opositor apenas para o tempo passar.

## Fiscalização

O Registro serve para impedir que fatos internos já estabelecidos sejam esquecidos.

```text
REGISTRO
→ determinado processo alcança sua etapa hoje.

OPOSITOR, SE ATIVO
→ traz a decisão adversarial pertinente quando houver.

NARRADOR / JUIZ
→ verifica a fonte e aplica o que realmente se tornou relevante.
```

A fiscalização não cria nem antecipa o fato.

## Conhecimento compartimentado

O executor do Opositor pode conhecer todo o material necessário para administrar sua função.

Esse conhecimento não pertence automaticamente a cada força representada.

```text
OPOSITOR SABE
≠
FORÇA ADVERSARIAL SABE
```

Cada peça só pode agir com o conhecimento que ela própria possui legitimamente.

## Restrição operacional

O conteúdo real pode estar totalmente visível dentro de `campanhas/<nome>/`.

A regra não tenta impedir que quem administra a campanha o leia.

Ela apenas impede que uma cadeira use esse conteúdo como conhecimento ficcional sem fundamento.

```text
EXECUTOR LEU O ARQUIVO
≠
PERSONAGEM DESCOBRIU A INFORMAÇÃO
```

Se uma informação adversarial for descoberta legitimamente, registrar o fato correspondente na fonte apropriada para que o conhecimento da personagem possa ser reconstruído depois.

## Regra final

> **O Registro Reservado é um modelo opcional para campanhas com Opositor ativo e informação adversarial persistente que precise ser preservada. Ele não cria planos, não torna o Opositor obrigatório e não concede conhecimento às personagens. “Reservado” é uma restrição operacional de conhecimento, não ocultação física do arquivo.**