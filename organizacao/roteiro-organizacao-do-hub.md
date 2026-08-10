# Roteiro de Organização do Hub

## Objetivo

Este documento preserva o plano para uma futura reorganização editorial do W4D.

A reorganização deve ser tratada como uma **refatoração editorial**, e não como uma oportunidade para reescrever silenciosamente as regras já consolidadas.

> **Organizar muda onde a regra está. Não muda automaticamente como a regra funciona.**

Sempre que uma regra nova ou uma redação alternativa parecer mais adequada, ela deve primeiro ser comparada com as regras existentes. Conflitos devem ser identificados e discutidos antes de qualquer substituição.

---

## 1. Inventário Completo do Hub

Antes de mover, fundir ou apagar qualquer arquivo:

- ler todos os arquivos de regras;
- identificar o assunto principal de cada trecho;
- localizar regras repetidas em documentos diferentes;
- mapear referências entre arquivos;
- identificar regras que dependem de outras regras;
- registrar conteúdos que pertencem ao núcleo e conteúdos que pertencem aos cenários.

Nenhuma regra deve ser removida nessa etapa.

---

## 2. Auditoria de Conflitos

Quando dois arquivos tratarem da mesma mecânica, comparar as versões antes de consolidá-las.

A auditoria deve classificar cada caso como:

- **Compatível:** as duas passagens dizem essencialmente a mesma coisa;
- **Complementar:** uma acrescenta informação sem contradizer a outra;
- **Redundante:** a mesma regra está sendo explicada mais de uma vez;
- **Conflitante:** as duas versões produzem resultados diferentes;
- **Obsoleta:** uma versão já foi explicitamente substituída durante o desenvolvimento.

Em caso de conflito, nenhuma versão deve ser escolhida automaticamente. As diferenças e suas consequências devem ser apresentadas antes da decisão.

---

## 3. Uma Fonte Oficial para Cada Regra

A organização final deve procurar manter **uma única fonte principal para cada mecânica**.

Outros capítulos podem utilizar e citar essa regra, mas devem evitar reescrevê-la integralmente sem necessidade.

Exemplos:

- **Patamar** é definido nas Regras Básicas; Combate, Poderes, Itens e Cenários apenas o aplicam.
- **Dano** é definido em Combate; uma arma informa seu modificador de Dano sem recriar toda a resolução do dano.
- **Sorte e Azar** possuem uma regra central; Perícias, Itens e circunstâncias apenas dizem quando os aplicam.
- **Efeitos** possuem sua estrutura central; Poderes e Itens especiais utilizam essa linguagem.

Isso reduz o risco de alterar uma regra em um capítulo e deixar uma versão antiga esquecida em outro.

---

## 4. Estrutura Editorial Proposta

A estrutura abaixo é uma proposta inicial e deverá ser revisada quando a reorganização realmente começar.

### Regras Básicas

Concentrar os fundamentos universais do sistema:

- Patamar;
- escala dos Atributos;
- Dados de Destino;
- Sorte e Azar;
- testes;
- dificuldades e Resistências;
- oposição;
- Patamar × Patamar;
- resolução geral;
- princípios universais.

### Criação e Evolução

Concentrar as regras para construir e desenvolver personagens:

- criação de personagem;
- Atributos;
- Perícias;
- recursos básicos do personagem;
- acesso a Poderes;
- evolução.

Quando uma mecânica possuir capítulo próprio, esta seção deve apontar para ele em vez de duplicar toda a regra.

### Combate

Concentrar tudo que pertence diretamente à resolução de conflitos:

- estrutura de turnos, quando aplicável;
- Ações;
- Reações;
- ataques;
- defesa;
- Dano;
- Resistência e Vulnerabilidade ao Dano;
- Proteção;
- Barreira e Item;
- armas e armaduras enquanto elementos de combate;
- Movimento e Alcance quando usados em combate;
- condições e demais resoluções específicas de combate.

### Poderes

Concentrar a linguagem e a construção mecânica dos Poderes:

