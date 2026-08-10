# Auditoria por Duas Perspectivas — Dúvidas Pendentes

## Estado deste documento

Este arquivo é uma **memória de revisão**, não um conjunto de regras novas.

As questões abaixo surgiram da leitura do sistema atual por duas perspectivas:

- **Narrador:** alguém tentando aplicar as regras em mesa sem precisar adivinhar decisões importantes;
- **Jogador:** alguém tentando criar, compreender e utilizar um personagem apenas com o texto disponível.

Nenhum item abaixo altera uma regra existente. Cada dúvida deve ser analisada **uma por vez**, comparando os arquivos relacionados antes de qualquer mudança.

> **Encontrar uma dúvida não significa que a regra esteja errada. Significa apenas que existe um ponto que merece ser confirmado, explicado ou conscientemente mantido como está.**

---

# Fila de Dúvidas

## D01 — O que exatamente chamamos de Patamar?

**Perspectiva:** Narrador + Jogador  
**Arquivos relacionados:** `patamar.md`, `combate.md`, `efeitos.md`, `dados-de-destino.md`

`patamar.md` afirma que Patamar representa atributos, Sorte, dificuldades, Resistências, Dano, Proteção, Poderes e Efeitos. Porém, outras regras já distinguem **Patamar** de valores derivados como **Dano** e **Proteção**, que podem ultrapassar [8], enquanto Sorte/Azar possuem uma escala própria limitada efetivamente a [2].

**Dúvida:** precisamos tornar a terminologia mais precisa para evitar que o leitor trate Dano, Proteção ou Sorte como se obedecessem exatamente às mesmas regras do Patamar de resultado?

---

## D02 — Qual é toda a função do Patamar de Cenário?

**Perspectiva:** Narrador + criação de cenário  
**Arquivos relacionados:** `patamar.md`, `atributos.md`

O texto atual diz que o Patamar de Cenário determina **apenas** pontos iniciais de Atributo e limite inicial por Atributo. Durante o desenvolvimento, porém, ele também passou a ser entendido como o **coração da escala do cenário**, servindo de referência para gênero, capacidades comuns, ameaças, dificuldades do mundo, equipamentos e demais elementos.

**Dúvida:** a definição atual está estreita demais em relação ao papel que queremos que o Patamar de Cenário exerça?

**Observação:** qualquer alteração aqui toca o coração do sistema e não deve ser feita sem discussão específica.

---

## D03 — Como o Narrador escolhe uma Resistência fixa do mundo?

**Perspectiva:** Narrador  
**Arquivos relacionados:** `testes-e-resolucoes.md`, `patamar.md`

A regra explica como resolver uma Resistência passiva, mas ainda oferece pouca orientação sobre **como escolher seu valor**.

Exemplo: o Narrador sabe que uma porta reforçada usa Resistência fixa, mas como decide se ela é [1], [2], [3] ou [5] dentro daquele cenário?

**Dúvida:** precisamos de uma orientação ligada ao Patamar do cenário para definir a faixa de Resistências testáveis do mundo e reconhecer quando é melhor declarar uma abordagem simplesmente impossível?

**Ideia já discutida, ainda não transformada em regra:** usar como referência uma Resistência máxima normalmente testável próxima de `maior Atributo inicial do cenário + 2`.

---

## D04 — Quando uma falha negativa produz uma consequência contra o personagem?

**Perspectiva:** Narrador  
**Arquivos relacionados:** `patamar.md`, `testes-e-resolucoes.md`

O Patamar negativo permite que a Resistência prevaleça com intensidade e pode gerar consequências contra quem realizou a ação. O exemplo de arrombar uma porta chega a sugerir queda ou lesão em falhas intensas.

**Dúvida:** está suficientemente claro que a consequência precisa nascer de um **risco plausível da situação**, e não simplesmente do fato matemático de o resultado ser negativo?

Um Narrador novo poderia interpretar que qualquer Resistência passiva de Patamar alto “contra-ataca” o personagem mesmo quando não existe risco ficcional para isso.

---

## D05 — O texto final de Dados de Destino ainda possui uma nota obsoleta?

**Perspectiva:** Editorial + Narrador  
**Arquivo relacionado:** `dados-de-destino.md`

O final do arquivo diz que a interação detalhada dos Dados de Destino com Patamar e outras mecânicas “será definida conforme o desenvolvimento avançar”. Essa interação já foi desenvolvida em vários capítulos.

**Dúvida:** essa nota deve ser removida ou atualizada para não transmitir a impressão de que a regra ainda está incompleta?

---

## D06 — Todos os tipos de Perícia usam o mesmo orçamento de Pontos de Perícia?

**Perspectiva:** Jogador criando personagem  
**Arquivo relacionado:** `pericias.md`

O arquivo define:

> `Pontos de Perícia = (Patamar de Cenário × 4) + INT`

Depois informa custos para Perícias Gerais, de Combate e de Poder, mas não declara de forma absolutamente explícita se **todas são compradas usando o mesmo total de Pontos de Perícia**.

