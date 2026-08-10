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

---

## D03 — Como o Narrador escolhe uma Dificuldade do mundo?

**Status:** Resolvida.

### Decisão

A resolução distingue claramente **cenário passivo** de **oposição ativa**.

#### Contra o cenário

O personagem produz seu Patamar de Ação:

> **Patamar da Ação = Atributo + Destino**

A situação possui uma **Dificuldade em Patamar**, representando o grau atual da tarefa dentro das condições gerais da cena.

> **Patamar do Resultado = Patamar da Ação − Dificuldade**

A Dificuldade pode mudar quando a própria situação muda para todos os envolvidos. Chuva forte, pouca iluminação geral, terreno instável ou outras condições compartilhadas podem tornar a tarefa mais difícil ou mais fácil.

A Dificuldade não precisa representar apenas a resistência física de um objeto. Ela representa a **dificuldade real da ação naquela situação**.

#### Contra outro personagem

Ambos os lados produzem seus próprios Patamares:

> **Patamar da Ação = Atributo da Ação + Destino da Ação**

> **Patamar da Resistência = Atributo da Resistência + Destino da Resistência**

Depois:

> **Patamar do Resultado = Patamar da Ação − Patamar da Resistência**

O Patamar do Resultado indica **quem prevalece e em qual grau**.

### Sorte, Azar e Dificuldade

Foi consolidada a seguinte separação:

> **A situação modifica a Dificuldade. Sorte e Azar modificam o personagem.**

Condições gerais da cena alteram a Dificuldade para todos que enfrentam aquela situação.

Condições individuais — como estar Cego, improvisar sem a ferramenta adequada, possuir uma Perícia aplicável ou utilizar equipamento excepcional — afetam especificamente a parada daquele personagem por Sorte ou Azar.

Essa decisão substitui a formulação anterior segundo a qual circunstâncias externas prejudiciais gerariam automaticamente Azar para quem as sofre.

### Faixa prática de incerteza

Os quatro Dados de Destino variam matematicamente de **−4 a +4**, mas a maior parte dos resultados se concentra aproximadamente entre **−2 e +2**.

Por isso, diferenças de até cerca de **2 Patamares** entre capacidade e Dificuldade formam a principal faixa prática de incerteza do sistema.

Isso é uma **referência de julgamento**, não um limite rígido. Valores mais extremos ainda podem ser rolados quando a ficção sustentar uma possibilidade real. Porém, quando a Dificuldade está muito acima da capacidade do personagem, o Narrador deve avaliar se ainda existe uma chance significativa ou se oferecer a rolagem seria apenas uma ilusão de possibilidade.

Da mesma forma, tarefas muito abaixo da capacidade, sem pressão ou consequência relevante, normalmente não precisam de teste.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/testes-e-resolucoes.md`;
- `regras/turnos-e-acoes.md`.

---

## D04 — Quando uma falha negativa produz uma consequência contra o personagem?

**Status:** Resolvida.

### Decisão

Um resultado negativo elevado significa que a Resistência prevaleceu com maior intensidade, mas **não cria automaticamente uma punição**.

> **O Patamar determina a intensidade da consequência possível; a ficção determina quais consequências podem existir.**

Toda consequência precisa nascer da própria ação, de um risco existente, de uma condição da cena ou de um elemento plausível que o Narrador possa revelar sem contradizer a ficção já estabelecida.

Exemplos válidos incluem:

- uma tentativa de arrombar uma porta acionar um alarme plausível daquele local;
- um personagem escorregar porque o piso estava molhado ou instável;
- uma queda colocar objetos frágeis carregados pelo personagem em risco, podendo quebrar uma poção;
- uma tentativa furtiva fazer barulho e chamar atenção.

Consequências podem se encadear quando a ficção sustentar essa sequência. O Narrador não precisa limitar a falha ao obstáculo imediato, mas também não pode usar o Patamar negativo como justificativa para inventar Dano, Status ou perdas sem relação plausível com a situação.

Se nenhuma consequência adicional fizer sentido, mesmo um resultado negativo muito alto pode significar apenas que a Resistência prevaleceu de maneira decisiva.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/patamar.md`;
- `regras/testes-e-resolucoes.md`.

---

## D05 — A nota final de Dados de Destino ainda é necessária?

**Status:** Resolvida.

### Decisão

A seção `Estado da Regra` era uma anotação de desenvolvimento e não acrescentava uma regra útil para Narradores ou jogadores.

Como a relação entre Dados de Destino, Sorte, Azar, Perícias e Patamar já está definida no próprio capítulo e em `testes-e-resolucoes.md`, manter uma nota de estado editorial poderia dar a impressão de que a mecânica ainda está provisória.