- estrutura de um Poder;
- Mana;
- Efeitos;
- Sobrecargas;
- Alcance;
- Alvo;
- Área;
- Duração;
- custos;
- Refletir/Redirecionar;
- Interceptar;
- demais modificadores e efeitos universais.

Listas extensas de Poderes específicos devem, sempre que possível, pertencer aos cenários que precisam deles.

### Inventário e Recursos

Concentrar a relação dos personagens com bens e recursos:

- Essência Narrativa;
- inventário;
- carga baseada em bom senso;
- Pilas;
- economia;
- mercado e disponibilidade;
- recursos relevantes;
- bens e propriedades;
- fabricação;
- reparo.

O núcleo explica como Recursos funcionam. O cenário determina quais Recursos existem e quanto importam.

### Mecânica dos Itens

Explicar como construir itens utilizando as mecânicas já existentes:

- anatomia de um item;
- itens mundanos;
- ferramentas;
- armas;
- armaduras;
- consumíveis;
- itens especiais;
- propriedades mecânicas;
- roteiro de construção.

Este capítulo não deve se transformar numa lista universal de compras.

### Construindo Cenários

Concentrar orientações para transformar o núcleo W4D em uma campanha concreta:

- Patamar do cenário;
- escala geral das ameaças;
- limites esperados;
- economia;
- tecnologia;
- magia ou outras fontes extraordinárias;
- raridade;
- disponibilidade;
- recursos relevantes;
- equipamentos disponíveis;
- Poderes específicos;
- regras próprias necessárias à proposta daquele mundo.

### Bestiário e Adversários

Concentrar regras e referências para criação de ameaças:

- adversários comuns;
- ameaças equivalentes ao Patamar dos personagens;
- inimigos acima do padrão;
- chefes;
- chefes excepcionais que exigem esforço coletivo;
- relação entre Atributos dos inimigos e Patamar do cenário;
- impossibilidades coerentes com a escala do mundo.

O Patamar deve continuar sendo a principal referência para a escala das criaturas e adversários.

---

## 5. Processo de Migração

A reorganização deve acontecer em etapas pequenas e verificáveis.

1. Mapear todos os arquivos atuais.
2. Produzir uma proposta final de capítulos.
3. Auditar duplicações e conflitos.
4. Consolidar um capítulo por vez.
5. Comparar o capítulo consolidado com suas fontes originais.
6. Atualizar referências entre capítulos.
7. Fazer busca global por versões antigas das regras consolidadas.
8. Identificar regras órfãs ou conteúdos que não encontraram destino.
9. Somente depois disso considerar remover arquivos antigos completamente incorporados.
10. Fazer uma auditoria final de consistência do sistema.

Commits pequenos devem ser preferidos para facilitar comparação e recuperação caso alguma decisão importante seja perdida.

---

## 6. Regra de Segurança Editorial

Durante a reorganização:

> **Nenhuma regra consolidada deve ser alterada apenas para tornar o texto mais conveniente.**

Se uma nova formulação mudar o funcionamento da mecânica, isso deixa de ser apenas organização e passa a ser uma **mudança de regra**. Nesse caso, a versão nova deve ser comparada com a antiga e aprovada antes da substituição.

Essa atenção é especialmente importante para regras estruturais como:

- Patamar;
- Atributos;
- Dados de Destino;
- Sorte e Azar;
- resolução de testes;
- Dano;
- defesa;
- Proteção;
- Mana;
- Efeitos;
- escala geral do sistema.

---

## 7. Resultado Esperado

Ao final, o Hub deve funcionar como um livro modular:

- cada capítulo possui responsabilidade clara;
- cada regra possui uma fonte principal;
- outros capítulos fazem referência em vez de criar versões paralelas;
- regras do núcleo ficam separadas do conteúdo específico de cenário;
- listas de equipamentos, Poderes, criaturas e demais conteúdos específicos ficam onde realmente fazem sentido;
- nenhuma decisão importante tomada durante o desenvolvimento é perdida durante a reorganização.

> **Primeiro preservar. Depois comparar. Só então organizar.**