**Dúvida:** um jogador lendo somente o capítulo saberá sem hesitar se deve usar um único orçamento para todas essas compras?

---

## D07 — INT concede novos Pontos de Perícia quando aumenta depois da criação?

**Perspectiva:** Jogador + Evolução  
**Arquivos relacionados:** `pericias.md`, futuro capítulo de Evolução

Como INT participa da fórmula dos Pontos de Perícia, surge uma dúvida quando o personagem aumenta INT durante a campanha.

**Dúvida:** esse aumento concede Pontos de Perícia retroativamente, apenas na criação, ou de outra forma?

**Observação:** esta questão pertence principalmente ao futuro tema **Evolução** e deve permanecer aqui até chegarmos a ele.

---

## D08 — Quantos Poderes um personagem possui na criação e como são adquiridos?

**Perspectiva:** Jogador criando personagem  
**Arquivos relacionados:** `poderes.md`, `pericias.md`, `magia-e-sobrecarga.md`

A estrutura explica o que um Poder faz, como seus Atributos funcionam e como uma Perícia de Poder pode existir, mas o conjunto atual ainda não responde integralmente:

- quantos Poderes um personagem começa possuindo;
- como escolhe sua fonte/tradição;
- qual o custo de adquirir novos Poderes;
- quais limites dependem do Patamar do cenário.

**Dúvida:** isso é uma lacuna intencional aguardando o futuro framework de Poderes/Criação, ou alguma parte já deveria estar definida no núcleo atual?

---

## D09 — A notação de Cura pode ser interpretada como multiplicação?

**Perspectiva:** Jogador + Narrador  
**Arquivos relacionados:** `poderes.md`, `vida-e-mana.md`

A Cura aparece escrita como:

> `Cura = SAB + Destino × Patamar [0]`

A intenção parece ser uma **Ação SAB + Destino contra Resistência Patamar [0]**, mas o símbolo `×` pode ser lido matematicamente como multiplicação.

**Dúvida:** devemos padronizar a notação de disputas para eliminar essa ambiguidade visual?

---

## D10 — Como funciona exatamente o “mínimo [1]” da recuperação natural?

**Perspectiva:** Jogador + Narrador  
**Arquivo relacionado:** `vida-e-mana.md`

No Descanso Curto, Vida e Mana são recuperadas com teste contra Patamar [0] e o texto determina recuperação “mínimo [1]”.

**Dúvida:** mesmo um resultado 0 ou negativo recupera automaticamente 1 ponto? Se sim, a redação deveria deixar isso explícito para que ninguém interprete que apenas resultados positivos recebem o mínimo?

---

## D11 — O que significa a duração-base “Cena” para Poderes de efeito instantâneo?

**Perspectiva:** Narrador + criador de Poder  
**Arquivos relacionados:** `poderes.md`, `magia-e-sobrecarga.md`, `efeitos.md`

A regra geral diz que a duração-base dos Poderes é **Cena**, salvo descrição em contrário. Entretanto, Dano direto, Cura e Teleporte são naturalmente efeitos instantâneos segundo `efeitos.md`.

**Dúvida:** ao criar um Poder como “Lança de Energia — Dano: Patamar”, sem escrever sua duração, o leitor entende automaticamente que o Dano acontece uma vez ou poderia interpretar que o Poder permanece causando Dano durante a Cena?

Talvez seja necessário esclarecer a diferença entre **duração da manifestação/Poder** e **duração do componente de Efeito**.

---

## D12 — Status e Patamar: quando vira Azar [1], Azar [2] ou impossibilidade?

**Perspectiva:** Narrador  
**Arquivos relacionados:** `status.md`, `turnos-e-acoes.md`, `efeitos.md`

Status seguem a narrativa: se atrapalham uma ação possível, podem gerar Azar; se impedem a ação, ela é impossível. Entretanto, não existe uma regra geral dizendo quando a magnitude de um Status resulta em Azar [1], Azar [2] ou impedimento completo.

`Criar Vantagem`, por outro lado, possui uma referência mecânica própria: Patamar [1–2] pode gerar Azar [1], e [3+] pode gerar Azar [2].

**Dúvida:** essa diferença é intencional, preservando interpretação livre para Status, ou precisamos de uma orientação comum sem transformar Status numa tabela rígida de penalidades?

---

## D13 — Surpresa: quem exatamente recebe a primeira ação?

**Perspectiva:** Narrador  
**Arquivo relacionado:** `iniciativa.md`

A regra diz que, quando apenas um lado está consciente do combate, “o lado consciente age primeiro” e depois a Iniciativa pode ser determinada.

**Dúvida:** se três personagens surpreendem quatro inimigos, os três personagens realizam um turno completo antes da Iniciativa, apenas o personagem que iniciou a emboscada age, ou a ordem interna do lado consciente precisa ser resolvida de alguma forma?

A frase atual permite mais de uma leitura em mesa.

---

## D14 — Perícias ou outras fontes de Sorte podem modificar Iniciativa?

**Perspectiva:** Jogador + Narrador  
**Arquivos relacionados:** `iniciativa.md`, `dados-de-destino.md`, `pericias.md`