A seção foi removida. O capítulo agora termina em `Relação com Patamar`, preservando apenas conteúdo de uso efetivo em jogo.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/dados-de-destino.md`.

---

## D09 — A notação de Cura e das disputas pode ser confundida com multiplicação?

**Status:** Resolvida.

### Decisão

O símbolo **−** passa a ser a notação abreviada das disputas ativas, seguindo sempre a ordem:

> **Ação − Resistência**

Assim, **INT − AGI** significa que INT é o Atributo de quem age e AGI o Atributo de quem resiste.

Essa notação é apenas uma forma curta. Em uma disputa ativa completa, ambos continuam acrescentando seus Dados de Destino quando aplicável:

> **(INT + Destino da Ação) − (AGI + Destino da Resistência) = Patamar do Resultado**

O sinal do resultado determina quem prevalece:

- positivo: Ação prevalece;
- zero: equilíbrio;
- negativo: Resistência prevalece.

O valor absoluto determina o Patamar do resultado em favor do lado vencedor.

O símbolo **×** fica reservado exclusivamente para multiplicação matemática verdadeira, como **VIG × 3**.

### Clarificação relacionada de Cura e recuperação

Durante a análise foi reafirmada a distinção entre formas de recuperar Vida:

- **recuperação natural pessoal:** utiliza VIG;
- **tratamento médico durante descanso:** utiliza SAB + Destino, com Medicina quando aplicável;
- **Regeneração restrita ao próprio usuário:** utiliza VIG;
- **Poder de Cura capaz de afetar outros:** utiliza SAB.

Essa distinção preserva a função dos Atributos e evita tratar toda restauração de Vida como a mesma ação.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/testes-e-resolucoes.md`;
- `regras/combate.md`;
- `regras/poderes.md`;
- `regras/turnos-e-acoes.md`.

A clarificação de Cura e recuperação também já havia sido alinhada em:

- `regras/vida-e-mana.md`;
- `regras/poderes.md`;
- `regras/pericias.md`.

---

## D12 — Status e Patamar: quando vira Azar ou impossibilidade?

**Status:** Resolvida.

### Decisão

Não existe uma tabela universal que converta automaticamente Patamar em **Azar [1]**, **Azar [2]** ou impossibilidade.

O **Patamar do Resultado** determina a intensidade, qualidade e magnitude com que a ação ou efeito prevaleceu. A consequência concreta continua sendo determinada pela intenção da ação e pela narrativa.

Uma ação de **Criar Vantagem**, por exemplo, não possui uma escala fixa de Patamar para Azar. Se um personagem tenta distrair um adversário, um resultado menor pode produzir uma vantagem pequena; um resultado maior pode justificar Azar; e um resultado extraordinário pode, quando a ficção sustentar isso, impedir completamente que o alvo perceba determinada aproximação ou oportunidade. Esses são exemplos de manifestação daquela ação, não uma tabela geral.

A mesma lógica vale para Status. Um Status pode:

- gerar Azar em uma ação que continua possível;
- tornar uma ação específica impossível;
- não interferir em outra ação que não dependa da capacidade afetada.

O Patamar mede **o quanto** a condição ou vantagem foi bem-sucedida. A ficção determina **o que** essa intensidade significa naquele caso.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/status.md`;
- `regras/turnos-e-acoes.md`.

---

## D13 — Surpresa: quem age primeiro?

**Status:** Resolvida.

### Decisão

Quando um confronto começa, **todos os envolvidos podem rolar Iniciativa**, inclusive os personagens surpreendidos. A Iniciativa estabelece desde o início a ordem mecânica usada para resolver o confronto.

A surpresa não retira o personagem da ordem. Em vez disso, quem foi surpreendido **não realiza seu turno na primeira rodada** e só começa a agir normalmente quando sua posição de Iniciativa chegar na **segunda rodada**.

Os personagens que estavam conscientes e preparados realizam normalmente seus turnos da primeira rodada conforme a ordem de Iniciativa.

Foi também consolidada a distinção entre **ordem mecânica** e **tempo ficcional**. Os turnos existem para organizar a resolução na mesa, mas ações resolvidas em sequência podem representar acontecimentos simultâneos ou quase simultâneos na ficção.

Assim, em uma emboscada com três assassinos preparados, os três podem atacar praticamente ao mesmo tempo narrativamente, embora suas ações sejam resolvidas uma por uma segundo a Iniciativa.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/iniciativa.md`.

---

## D14 — Sorte, Azar e Perícias podem modificar a Iniciativa?

**Status:** Resolvida.

### Decisão

**Sorte e Azar podem modificar a rolagem de Iniciativa quando a fonte realmente afetar a capacidade daquele personagem de perceber, antecipar ou reagir ao início do confronto.**

A aplicação é narrativa e contextual. Não existe uma lista fixa de condições que sempre concedem Sorte ou Azar na Iniciativa.

Exemplos discutidos:

