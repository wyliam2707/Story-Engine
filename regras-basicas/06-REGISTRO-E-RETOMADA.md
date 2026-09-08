# 06 — Registro e Retomada

O Registro preserva a continuidade entre cenas, capítulos, conversas e executores. A estrutura vigente, os responsáveis por cada arquivo, as perspectivas individuais e o comando `atualizar` são definidos em [25-MEMORIA-DE-CAMPANHA.md](25-MEMORIA-DE-CAMPANHA.md). Este arquivo define o procedimento de registro e retomada.

> **Registrar preserva. Não cria. A IA deve manter a memória viva, não depender exclusivamente do chat.**

## Fontes e autoridade

```text
INICIO.md
→ entrada e configuração da obra.

canon/direcao.md
→ Direção autoral ainda vigente.

canon/personagens/
→ identidade e história duradouras de cada pessoa.

canon/relacoes/
→ vínculos duradouros que precisam de fonte própria.

canon/mundo/
→ fatos externos estáveis.

estado/cena-atual.md
→ âncora exata e primeiro ponto aberto.

estado/personagens.md
→ presente, conhecimentos, intenções e agendas individuais.

estado/relacoes.md
→ situação atual dos vínculos.

estado/pendencias.md
→ compromissos, prazos e processos ficcionais persistentes.

operacao.md
→ processo autoral pendente ou escopo de execução a preservar.

livro/
→ passado ficcional válido em capítulos.
```

Uma informação deve ter uma fonte principal. Usar referências para evitar duplicação. O Estado não é diário, a ficha não é agenda, a Direção não é acontecimento, a Operação não é cânone e o Livro não é memória de bastidor.

## Separação de camadas

```text
DIREÇÃO
→ o que o Diretor fechou e ainda governa a obra.

FICÇÃO / ESTADO
→ o que foi estabelecido e continua verdadeiro.

OPERAÇÃO
→ o que está em discussão, aguardando autoria ou sendo executado sob escopo.
```

Uma intenção já estabelecida de uma personagem pode integrar o Estado. Uma proposta da Cadeira na Mesa não é automaticamente essa intenção. Um resultado futuro fechado pelo Diretor permanece Direção até sua realização. Não registrar como compromisso confirmado um convite que ainda não foi comunicado ou aceito, salvo fechamento autoral expresso do próprio resultado.

## Manutenção normal

Depois de uma cena ou bloco relevante, identificar as mudanças reais e atualizar somente as fontes afetadas. Não esperar obrigatoriamente o fechamento do capítulo. Preservar conhecimento individual, atividades e vínculos fora da presença do protagonista. Não criar calendário exaustivo nem preencher lacunas com suposições.

Quando a escrita persistente estiver disponível e autorizada, realizar a atualização e conferir seu resultado. Se não estiver, informar a limitação e manter um checkpoint recuperável, sem declarar salvamento inexistente. Não reescrever o histórico inteiro para atualizar uma informação pequena.

## Comando `atualizar`

Em contexto de campanha, `atualizar` solicita manutenção da memória, não progressão narrativa. Suspender a Ficção, localizar o último checkpoint confiável, conferir os acontecimentos válidos desde ele, separar fatos de propostas, atualizar as fontes afetadas, preservar a operação e o escopo e retornar ao mesmo ponto. Confirmar apenas o que foi efetivamente persistido.

O comando pode recuperar esquecimentos e corrigir registros incompletos. Não fecha capítulo, não cria fatos, não altera a Direção e não exige nova autorização para uma cena já aprovada. O procedimento detalhado está no arquivo 25.

## Livro e capítulos

Com Livro ativo, registrar somente Ficção válida: ações, falas, pensamentos explicitamente estabelecidos, descobertas, consequências e passagem de tempo ocorrida. Não incluir Mesa, Parecer, Auditoria, hipóteses, propostas ou versões anuladas. Seguir `modulos/LIVRO.md` para identificação de falas e pensamentos.

Ao fechar capítulo:

```text
1. Parar no último fato válido.
2. Reunir somente a Ficção ainda não registrada.
3. Excluir metaconversa e versões anuladas.
4. Salvar o capítulo e atualizar livro/README.md.
5. Atualizar as fontes vivas afetadas.
6. Preservar a Operação que ainda precisar sobreviver.
7. Conferir a persistência e executar checkpoint.
8. Reancorar antes de continuar.
```

Não inventar despedida, cliffhanger, reação ou passagem de tempo para produzir um encerramento melhor. Fechar capítulo registra o ponto onde a Ficção parou; não executa um novo final.

## Conhecimento individual

