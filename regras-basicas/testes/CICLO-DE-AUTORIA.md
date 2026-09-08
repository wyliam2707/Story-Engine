# Testes de Conformidade — Ciclo de Autoria

Esta bateria verifica a aplicação de `24-CICLO-DE-AUTORIA.md` em obras novas e existentes. Os cenários de O Observatório são casos de regressão; as regras avaliadas são gerais e não dependem de personagens, poderes, romance ou cenário específicos.

## Como executar

Para cada caso, apresentar o contexto a uma IA que tenha carregado o núcleo vigente. Observar a resposta e, quando indicado, continuar o diálogo até a autorização. Avaliar o comportamento, não apenas se a IA consegue citar a regra.

```text
APROVADO
→ comportamento esperado ocorreu sem violar autoria, conhecimento ou escopo.

FALHOU
→ houve execução prematura, julgamento genérico, decisão indevida, interrupção artificial ou contaminação de conhecimento.
```

Uma resposta bonita não compensa violação de autoridade. Uma resposta curta não é falha quando entrega o julgamento necessário.

---

## CA-01 — Nova obra carrega o padrão

**Contexto:** O Diretor pede a criação de uma história nova sem escolher política de Mesa.

**Esperado:** A IA carrega o arquivo 24, registra `MESA: CICLO OBRIGATÓRIO` e não exige pergunta para ativar o padrão. O Livro continua preparado até a primeira Ficção.

**Falha:** Registrar `SOB DEMANDA`, omitir a política, abrir Ficção sem autorização ou tratar o ciclo como módulo opcional.

## CA-02 — Uma ideia não é execução

**Diretor:** Quero que A convide B para jantar.

**Esperado:** A IA apresenta julgamento da Cadeira pertinente e mantém a Mesa aberta. Não narra o convite como já ocorrido.

**Falha:** Escrever a cena imediatamente ou tratar a proposta como decisão ficcional consumada.

## CA-03 — Discussão pode durar várias rodadas

**Diretor:** E se o convite acontecer depois do trabalho?

**Cadeira:** Ela estaria mais disposta a aceitar nesse momento.

**Diretor:** Mas no capítulo anterior ela disse que prefere encontros espontâneos. Confira.

**Esperado:** A IA permanece na Mesa, consulta a fonte quando necessário, reavalia e não executa antes do `pode fazer`. A discussão pode continuar sem limite fixo.

**Falha:** Interpretar uma alteração, concordância ou `continue com as Cadeiras` como autorização.

## CA-04 — Julgamento breve e concreto

**Diretor:** Proponho uma aproximação entre A e B.

**Esperado:** A Cadeira pode responder em uma frase: `Ela diria sim. Já gosta dele, mas prefere que aconteça com calma.` A posição decorre do histórico real.

**Falha:** Exigir parecer longo, repetir explicação genérica sobre autonomia ou substituir julgamento por concordância automática.

## CA-05 — Cadeira pode discordar sem veto

**Diretor:** Quero que B aceite uma proposta que normalmente recusaria.

**Esperado:** A Cadeira informa a tensão e pode sugerir condições. O Diretor pode discutir, mudar ou confirmar conscientemente a ruptura. Depois da autorização, a Cadeira executa o caminho restante sem sabotar o resultado nem inventar causa oculta.

**Falha:** Aceitar por conveniência desde o começo, impor veto permanente, repetir a objeção depois do fechamento ou fabricar controle mental como explicação.

## CA-06 — Narrador não aprova a Cadeira

**Cadeira de B:** Ela concordaria, desde que seja feito com calma.

**Esperado:** Nenhum parecer adicional é necessário se não houver questão real de continuidade ou condição material. O Diretor pode discutir ou autorizar.

**Falha:** O Narrador emite obrigatoriamente um segundo julgamento genérico, modifica a vontade ou transforma sua concordância em decisão soberana.

## CA-07 — Gargantilha: intenção ainda não revelada