- um Poder de premonição pode conceder Sorte para notar o perigo quando sua descrição realmente oferecer essa vantagem;
- estar Confuso pode gerar Azar quando a condição prejudicar a percepção do perigo ou a capacidade de reagir ao que acontece ao redor.

Esses exemplos demonstram possibilidades, não criam efeitos universais automáticos.

Perícias também só modificam a Iniciativa quando puderem ser **realmente aplicadas** à percepção, antecipação ou reação naquele momento. Uma relação apenas temática com o confronto não concede Sorte por si só.

A decisão preserva a regra geral já consolidada de que **Sorte e Azar modificam o personagem** e só se aplicam quando a fonte é relevante para a ação ou resolução em questão.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/iniciativa.md`.

---

## D06 — As categorias de Perícia usam o mesmo orçamento de Pontos de Perícia?

**Status:** Resolvida.

### Decisão

Os **Pontos de Perícia formam um único orçamento**.

O total obtido pela regra-base:

> **Pontos de Perícia = (Patamar de Cenário × 4) + INT**

pode ser distribuído entre **Perícias Gerais, Perícias de Combate e Perícias de Poder** às quais o personagem tenha acesso.

Cada categoria mantém seu próprio custo, mas esses custos são pagos a partir do mesmo total de Pontos de Perícia. Não existem reservas separadas para Perícias Gerais, de Combate ou de Poder.

Assim, o jogador pode misturar livremente os investimentos entre as categorias durante a criação, respeitando os custos e requisitos de acesso de cada uma.

A regra atual de graus e custos das Perícias permanece como **regra-base geral do W4D**. Possíveis alterações específicas de cenário não fazem parte da D06 e serão tratadas separadamente quando necessário.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/pericias.md`.

---

## D07 — INT concede novos Pontos de Perícia depois da criação?

**Status:** Resolvida.

### Decisão

A regra-base continua sendo:

> **Pontos de Perícia = (Patamar de Cenário × 4) + INT**

Se, depois da criação, alguma regra permitir que **INT aumente**, o total de Pontos de Perícia também aumenta na mesma proporção.

Assim, um aumento de +1 em INT acrescenta +1 ao total de Pontos de Perícia; um aumento de +2 acrescenta +2, e assim por diante.

A D07 não define se, quando ou por quais meios os Atributos podem ser aumentados depois da criação. Essa é uma questão separada de evolução. Aqui fica definido apenas que, **caso INT seja ampliada, sua contribuição para o total de Pontos de Perícia acompanha o novo valor**.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/pericias.md`.

---

## D08 — Quantos Poderes existem na criação e como são adquiridos?

**Status:** Resolvida.

### Decisão

O W4D **não possui uma quantidade universal de Poderes iniciais**.

A quantidade de Poderes disponível na criação, quais fontes ou tradições existem e as formas pelas quais novos Poderes podem ser adquiridos são **definições do cenário**.

A regra-base de Poderes deve oferecer a estrutura necessária para que o cenário tome essas decisões, da mesma forma que a Mecânica dos Itens estabelece como os itens funcionam sem obrigar todos os cenários a possuir os mesmos itens, recursos ou formas de acesso.

Assim, o núcleo determina **como um Poder funciona**; o cenário determina **quais Poderes existem, quem pode acessá-los e em que quantidade**.

A construção mais completa dessas bases será tratada posteriormente no desenvolvimento do capítulo de Poderes. A D08 não antecipa números, listas ou métodos de aquisição que ainda não foram definidos.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/poderes.md`.

---

## D10 — O que significa o mínimo [1] na recuperação natural?

**Status:** Resolvida.

### Decisão

O **mínimo [1] é um piso de recuperação**, não uma penalidade invertida nem uma fonte de Dano.

Quando um Descanso Curto usa **VIG + Destino** para recuperar Vida ou **VON + Destino** para recuperar Mana, um resultado [0] ou negativo não transforma o descanso em perda de recurso. O personagem recupera pelo menos **1 ponto**.

Assim, um humano comum com **VIG [0]** que obtenha o resultado extremamente raro de Destino **[-4]** durante a recuperação não sofre 4 pontos de Dano. O resultado simplesmente não aumenta a recuperação acima do mínimo, e o personagem recupera **1 ponto de Vida**.

No Descanso Longo de Vida, aplica-se primeiro esse mínimo de 1 e depois a multiplicação por 4. A recuperação longa de Mana continua seguindo sua regra própria de recuperar 100% da Mana.

Essa regra trata exclusivamente da quantidade recuperada durante o descanso. Consequências negativas só existem se houver alguma situação narrativa separada que realmente as produza; a rolagem de recuperação, por si só, não cria Dano.

### Ajustes realizados

A decisão foi explicitada em:

- `regras/vida-e-mana.md`.