Iniciativa é definida como `maior entre AGI ou SAB + Destino`. A regra geral de Sorte permite que qualquer fonte aplicável modifique Dados de Destino, mas o capítulo de Iniciativa não esclarece se Perícias podem ser aplicadas à rolagem ou se a Iniciativa deliberadamente não utiliza Perícia.

**Dúvida:** devemos declarar explicitamente quais fontes podem ou não melhorar a Iniciativa?

---

## D15 — Cada cenário deve concretizar as faixas de Alcance?

**Perspectiva:** Narrador + jogador  
**Arquivos relacionados:** `alcance-e-movimento.md`, construção futura de cenário

Toque, Curto, Médio e Longo são abstratos por design, e a distância concreta depende do cenário, da cena e do meio utilizado.

**Dúvida:** o capítulo de criação de cenário deverá fornecer exemplos ou referências próprias de alcance para que jogadores compartilhem uma expectativa comum, especialmente em cenários com escalas muito diferentes?

Exemplo: “Longo” numa perseguição medieval e “Longo” numa batalha espacial podem representar ordens de grandeza completamente diferentes.

---

## D16 — Proteção 4/8/12 é universal ou referência de cenário?

**Perspectiva:** Narrador + criador de cenário + jogador  
**Arquivos relacionados:** `combate.md`, `mecanica-dos-itens.md`, `patamar.md`

O núcleo atualmente estabelece Armadura Leve 4, Média 8 e Pesada 12. Ao mesmo tempo, estamos reforçando que o Patamar do cenário baliza a escala do mundo e que os equipamentos concretos pertencem ao cenário.

**Dúvida:** os valores 4/8/12 devem continuar sendo valores universais de Proteção para categorias de armadura, ou são melhor entendidos como uma referência estrutural que cada cenário aplica aos seus equipamentos?

Nenhuma mudança deve ser feita antes de comparar essa questão com o funcionamento atual de Dano, Vida e Proteção.

---

## D17 — Falta um fluxo completo de criação de personagem?

**Perspectiva:** Jogador criando personagem  
**Arquivos relacionados:** `atributos.md`, `pericias.md`, `vida-e-mana.md`, `poderes.md`, `equipamentos-e-fabricacao.md`

As partes principais existem em arquivos separados, mas um jogador novo ainda precisa descobrir a ordem correta por conta própria.

**Dúvida:** quando a criação estiver mecanicamente fechada, precisamos de um capítulo/roteiro único que diga, em ordem, como escolher Patamar, distribuir Atributos, calcular Perícias, definir Poderes, calcular Vida/Mana e determinar recursos/equipamentos iniciais?

Esta dúvida é principalmente **editorial**, mas afeta diretamente a capacidade de alguém criar um personagem sem ajuda externa.

---

## D18 — Recursos iniciais do personagem pertencem totalmente ao cenário?

**Perspectiva:** Jogador + criador de cenário  
**Arquivos relacionados:** `equipamentos-e-fabricacao.md`, futuro capítulo de criação de personagem

O capítulo de Recursos estabelece que o cenário determina moeda, preços, disponibilidade e importância econômica, mas ainda não existe uma regra geral de quanto um personagem começa possuindo.

**Dúvida:** dinheiro, equipamentos, propriedades e demais recursos iniciais devem ser definidos inteiramente pelo cenário/Histórico, ou o núcleo precisa fornecer algum procedimento mínimo de criação?

---

# Ordem Recomendada de Discussão

A prioridade proposta é analisar primeiro as dúvidas que afetam o **motor universal**, depois criação e só então subsistemas específicos:

1. D01 — significado preciso de Patamar;
2. D02 — função completa do Patamar de Cenário;
3. D03 — escolha de Resistências do mundo;
4. D04 — consequências de resultados negativos;
5. D05 — nota obsoleta em Dados de Destino;
6. D09 — notação de disputas/Cura;
7. D12 — Status, Azar e impossibilidade;
8. D13 — Surpresa;
9. D14 — Iniciativa e Sorte/Perícias;
10. D06 — orçamento de Perícias;
11. D07 — INT e evolução de Perícias;
12. D08 — aquisição inicial de Poderes;
13. D10 — recuperação mínima;
14. D11 — duração-base de Poderes;
15. D15 — Alcance por cenário;
16. D16 — escala de Proteção 4/8/12;
17. D17 — fluxo completo de criação;
18. D18 — recursos iniciais.

Essa ordem é apenas um roteiro de revisão. Cada item deve ser discutido separadamente e pode mudar de prioridade conforme outras decisões forem tomadas.

---

## Regra desta Auditoria

Quando uma dúvida for encerrada:

1. comparar todas as regras relacionadas;
2. chegar a uma conclusão antes de editar o núcleo;
3. atualizar todos os arquivos realmente afetados;
4. registrar a decisão de forma coerente;
5. marcar a dúvida neste documento como **RESOLVIDA**, mantendo um resumo curto da decisão para preservar o histórico.

> **Dúvidas são preservadas aqui. Regras só mudam depois da conclusão.**
