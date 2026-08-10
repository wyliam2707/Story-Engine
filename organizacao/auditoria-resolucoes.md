# Auditoria — Resoluções

Este arquivo acompanha as decisões tomadas durante a revisão por duas perspectivas. A lista original de dúvidas permanece em `auditoria-narrador-jogador-pendencias.md`.

Cada item só é registrado aqui depois de discutido e concluído.

---

## D01 — O que exatamente chamamos de Patamar?

**Status:** Resolvida.

### Decisão

**Patamar** é a escala universal de magnitude do W4D, normalmente expressa de **[0] a [8]**.

São medidos diretamente em Patamar, quando aplicável:

- Atributos;
- dificuldades e Resistências fixas;
- resultados de disputas;
- Efeitos cuja descrição determine intensidade em Patamar.

Nem todo número do sistema é um Patamar.

**Dano, Proteção, Vida, Mana e outros valores derivados** possuem regras próprias. Eles podem ser calculados a partir de um Patamar sem se tornarem Patamares e podem ultrapassar [8] quando sua regra permitir.

**Sorte e Azar** são Graus próprios, não Patamares. Seu valor efetivo segue a mecânica dos Dados de Destino.

**Poderes** não possuem automaticamente um Patamar próprio. Quando necessário, uma resolução produz um Patamar e a descrição do Poder determina como esse resultado se manifesta ou é convertido em outra grandeza.

O **Patamar de Cenário [I–V]** é uma classificação de escala do cenário, distinta do Patamar universal [0–8] usado para magnitudes e resultados.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/patamar.md`;
- `regras/dados-de-destino.md`;
- `regras/combate.md`;
- `regras/poderes.md`.

A alteração foi de **clareza terminológica**, preservando as mecânicas já existentes.

---

## D02 — Qual é toda a função do Patamar de Cenário?

**Status:** Resolvida.

### Decisão

O **Patamar de Cenário [I–V]** possui duas funções oficiais e complementares:

1. **Função mecânica de criação:** determina os pontos iniciais de Atributo e o maior valor inicial permitido por Atributo para os protagonistas.
2. **Função de referência de escala:** estabelece qual é a escala normal esperada para os protagonistas e serve como régua para comparar ameaças, obstáculos, equipamentos, fenômenos e demais elementos do cenário.

Essa referência **não é um teto do mundo**. Criaturas, chefes, fenômenos e outros elementos podem possuir valores acima do Patamar do Cenário quando isso for narrativamente apropriado.

A referência do Bestiário já expressava esse princípio:

> **O Patamar do cenário define a normalidade, não os limites do mundo.**

Assim, estar acima da escala normal deve ser excepcional e significativo, mas não proibido. Quanto maior a diferença, mais a situação pode exigir preparação, cooperação, vantagens, recursos especiais ou uma abordagem diferente do confronto direto.

O Patamar de Cenário também **não cria fórmulas automáticas para todos os subsistemas**. Ele orienta a escala; regras específicas continuam determinando Dano, Proteção, Resistências, equipamentos, criaturas e demais elementos.

### Relação com dúvidas futuras

A ideia já discutida de usar uma faixa aproximada ligada ao maior Atributo do cenário — incluindo a referência de **+2 para Resistências normalmente testáveis** — pertence principalmente à **D03**, que trata de como o Narrador escolhe Resistências fixas do mundo. Essa questão não foi incorporada à D02 para evitar misturar função de escala com calibração de dificuldade.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/patamar.md`.

O arquivo `bestiario/referencia-de-patamar.md` já estava coerente com essa interpretação e não precisou ser alterado.
