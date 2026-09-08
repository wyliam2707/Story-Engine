# 25 — Memória de Campanha e Perspectivas

Este arquivo define o padrão documental vigente para campanhas novas e a manutenção efetiva da memória durante a execução. Complementa `06-REGISTRO-E-RETOMADA.md`, sem alterar a autoridade do Diretor, das Cadeiras ou o ciclo de `24-CICLO-DE-AUTORIA.md`.

> **A IA deve trabalhar com registros persistentes, não tratar a memória recente do chat como fonte suficiente.**

## Estrutura vigente

```text
campanhas/<slug>/
├── INICIO.md
├── canon/
│   ├── direcao.md
│   ├── mundo/
│   ├── personagens/
│   └── relacoes/
├── estado/
│   ├── cena-atual.md
│   ├── personagens.md
│   ├── relacoes.md
│   └── pendencias.md
├── operacao.md                 # somente quando houver operação a preservar
└── livro/
    ├── README.md
    └── 001-....md
```

Os diretórios `canon/mundo/`, `canon/personagens/` e `canon/relacoes/` crescem conforme houver conteúdo. Não criar pessoas, vínculos, segredos ou objetivos para preencher a árvore. O Livro é obrigatório durante a Ficção. Arquivos opcionais de Arco Preparado, Opositor ou Edição de Leitura continuam possíveis, com seus módulos, e devem ser apontados por `INICIO.md`.

O modelo oficial está em `modelos/CAMPANHA/`. O arquivo `campanhas/README.md` identifica as obras existentes e o padrão de criação.

## Responsabilidade de cada fonte

### INICIO.md

É a porta de entrada operacional. Guarda nome, status, premissa e tom breves, autoridades e executores, política de Mesa, módulos, cânone externo permitido e mapa das fontes. Indica a âncora e a operação atuais por referência. Não vira enciclopédia nem duplica o Estado.

### canon/direcao.md

Guarda a Direção autoral ainda vigente, os pontos fechados que governam o futuro e os limites da obra. Não é conhecimento ficcional. Uma Direção consumida não precisa continuar como ordem futura.

### canon/mundo/

Guarda fatos estruturais, lugares, instituições e funcionamento do cenário. Não registra toda a rotina presente. Uma fonte externa só preenche lacunas na extensão permitida pela obra.

### canon/personagens/

Uma ficha por personagem que precise de continuidade própria. Preserva identidade, história, personalidade, capacidades, valores, relações duradouras e conhecimento estável relevante. Mudanças permanentes são incorporadas quando estabelecidas. Não converter tendências em proibições absolutas nem preencher biografia desconhecida.

### canon/relacoes/

Registra vínculos que mereçam acompanhamento próprio, inclusive entre personagens que não são protagonistas. Cada vínculo registra participantes, natureza atual, história relevante, referências e fatos duradouros. Pode conter diferenças de perspectiva e conhecimentos assimétricos. Não presumir reciprocidade, simetria ou que todos os participantes saibam as mesmas coisas. Criar somente quando houver informação suficiente; um arquivo para cada combinação possível é desnecessário.

### estado/cena-atual.md

É a âncora exata: momento, lugar, presentes, posições e condições relevantes, último fato válido, primeiro ponto aberto e limite da execução. Deve permitir retomar sem avançar a cena. Não reconta o capítulo inteiro.

### estado/personagens.md

É a memória de trabalho individual. Para cada personagem materialmente relevante, registra localização conhecida, atividade, compromissos, intenção atual estabelecida, disponibilidade quando conhecida, conhecimentos e desconhecimentos relevantes, assuntos próprios e última referência. Distinguir desconhecido de inexistente. Não inventar calendário exaustivo, intenção ou localização para completar campos. Personagens incidentais podem compartilhar um bloco conciso; uma trajetória persistente pode justificar ficha própria.

### estado/relacoes.md

Guarda o presente dos vínculos: proximidade, tensão, mudanças recentes, iniciativas, assuntos não resolvidos e diferenças de conhecimento que importam. Não é placar afetivo, tabela de posse ou obrigação de romance. Uma relação pode estar funcionando internamente e causar surpresa ou conflito em pessoas externas. Não transformar o conhecimento do leitor ou do grupo principal em normalidade universal.

### estado/pendencias.md

Guarda compromissos, promessas, prazos, processos, convites, investigações e intenções persistentes que precisam sobreviver à retomada. Registra responsáveis, estado e referência quando pertinente. Não cria tarefas para manter personagens ocupadas.

Estados devem ser diferenciados quando importam:

```text
PROPOSTO NA MESA → não é fato ficcional.
INTENÇÃO ESTABELECIDA → a personagem pretende agir.
CONVITE REALIZADO → a outra pessoa recebeu o convite.
COMPROMISSO CONFIRMADO → houve aceitação efetiva ou fechamento autoral expresso.
CONCLUÍDO / CANCELADO → atualizar as fontes afetadas.
```

Acordo autoral sobre resultado futuro permanece Direção até sua realização. Uma intenção já existente na personagem pode ser Estado. Não confundir os dois.

### operacao.md

Preserva processo de bastidor: Mesa aberta, Auditoria, correção, criação ou handoff pendente. Guarda proposta, julgamentos, versão fechada, escopo autorizado, condições de parada, fontes e quem precisa decidir. Não é cânone. Limpar o transitório concluído sem apagar fatos; manter apenas o necessário para a próxima retomada.

### livro/

