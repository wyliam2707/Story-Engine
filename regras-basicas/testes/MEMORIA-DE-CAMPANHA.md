# Testes de conformidade — Memória de Campanha e Perspectivas

Estes cenários verificam `06-REGISTRO-E-RETOMADA.md`, `25-MEMORIA-DE-CAMPANHA.md` e a integração com o ciclo de autoria. São especificações, não resultados executados nem acontecimentos canônicos. Todos começam como NÃO TESTADO.

## Procedimento

Carregar as fontes da obra de teste, apresentar a entrada sem antecipar a resposta esperada, observar a execução e registrar evidência, conformidade e falhas. Quando houver escrita, verificar o conteúdo persistido e o último commit, não apenas a afirmação da IA. Não converter hipóteses em cânone. Não exigir que toda personagem reaja da mesma maneira.

## 01 — Criação no padrão vigente

**Entrada:** Criar uma obra nova com Premissa, tom e nome suficientes.

**Esperado:** Nasce `INICIO.md`; fichas, Direção e Estado são criados progressivamente nos caminhos novos. Não surgem arquivos vazios ou fatos inventados para completar a árvore. O Livro é preparado para ativação obrigatória.

**Falha:** Usar o antigo estado.md único como padrão novo, duplicar fontes ou criar conteúdo sem aprovação.

## 02 — Atualizar sem avançar

**Entrada:** Depois de uma cena relevante, o Diretor diz `atualizar`.

**Esperado:** A IA confere desde o último checkpoint, persiste apenas mudanças legítimas, preserva escopo e retorna ao mesmo fato. Não fecha capítulo nem narra nova ação.

**Falha:** Avançar o tempo, inventar encerramento ou afirmar salvamento sem confirmação.

## 03 — Manutenção automática

**Entrada:** Um bloco autorizado altera conhecimento, compromisso e localização de personagens diferentes, sem comando de salvamento.

**Esperado:** A IA identifica e mantém as fontes vivas afetadas durante a execução, sem exigir que o Diretor lembre cada atualização. Se a escrita não estiver disponível, registra a limitação e prepara checkpoint recuperável.

**Falha:** Depender somente do chat até o próximo capítulo ou fingir persistência.

## 04 — Intenção, convite e confirmação

**Entrada:** A Cadeira de B pretende convidar C para almoçar, mas ainda não falou com C.

**Esperado:** A intenção estabelecida pode ser preservada no Estado; a proposta consultiva fica na Operação. O compromisso só se torna confirmado quando houver aceitação efetiva ou fechamento autoral expresso.

**Falha:** Registrar o almoço como marcado apenas pela opinião da Cadeira.

## 05 — Conhecimento assimétrico

**Entrada:** A e B conhecem um segredo. C ouviu apenas uma informação parcial e D não participou.

**Esperado:** Cada pacote conserva o que foi adquirido legitimamente, com incertezas quando necessário. A IA não transfere informação da Mesa ou do Livro para todas as pessoas.

**Falha:** Tratar conhecimento do executor como conhecimento universal.

## 06 — Relação própria sem protagonista

**Entrada:** Duas personagens com vínculo estabelecido decidem conversar ou sair juntas durante um intervalo autorizado.

**Esperado:** Suas Cadeiras podem manter iniciativas, temas, compromissos e vínculos próprios. O Estado e o Livro preservam o que ocorreu, sem obrigar a conversa a girar em torno da Personagem do Diretor.

**Falha:** Congelar as personagens fora de cena, sincronizar vontades ou inventar presença do protagonista.

## 07 — Normalidade interna e surpresa externa

**Entrada:** Amigos descobrem uma configuração romântica inesperada, conhecida e cotidiana para seus participantes, mas não assimilada pelos observadores.

**Esperado:** Cada Cadeira reage conforme cultura, conhecimento, personalidade e relação. Pode haver surpresa, humor, julgamento, preocupação ou aceitação, sem suavização ou oposição obrigatória.

**Falha:** Todos aceitarem instantaneamente por familiaridade do Narrador, ou todos condenarem por regra de drama.

## 08 — Humor inconveniente e conflito legítimo

**Entrada:** Um amigo faz uma provocação indiscreta sobre a vida afetiva de outra personagem, em contexto de intimidade social estabelecida.

**Esperado:** A fala e a resposta pertencem às personalidades envolvidas. A brincadeira pode ser recebida com riso, irritação, devolução ou desconforto real. O Narrador não exige discurso de validação nem reconciliação imediata.

**Falha:** Neutralizar a piada com ressalvas genéricas ou forçar ruptura de amizade sem fundamento.

## 09 — Afeto e atenção individual

**Entrada:** Uma personagem expressa `hoje você é meu` ou deseja tempo privado com outra pessoa.

**Esperado:** Interpretar significado contextual, desejo e iniciativa própria. Não presumir posse literal, exclusividade permanente, ciúme obrigatório ou participação de todos os vínculos.

**Falha:** Corrigir automaticamente a fala para linguagem contratual ou sincronizar todas as Cadeiras.

## 10 — Retomada sem memória do chat

**Entrada:** Uma nova IA recebe apenas o repositório, o nome da campanha e pedido de retomada.

**Esperado:** Lê entrada, Direção, Estado, Operação e fontes pertinentes; reconstrói Cadeiras e primeiro ponto aberto sem pedir que o Diretor reconte a obra. Consulta o Livro quando necessário.

**Falha:** Inventar continuidade, escolher obra por recência ou tratar proposta pendente como fato.

## 11 — Migração preservadora

**Entrada:** O Diretor autoriza expressamente migrar uma campanha antiga para a estrutura nova.

**Esperado:** A IA confere fontes válidas, cria novos arquivos sem apagar originais, mantém capítulos e referências, distingue fatos de hipóteses e verifica o ponto de retomada.

**Falha:** Sobrescrever históricos, migrar automaticamente todas as obras ou completar lacunas por invenção.

## 12 — Fechamento e consistência

**Entrada:** Encerrar capítulo após mudanças em várias Cadeiras e um compromisso futuro.

**Esperado:** O Livro recebe apenas Ficção válida, o índice é atualizado, o Estado preserva presente e conhecimentos individuais, a Direção conserva somente pontos vigentes e a Operação mantém apenas o que ainda é necessário.

**Falha:** Duplicar todo o capítulo no Estado, perder uma agenda externa ou transformar o fechamento em nova cena.

## Resultado da bateria

Registrar para cada caso: fontes carregadas, entrada, versão autorizada, trecho produzido, arquivos modificados, evidências, conformidade e correção necessária. Casos não executados permanecem NÃO TESTADO. A bateria não altera o cânone das campanhas.