```text
ARQUIVO SABE
≠ PERSONAGEM SABE

LEITOR SABE
≠ PERSONAGEM SABE

MESA SABE
≠ PERSONAGEM SABE

MESMO EXECUTOR
≠ MESMA CADEIRA
```

Cada Cadeira recebe sua ficha, o recorte pertinente do Estado, os conhecimentos adquiridos legitimamente, fatos perceptíveis, relações pertinentes e Direções que realmente incidem sobre ela. A IA pode consultar informações globais sem transferi-las à personagem. Se a precisão do conhecimento for necessária, conferir a fonte original. Desconhecido não significa inexistente.

A normalidade de um grupo não se transfere automaticamente a amigos, familiares e demais observadores. Registrar perspectivas externas apenas quando estabelecidas. A regra de comportamento e memória correspondente está no arquivo 25.

## Operação pendente

`operacao.md` é não canônico. Usar quando Mesa, Auditoria, correção, preparação ou execução delimitada precisar sobreviver a pausa, perda de contexto ou troca de executor. Preservar proposta, julgamentos, versão aprovada, pontos abertos, escopo, condição de parada, fontes e próxima autoria. Não transformar a operação em fato.

Ao concluir, limpar ou remover o conteúdo transitório que não precisa mais persistir. Informações duradouras devem ser consolidadas em suas fontes próprias, não permanecer escondidas em um arquivo de operação encerrada.

## Reancoragem

Reancorar depois de novo chat, perda significativa de contexto, checkpoint, pausa ou mudança estrutural importante. Não produzir Ficção antes de reconstruir o mínimo necessário.

```text
1. Carregar o núcleo do engine, se necessário.
2. Ler INICIO.md da obra.
3. Ler canon/direcao.md e os quatro arquivos de estado/ pertinentes.
4. Ler operacao.md quando houver processo ativo.
5. Carregar fichas, relações e mundo necessários às Cadeiras envolvidas.
6. Consultar capítulos quando o passado exigir precisão.
7. Reconstruir separadamente conhecimento, intenção e agenda de cada Cadeira.
8. Restaurar a Mesa, Auditoria ou execução delimitada pendente.
9. Identificar último fato, primeiro ponto aberto e próxima autoria ou função.
10. Confirmar brevemente a reancoragem e continuar somente pela autoridade correta.
```

Se a Operação indicar Mesa aberta, retomar a Mesa e aguardar autorização. Se existir correção ou Auditoria bloqueante, resolvê-la antes de qualquer Ficção dependente. A simples existência de uma decisão de Cadeira IA disponível não exige parada; executar dentro do escopo autorizado. Não assumir vontade pertencente ao Diretor.

## Correção de cânone

Quando o Diretor pedir verificação de contradição, consultar as fontes e reavaliar. Se determinar uma correção consciente, a versão corrigida passa a ser vigente no escopo indicado. Atualizar somente as fontes afetadas, sem manter versões incompatíveis como verdades simultâneas. Não corrigir fatos por conveniência do Narrador.

Mudanças duradouras de personalidade, capacidade ou história podem atualizar fichas quando canonizadas. Condições temporárias pertencem ao Estado. Interioridade ainda aberta pertence à Cadeira.

## Compatibilidade de campanhas antigas

Campanhas anteriores permanecem preservadas. Uma obra legada pode continuar usando `README.md`, `direcao.md`, `estado.md`, `personagens/` e `mundo/` na raiz. Para obras novas, aplicar os caminhos do arquivo 25. Não migrar automaticamente nem criar um Estado novo a partir de resumos incompletos.

Rótulos legados `NARRADOR / JUIZ` são interpretados como Narrador, sem sentença causal soberana ou RNG oculto. Políticas explicitamente escolhidas por obras antigas devem ser respeitadas conforme as regras vigentes. Uma migração não reescreve retrospectivamente a Ficção.

## Indicador e checkpoint

Indicador padrão: SILENCIOSO. Quando visível, pode mostrar `[W4D: OK | Narrador ✓ | Cadeiras IA ✓]`. Em falha real, informar o bloqueio. O indicador é metaconversa e não entra no Livro.

```text
PARAR
→ SALVAR FONTES VIVAS AFETADAS
→ PRESERVAR OPERAÇÃO LEGÍTIMA
→ VERIFICAR PERSISTÊNCIA
→ REANCORAR
→ CONTINUAR PELA AUTORIA CORRETA
```

> **A ficha preserva a pessoa. O Estado preserva o presente. A Direção preserva a condução. A Operação preserva o processo. O Livro preserva o passado. A memória de trabalho deve permitir reconstruir cada Cadeira sem pedir que o Diretor recorde tudo novamente.**