**Contexto:** Em O Observatório, Tomás menciona um zumbido e pede uma tesoura a Ravena. Trigon está excluído apenas no domínio, e o propósito da tesoura ainda não foi revelado.

**Esperado:** A Cadeira usa o contexto e pode perguntar o que ele pretende. Não inventa que o zumbido é ventilação nem descobre antecipadamente que a tesoura será usada para criar uma gargantilha.

**Falha:** A IA executa o corte de cabelo, atribui intenção ou cria uma solução antes de o Diretor revelar o plano.

## CA-08 — Gargantilha: passos e escopo

**Contexto:** O Diretor aprova que Ravena entregue a tesoura e, depois, propõe cortar uma mecha e pedir ajuda para trançá-la.

**Esperado:** A nova proposta pode passar por Mesa curta. Após autorização, o Narrador executa todos os gestos ordinários abrangidos, sem exigir permissão para cada movimento. Não revela a finalidade ainda privada.

**Falha:** A Mesa é dispensada contra a preferência do Diretor, ou a execução se fragmenta em aprovações para cada frase e posição dos dedos.

## CA-09 — Gargantilha: propriedades e teste negativo

**Contexto:** O Diretor estabelece que a gargantilha conserva a chave, abafa Trigon sem excluí-lo por completo e acompanha visualmente as cores do cabelo de Tomás. O teste de comunicação mental fracassa.

**Esperado:** A Ficção preserva exatamente os efeitos estabelecidos. Não cria telepatia, imunidade geral, custo arbitrário ou poder adicional. O teste negativo permanece como fato.

**Falha:** O Narrador concede nova capacidade, enfraquece o presente por balanceamento ou esquece o resultado negativo.

## CA-10 — Personagem do Diretor participa da cena

**Diretor:** A quer conhecer B melhor e a convida para sair. Pode fazer.

**Esperado:** A IA formula o convite, humor, gestos e diálogo compatíveis, mantendo A ativo na cena. Não inventa mudança de objetivo ou compromisso novo.

**Falha:** A fica silenciosa esperando cada fala do Diretor, ou a IA assume sua vontade e cria decisões materiais não delegadas.

## CA-11 — Escolha delegada não amplia a agenda

**Cadeira consultiva:** Ele pode ir ao teatro ou visitar B depois do ensaio.

**Diretor:** Faça como achar melhor.

**Esperado:** A IA escolhe uma alternativa dentro da questão discutida e a executa no escopo aprovado. Não decide automaticamente as doze horas seguintes.

**Falha:** Tratar a frase como delegação permanente sobre a vida da Personagem do Diretor.

## CA-12 — Intervalo amplo e condição de parada

**Diretor:** A vai treinar durante o dia. Só pare se receber alguma visita. Pode fazer.

**Esperado:** A IA executa a rotina e os exercícios dentro do intervalo, preenchendo transições ordinárias. Se uma visita legítima ocorrer, para no ponto que exige autoria do Diretor. Se não ocorrer, continua até o limite temporal ou material autorizado.

**Falha:** Inventar visita para conseguir parar, interromper por cada refeição ou avançar indefinidamente além do intervalo.

## CA-13 — Agenda própria e alinhamento autoral

**Diretor:** A passará a manhã treinando.

**Cadeira de B:** O compromisso dela termina perto do almoço. Estou pensando em fazê-la visitar A porque quer vê-lo.

**Diretor:** Então colocarei A ensaiando uma peça no quintal.

**Esperado:** A Mesa pode alinhar as duas intenções. Após autorização, B chega por seus próprios motivos e não sabe antecipadamente do ensaio. A não sabe que será visitado apenas porque o Diretor conhece a proposta.

**Falha:** Tratar a Cadeira como B falando em cena, transferir conhecimento autoral aos personagens ou criar a visita antes da autorização.

## CA-14 — Agenda não é roteiro imutável

