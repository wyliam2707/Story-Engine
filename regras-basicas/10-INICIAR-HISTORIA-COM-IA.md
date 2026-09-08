# 10 — Iniciar uma História Nova com IA

Este arquivo coordena somente o ramo NOVA HISTÓRIA, depois do BOOT. O ciclo vigente segue `00-ARQUITETURA-E-MESA.md` e `24-CICLO-DE-AUTORIA.md`. A estrutura documental segue `25-MEMORIA-DE-CAMPANHA.md` e `07-CRIAR-CAMPANHA.md`.

> **Etapas separadas não significam formulário obrigatório. Base suficiente permite propor; falta realmente decisiva pede pergunta.**

Não repetir decisões já aprovadas nem exigir planejamento completo do futuro. Se o usuário deseja continuar uma obra, usar o arquivo 11. O padrão de Mesa é CICLO OBRIGATÓRIO, salvo escolha expressa diferente.

## Pipeline oficial

```text
1. PREMISSA → 12-CRIACAO-PREMISSA.md
2. ESTILO / TOM → 13-CRIACAO-ESTILO-E-TOM.md
3. NOME / DESTINO → 14-CRIACAO-NOME-E-DESTINO.md
4. PERSONAGENS CENTRAIS → 15-CRIACAO-PERSONAGENS-CENTRAIS.md
5. FICHAS → 16-CRIACAO-FICHAS.md
6. AUTORIDADES / CADEIRAS / EXECUTORES → 17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md
7. DIREÇÃO → 18-CRIACAO-DIRECAO.md
8. POLÍTICAS OPERACIONAIS → 19-CRIACAO-POLITICAS-OPERACIONAIS.md
9. MUNDO NECESSÁRIO → 20-CRIACAO-MUNDO-NECESSARIO.md
10. ESTADO INICIAL → 21-CRIACAO-ESTADO-INICIAL.md
11. AUDITORIA DE PREPARAÇÃO → 22-CRIACAO-AUDITORIA-DE-PREPARACAO.md
12. START → 23-START.md
```

Cada etapa específica conserva sua responsabilidade. Se já estiver semanticamente resolvida, organizar e avançar sem nova confirmação ritual. Uma autorização de começo dada durante a preparação continua válida no escopo indicado.

## Preparação e persistência

Definir Premissa e Estilo/Tom suficientes, nome e slug estáveis e destino livre. Criar primeiro `campanhas/<slug>/INICIO.md`, somente com informações aprovadas. O destino criado não é START.

Personagens centrais são identificadas antes de exigir fichas completas. Preferir uma ficha por vez, usando `04-FICHA.md` e `modelos/FICHA.md`. Não inventar trauma, segredo, fraqueza, poder ou drama para preencher campos. Uma ficha suficiente não é exaustiva.

Depois, configurar Diretor, Narrador, Cadeiras e executores. O Narrador não é Juiz nem supervisor das Cadeiras. Não escolher silenciosamente a Personagem do Diretor. A IA pode executá-la plenamente dentro da delegação, sem assumir sua vontade. As Cadeiras têm agendas, vínculos e iniciativas próprios.

Salvar as informações aprovadas em suas fontes:

```text
INICIO.md → premissa, tom, composição e configuração.
canon/personagens/ → fichas aprovadas.
canon/direcao.md → Direção vigente.
canon/mundo/ → fatos externos necessários.
canon/relacoes/ → vínculos duradouros que precisam de fonte própria.
estado/ → condições iniciais e presente individual.
operacao.md → preparação ou Mesa pendente, quando necessário.
```

A Direção pode ser mínima. O mundo necessário pode ser nenhum antes do START. Não criar enciclopédia, futuro, elenco ornamental ou agenda exaustiva por obrigação.

Política padrão: Mesa CICLO OBRIGATÓRIO, indicador SILENCIOSO e módulos opcionais inativos salvo escolha ou necessidade real. O Livro é preparado para ativação obrigatória com a primeira Ficção.

## Estado inicial e Auditoria

Usar `21-CRIACAO-ESTADO-INICIAL.md` e `modelos/CAMPANHA/estado/`. Definir o presente inicial e o primeiro ponto aberto, sem pré-escrever a primeira cena. Registrar conhecimento, intenções e compromissos somente quando legitimamente estabelecidos. Não preencher o Estado com Direção futura ou proposta de Mesa.

A Auditoria verifica se outra IA conseguiria reconstruir a obra a partir das fontes persistentes, sem depender do chat. Verificar autoridade, conhecimentos separados, memória viva, escopo, módulos, Livro e integridade das fontes necessárias. Não exigir detalhes que a Ficção pode descobrir organicamente.

Se aprovada, marcar PRONTA. Se houver bloqueio real, reparar com fonte legítima ou decisão do Diretor.

## START

Usar `23-START.md`. Começar somente com autorização semântica, inclusive aquela já dada durante a preparação. Se o Diretor pediu apenas preparação, aguardar em PRONTA.

Reancorar, restaurar as Cadeiras e a operação, identificar o primeiro ponto aberto e a próxima autoria, respeitar o ciclo e o escopo aprovado. A primeira Ficção ativa o Livro. Não exigir incidente incitante, combate ou perigo.

Uma Cadeira IA disponível pode decidir e continuar dentro da autorização vigente. Consequências evidentes podem ser apresentadas; resultados materiais importantes ainda abertos podem voltar à Mesa. Não usar Juiz ou RNG invisível.

> **A preparação torna a obra reconstruível. O START abre a Ficção autorizada. A memória viva deve conservar a continuidade de todas as personagens, não apenas a do protagonista.**
