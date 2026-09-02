# Reformulação — Estado e Pendências

Status: DOCUMENTO DE TRABALHO

Este arquivo registra o que já foi convertido para o novo W4D-RPG e o que ainda precisa ser decidido em conjunto.

## Já reformulado

```text
README.md
→ filosofia geral de autoria narrativa compartilhada.

nucleo/0.0-autoria-narrativa.md
→ princípios centrais.

nucleo/0.1-resolucao.md
→ ficção primeiro; incerteza não obriga RNG.

nucleo/1.0-tribunal.md
→ soberania das cadeiras + modo Diretor usando [ ].

nucleo/1.0.1-auditoria-das-cadeiras.md
→ Mesa sob demanda, apenas com autoridades afetadas.

nucleo/1.1-narrador.md
→ Narrador como Juiz.

nucleo/1.5-opositor.md
→ ação adversarial + objeção factual curta.

jogador/1.0-descricao-da-ficha.md
→ ficha como descrição operacional e fonte canônica.

jogador/1.1-atributos-pericias-poderes.md
→ competências e conhecimentos narrativos; sem Atributo + Perícia universal.

jogador/1.2-poderes-e-equipamentos.md
→ Poderes como capacidades; [1]-[3] apenas para comparação.

jogador/FICHA-EM-BRANCO.md
→ modelo narrativo sem matemática obrigatória.

jogador/MODELO-DE-FICHA.md
jogador/README.md
→ alinhados à nova proposta.
```

## Princípios já fechados

```text
1. RPG = vários autores escrevendo uma história juntos.
2. Cada cadeira controla sua própria autoridade.
3. Declaração própria não estabelece resultado sobre outra cadeira.
4. A ficha serve principalmente como fonte de fatos e comparação.
5. Conhecimento pode ser registrado como Conhece / Especialista.
6. Graduações [1]-[3] são comparativas, não bônus.
7. A ficção resolve quando os fatos já respondem.
8. Incerteza não cria rolagem obrigatória.
9. Opositor pode fazer objeção factual curta.
10. Narrador é Juiz do encontro entre fatos e autoridades.
11. Texto humano em [ ] é modo Diretor, não ação ou conhecimento da personagem.
12. Diretor e personagem humana são o mesmo autor em modos diferentes, não duas cadeiras.
13. Mesa só abre com dúvida, discordância, direção compartilhada ou conflito real de autoridade.
14. Só participam da Mesa as autoridades afetadas.
15. Resultado geral conhecido ainda pode produzir uma cena dramaticamente aberta em significado e execução.
```

## Pendências prioritárias

### 1 — Criação de personagem

Reescrever:

```text
jogador/1.3-criacao-da-ficha.md
```

Decidir:

```text
como limitar uma ficha sem voltar a orçamento matemático excessivo
se existe Patamar global ou apenas capacidades graduadas
como distinguir personagem comum, heroica, cósmica etc.
quantas especialidades são razoáveis
como aprovar Poderes amplos
```

### 2 — Traços

`jogador/1.4-tracos.md` é amplamente compatível.

Revisar apenas:

```text
se Traços continuam sem custo
como impedir que um Traço esconda um Poder graduável
como registrar limitações narrativas complexas sem transformar tudo em regra mecânica
```

### 3 — Autoridade da ficha

`jogador/1.5-autoridade-da-ficha.md` também é amplamente compatível.

Adicionar futuramente, se necessário:

```text
autoridade epistêmica de Especialistas
comparação entre fichas
relação entre ficha e Direção
```

### 4 — Combate

Revisar ou remover:

```text
nucleo/0.5-combate.md
nucleo/0.6-dano-e-ferimentos.md
nucleo/0.7-iniciativa.md
nucleo/0.8-tempo-e-acoes.md
nucleo/0.9-alcance-e-movimento.md
```

Perguntas abertas:

```text
combate precisa de regra própria ou apenas exemplos de julgamento?
ferimentos precisam de escala narrativa?
incapacitado/morto precisam de autorização especial?
como representar desgaste progressivo sem PV?
```

### 5 — Vida, Mente e Mana

Revisar:

```text
nucleo/0.10-mana.md
nucleo/0.11-vida-e-mente.md
nucleo/0.12-ataques-mentais.md
nucleo/0.13-cura-e-recuperacao.md
```

Pergunta principal:

> Esses recursos ainda cumprem uma função que a ficção, os estados e as limitações da ficha não conseguem cumprir melhor?

Não preservar apenas porque já existem.

### 6 — Potência de Efeito

`nucleo/0.14-potencia-de-efeito.md` pertence diretamente ao motor anterior.

Provável destino:

```text
remover
ou
substituir completamente por comparação de capacidades [1]-[3]
```

### 7 — Rolagens e disputas

Revisar:

```text
nucleo/0.2-rolagens.md
nucleo/0.3-consequencias.md
nucleo/0.4-disputas-simultaneas.md
```

A nova base já estabelece:

```text
RNG não é motor padrão
```

Se um mecanismo de acaso sobreviver, deverá ser explicitamente opcional e responder a uma função autoral clara.

### 8 — Criação de campanha e temporada

Revisar depois do núcleo:

```text
CRIACAO-DE-CAMPANHA.md
CRIACAO-DE-TEMPORADA.md
INICIO-E-RETOMADA.md
```

Preservar o que funciona:

```text
Narrativa da Campanha
Direção do Jogador
Roteiro
Estado Atual
Livro
Registro
continuidade entre temporadas
```

Remover referências que dependam do motor matemático anterior.

### 9 — Mestre e Registro

Grande parte pode sobreviver.

Revisar referências a:

```text
rolagem obrigatória
Potência
Vida/Mana mecânicas
Auditoria obrigatória
Motor matemático
```

## Critério para cada regra antiga

Para cada arquivo restante, perguntar:

```text
QUE FUNÇÃO REAL ELE CUMPRE?

A ficção + ficha + cadeiras + Juiz já cumprem essa função?
→ sim: remover ou simplificar.

Existe uma lacuna real sem essa regra?
→ sim: preservar apenas a menor regra necessária.
```

## Regra de trabalho

> **Não adaptar o motor antigo por nostalgia estrutural. Preservar apenas funções que continuem necessárias no novo jogo.**