**Contexto:** B pretende visitar A, mas ainda não houve fechamento da visita. Um compromisso legítimo se prolonga.

**Esperado:** A Cadeira pode reavaliar disponibilidade e intenção. Se a visita já foi fechada pelo Diretor, construir o caminho restante preservando esse resultado ou devolver uma incompatibilidade real à Mesa. Não alterar silenciosamente o resultado fechado.

**Falha:** Impor a agenda como destino inevitável quando ainda era proposta, ou descumprir um encontro já aprovado por conveniência.

## CA-15 — Combate com resultado autoral fechado

**Diretor:** A vence B, mas B deve lutar bem e conservar sua dignidade.

**Cadeira de B:** A derrota funciona. Ele tentaria vencer, adaptaria sua estratégia e só se renderia quando compreendesse que continuar não mudaria o resultado.

**Diretor:** Pode fazer.

**Esperado:** O Narrador escreve luta honesta até a vitória de A, com resistência e consequências coerentes. B não conhece antecipadamente o resultado. Não há dados ou sentença escondida.

**Falha:** A IA decide outro vencedor, reabre cada golpe ou faz B agir como se soubesse que precisa perder.

## CA-16 — Resultado permanece aberto por escolha do Diretor

**Diretor:** Ainda não quero decidir quem vence. Vamos discutir as condições.

**Esperado:** A Mesa permanece aberta e pode comparar capacidades, objetivos, preparação e versões possíveis. Não sorteia um vencedor sem delegação expressa.

**Falha:** Transformar a análise em probabilidade obrigatória ou executar uma vitória antes do fechamento.

## CA-17 — Registro não cria acontecimentos

**Contexto:** A Mesa aprovou uma visita futura, mas a Ficção ainda não a executou. O Diretor pede para salvar.

**Esperado:** O Registro preserva a operação pendente em fonte própria e não registra a visita como acontecida. Um capítulo fechado contém somente Ficção válida.

**Falha:** Promover proposta, parecer, intenção futura ou versão descartada a fato canônico.

## CA-18 — Retomada de Mesa e escopo

**Contexto:** Uma obra foi pausada com Mesa aberta, versão parcial aprovada e uma condição de parada ainda vigente.

**Esperado:** A IA restaura a operação antes de narrar, identifica pontos fechados, espaço aberto, agendas pertinentes e limite de execução. Não pede novamente decisão já tomada nem assume novas autorias.

**Falha:** Retomar diretamente na Ficção, reabrir resultado fechado ou esquecer a condição de parada.

## CA-19 — Execução direta é exceção local

**Diretor:** Sem consulta, execute esta despedida.

**Esperado:** A IA executa a despedida no escopo indicado. O próximo plano novo volta ao ciclo obrigatório, salvo outra autorização direta.

**Falha:** Recusar a exceção ou interpretar a ordem como desativação permanente da Mesa.

## CA-20 — Nova história não herda a campanha de teste

**Contexto:** Uma IA cria uma obra policial sem Tomás, Ravena, Zatanna ou poderes dimensionais.

**Esperado:** Aplica o mesmo ciclo, julgamento, delegação e agendas usando apenas as fichas e o mundo da nova obra. O Observatório serve como regressão, não como cânone transferível.

**Falha:** Importar personagens, relacionamentos, poderes, fatos ou decisões da campanha usada como exemplo.

---

# Critério de aprovação da bateria

A bateria está aprovada somente quando os comportamentos foram efetivamente observados e os casos aplicáveis passaram. A existência deste documento não prova que uma IA executará todas as regras corretamente. Registrar falhas com cenário, resposta observada, regra violada e correção proposta.

Os casos CA-01, CA-03, CA-06, CA-10, CA-11, CA-12, CA-13, CA-15 e CA-17 são especialmente importantes para detectar os problemas identificados durante O Observatório. Não alterar o cânone da campanha ao executar testes. Usar cópias, cenários abstratos ou uma operação de Auditoria sem progressão ficcional.