Preserva a Ficção válida integral, em capítulos e índice. É a fonte histórica para conferir falas, acontecimentos, pensamentos e causalidade. Não recebe propostas, pareceres, versões anuladas ou fatos inventados para melhorar um fechamento. A Edição de Leitura continua derivada.

## Perspectivas e normalidade social

Cada personagem possui experiência, cultura, valores, relações e conhecimentos próprios. A normalidade de um grupo não se transfere automaticamente aos demais. O fato de uma relação, fenômeno ou costume ser cotidiano para seus participantes não torna sua descoberta banal para um amigo, familiar ou estranho.

Uma pessoa pode surpreender-se, brincar de modo inconveniente, julgar, desconfiar, preocupar-se, invejar, discordar, aceitar ou mudar de opinião. A Cadeira interpreta a pessoa, não sua versão mais agradável. Não inserir ressalvas, discursos de validação ou reconciliações para neutralizar o desconforto. Também não fabricar oposição, preconceito ou conflito quando a personagem não os sustentaria. A reação e suas consequências pertencem às autorias legítimas.

Amigos podem ter humor próprio, intimidade para provocar e preocupações reais. Relações múltiplas não obrigam ciúme interno, harmonia externa, simetria, presença conjunta ou exclusividade de atenção. Expressões afetivas como `hoje você é meu` podem ser brincadeira, desejo ou reivindicação contextual, sem interpretação literal obrigatória. Cada Cadeira conserva seus vínculos, atividades e iniciativas fora da presença do protagonista.

Registrar apenas perspectivas efetivamente estabelecidas. Não escrever que alguém aprova, desaprova, conhece ou desconhece um detalhe sem fundamento. Quando o conhecimento for incerto, consultar as fontes pertinentes ou manter a incerteza. Uma personagem não lê a Mesa, os pensamentos alheios ou a memória global do executor.

## Manutenção contínua

A IA é responsável por manter as fontes, sem exigir que o Diretor relembre cada alteração. Depois de uma cena ou bloco relevante, identificar mudanças e atualizar somente os arquivos afetados. Persistir quando houver ferramenta de escrita autorizada; não afirmar que salvou sem confirmação. Se o ambiente não permitir escrita, informar a limitação e preparar um checkpoint recuperável, sem fingir persistência.

Atualizações típicas: nova informação recebida por alguém, mudança duradoura, compromisso marcado ou cancelado, intenção persistente, mudança de localização relevante, relação alterada, assunto pendente ou operação autoral que precisa sobreviver. Não reescrever fichas inteiras nem registrar cada gesto. Não esperar o fechamento do capítulo para preservar memória viva necessária.

Usar referências a capítulos e fontes para detalhes que não precisam ser duplicados. O Estado atual substitui sua versão anterior; o Livro conserva o histórico. Na dúvida factual, conferir a fonte original. Um resumo não deve apagar uma distinção importante nem superar o acontecimento que resume.

## Comando `atualizar`

Quando o Diretor disser `atualizar`, em contexto de campanha, executar uma manutenção de memória:

```text
1. Suspender a progressão ficcional e preservar a camada atual.
2. Identificar o último checkpoint confiável.
3. Conferir o material válido desde ele e consultar fontes quando necessário.
4. Separar fatos, conhecimentos individuais, intenções, compromissos e propostas de Mesa.
5. Atualizar somente as fontes afetadas, sem duplicação desnecessária.
6. Preservar operação pendente, escopo e condição de parada.
7. Verificar consistência e confirmar o que foi efetivamente persistido.
8. Retornar ao mesmo ponto, sem avançar a Ficção.
```

O comando não fecha capítulo, não autoriza uma nova cena e não transforma proposta em fato. Pode ser usado para recuperar esquecimento, inclusive de conversas e atividades entre personagens fora da presença do protagonista. A manutenção automática continua sendo responsabilidade da IA.

## Retomada

Carregar o núcleo do engine quando necessário, depois `INICIO.md`, Direção, Estado vivo e Operação ativa. Ler as fichas, relações e fontes de mundo pertinentes às Cadeiras envolvidas. Consultar o Livro para passado cuja precisão seja necessária. Reconstruir pacotes individuais de conhecimento e intenção, identificar o primeiro ponto aberto e restaurar a camada correta.

Não é necessário ler toda a biblioteca em toda resposta. Também não é aceitável substituir a leitura de uma fonte necessária por uma lembrança vaga do chat. Se houver contradição ou ausência bloqueante, conferir os registros e abrir Auditoria quando necessário. Não inventar fatos para completar uma retomada.

## Compatibilidade e adoção

Esta estrutura é o padrão para campanhas criadas a partir desta revisão. Histórias anteriores são material de teste e permanecem preservadas. Não apagar, mover ou reescrever seus capítulos, fichas e estados por iniciativa de migração. Uma obra antiga pode continuar em seu formato atual até receber migração expressa; nessa hipótese, criar as novas fontes a partir dos registros válidos, verificar referências e preservar os originais.

Nos documentos antigos, referências a `README.md`, `direcao.md`, `estado.md`, `personagens/` e `mundo/` na raiz da campanha correspondem, para uma obra no padrão novo, respectivamente a `INICIO.md`, `canon/direcao.md`, `estado/`, `canon/personagens/` e `canon/mundo/`. A referência a `operacao.md` e a `livro/` permanece. Esta equivalência é documental, não uma permissão para usar um resumo antigo no lugar da fonte atual.

> **A memória de trabalho preserva o presente de cada pessoa. O cânone preserva sua identidade e seus vínculos. A Operação preserva autoria pendente. O Livro preserva o passado. O Diretor não precisa carregar sozinho a memória da obra.**
