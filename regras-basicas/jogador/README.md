# Jogador

Status: REFORMULAÇÃO ATIVA

Esta pasta reúne as regras necessárias para **criar, ler e usar uma personagem durante a sessão**.

Jogadores e NPCs usam a mesma lógica básica de ficha.

```text
jogador/
├── README.md
├── FICHA-EM-BRANCO.md
├── MODELO-DE-FICHA.md
├── 1.0-descricao-da-ficha.md
├── 1.1-atributos-pericias-poderes.md
├── 1.2-poderes-e-equipamentos.md
├── 1.3-criacao-da-ficha.md
├── 1.4-tracos.md
└── 1.5-autoridade-da-ficha.md
```

## Princípio

> **Primeiro cria-se a personagem. Depois a ficha registra e organiza aquilo que essa personagem realmente é.**

A ficha oficial serve simultaneamente como:

```text
ROTEIRO DE CRIAÇÃO
→ conduz a construção da personagem em uma ordem comum.

FONTE CANÔNICA
→ preserva quem a personagem é depois de aprovada.

BASE DE COMPARAÇÃO
→ permite ao Narrador comparar capacidades equivalentes quando isso realmente importar.
```

## Metadados da personagem

Antes dos sete blocos, a ficha registra:

```text
IMPORTÂNCIA NARRATIVA
→ quanto a campanha precisa preservar, acompanhar e desenvolver a personagem.

CONTROLE
→ qual cadeira decide voluntariamente por ela.
```

Importância Narrativa usa:

```text
PROTAGONISTA
RECORRENTE
EVENTUAL
INCIDENTAL
```

Ela serve somente para organização e profundidade de persistência.

```text
IMPORTÂNCIA NARRATIVA
≠ poder
≠ nível
≠ autoridade
≠ prioridade de ação
≠ bônus
≠ imunidade narrativa
```

Uma personagem incidental pode ser mais poderosa que uma protagonista.

`Patamar` pertence ao motor anterior e não existe como nível geral ativo da ficha nova.

## Estrutura central da personagem

A criação usa sete blocos:

```text
1. Descrição Física
2. Conceito
3. Habilidades
4. Traços e Poderes
5. Descrição Emocional / Personalidade
6. Histórico
7. Estado Atual
```

### Descrição Física

Registra como a personagem existe visualmente no mundo.

### Conceito

Resume quem ela é em essência e serve como primeira referência de coerência para o restante da ficha.

### Habilidades

Registra capacidades adquiridas por treino, prática, formação ou experiência.

Pode incluir:

```text
COMPETÊNCIA
→ o que sabe fazer.

CONHECIMENTO
→ o que sabe.

CONHECE
→ familiaridade relevante com um campo.

ESPECIALISTA
→ domínio profundo de um campo; sua interpretação possui forte autoridade quando o assunto está dentro de seu repertório.
```

### Traços e Poderes

O quarto bloco também guarda Equipamentos e Recursos relevantes.

```text
TRAÇO
→ verdade especial da personagem dentro da descrição aprovada.

PODER
→ capacidade extraordinária utilizável.

EQUIPAMENTO
→ item externo relevante que a personagem possui ou usa.

RECURSO
→ acesso, estrutura, patrimônio, veículo, contato institucional ou outro meio externo relevante.

[1] / [2] / [3]
→ comparação de intensidade entre capacidades equivalentes, não bônus.
```

### Descrição Emocional / Personalidade

Registra tendências, desejos, medos, limites, hábitos e relações que realmente alteram interpretação e decisão.

### Histórico

Explica origem, formação, experiências e fatos passados que continuam sustentando quem a personagem é hoje.

### Estado Atual

Registra somente o **recorte pessoal temporário** da personagem.

```text
campanhas/<nome>/estado/atual.md
→ fonte canônica global do presente.

FICHA / ESTADO ATUAL
→ parte desse presente que precisa acompanhar aquela cadeira.
```

## Coerência como limite de criação

O sistema não precisa começar por um orçamento matemático para impedir excesso.

Uma Habilidade, Traço, Poder, Equipamento ou Recurso relevante precisa nascer legitimamente de:

```text
Conceito
+
Descrição
+
Natureza
+
Formação
+
Experiência
+
Histórico
```

Quando algo não encontra fundamento suficiente, deve ser explicado ou removido antes da aprovação.

```text
"Especialista em Demônios"
+
histórico de estudo ocultista e convivência sobrenatural
→ coerente.

"Especialista em Engenharia Nuclear"
+
nenhuma formação, experiência ou fato que sustente isso
→ não aprovar ainda.
```

Não usar Patamar, orçamento de pontos ou Importância Narrativa para justificar algo que a personagem criada não sustenta.

## Memória por cadeira

Cada cadeira de personagem opera somente com:

```text
SUA PRÓPRIA FICHA
+
SEU RECORTE PESSOAL DO ESTADO ATUAL
+
CONHECIMENTO LEGÍTIMO DA PERSONAGEM
+
FATOS DA CENA QUE ELA PODE PERCEBER OU CONHECER
```

Ela não precisa carregar a ficha completa de outras personagens nem receber o Estado global inteiro.

```text
IA TÉCNICA PODE TER ACESSO
≠
CADEIRA DA PERSONAGEM PODE USAR
```

Comparações entre fichas pertencem ao Narrador/Juiz e, quando a oposição estiver legitimamente envolvida, ao Opositor.

A cadeira pode conhecer capacidades de outra personagem somente na medida em que sua própria personagem tenha aprendido isso dentro da ficção.

## Arquivos

`FICHA-EM-BRANCO.md`
→ estrutura oficial e roteiro copiável de criação.

`MODELO-DE-FICHA.md`
→ explica a lógica do modelo e a ordem da criação.

`1.0-descricao-da-ficha.md`
→ define como os blocos, Importância Narrativa e Controle são lidos.

`1.1-atributos-pericias-poderes.md`
→ competências, conhecimentos e linguagem comparativa; registra Patamar como legado.

`1.2-poderes-e-equipamentos.md`
→ capacidades extraordinárias e graduações comparativas.

`1.3-criacao-da-ficha.md`
→ procedimento de criação e aprovação.

`1.4-tracos.md`
→ verdades especiais da personagem.

`1.5-autoridade-da-ficha.md`
→ autoridade canônica da ficha durante interpretação, julgamento e representação.

## Regra final

> **A ficha é criada de dentro para fora: descrevemos a pessoa, entendemos seu conceito, extraímos Habilidades, Traços, Poderes, Equipamentos e Recursos coerentes, registramos sua vida emocional e seu Histórico e somente então tratamos esse conjunto como fonte canônica. Importância Narrativa organiza persistência; Controle define autoria; Patamar não pertence ao sistema ativo. Cada cadeira precisa memorizar a própria personagem, não o elenco inteiro.**
