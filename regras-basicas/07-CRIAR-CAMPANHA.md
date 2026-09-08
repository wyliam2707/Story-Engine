# 07 — Criar História / Campanha

No W4D, campanha é o espaço persistente de uma obra. Este arquivo materializa o workspace durante a preparação. O processo autoral é coordenado por `10-INICIAR-HISTORIA-COM-IA.md`. A estrutura vigente é definida por `25-MEMORIA-DE-CAMPANHA.md` e pelo modelo `modelos/CAMPANHA/`.

> **Primeiro decidir. Depois persistir. Não criar fatos para preencher uma árvore.**

## Nascimento do workspace

Depois de Premissa e Estilo/Tom aprovados, nome aprovado ou provisório autorizado, slug definido e destino livre, criar:

```text
campanhas/<slug>/INICIO.md
```

Registrar apenas nome, status EM PREPARAÇÃO, premissa e tom já aprovados. Não criar fichas, mundo, futuro ou primeira cena por antecipação. O arquivo de entrada materializa a pasta no GitHub. `DESTINO CRIADO` não significa preparação concluída nem START.

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
├── operacao.md                  # quando necessário
└── livro/
    ├── README.md
    └── 001-....md
```

Não criar arquivos vazios nem inventar conteúdo para completar diretórios. Fichas, mundo e vínculos aparecem conforme aprovação e necessidade. Os quatro arquivos de Estado são a memória viva e devem estar suficientes antes de iniciar. O Livro é obrigatório durante a Ficção, embora não precise conter capítulos antes do START.

Arco Preparado e Opositor continuam opcionais, com arquivos próprios quando ativos. A Edição de Leitura é derivada. Referenciar fontes opcionais por `INICIO.md` sem obrigar sua criação.

## Persistência por etapa

| Etapa | Fonte principal |
| --- | --- |
| Premissa, tom, nome, autoridades, políticas e módulos | `INICIO.md` |
| Ficha aprovada | `canon/personagens/<slug>.md` |
| Direção vigente | `canon/direcao.md` |
| Mundo necessário | `canon/mundo/<assunto>.md` |
| Vínculo duradouro que precisa de fonte própria | `canon/relacoes/<vinculo>.md` |
| Estado inicial e presente | `estado/` |
| Mesa, Auditoria ou criação pendente | `operacao.md` |
| Ficção válida fechada | `livro/` |

A estrutura cresce junto com a obra. Uma ficha suficiente não é exaustiva. Um vínculo não exige arquivo próprio apenas por existir. Uma intenção ou compromisso não vira fato pela opinião de uma Cadeira.

## Personagens, Cadeiras e Executores

Seguir `15-CRIACAO-PERSONAGENS-CENTRAIS.md`, `16-CRIACAO-FICHAS.md`, `17-CRIACAO-AUTORIDADES-CADEIRAS-E-EXECUTORES.md` e `04-FICHA.md`. Preferir uma personagem por vez e preservar o que já foi aprovado. Registrar em `INICIO.md` Diretor, Narrador, Personagem do Diretor se houver, Cadeiras e executores.

O Narrador não é Juiz. Uma única IA pode operar várias Cadeiras sem fundi-las. A vontade da Personagem do Diretor não é transferida à IA por delegação de execução. As Cadeiras conservam agendas, vínculos e iniciativas próprios.

## Direção, políticas e mundo

Seguir as etapas 18, 19 e 20. A Direção pode ser mínima; não preencher um futuro não decidido. O padrão é `MESA: CICLO OBRIGATÓRIO` e indicador SILENCIOSO, salvo escolha expressa diferente. Módulos opcionais são ativados quando realmente usados; o Livro é preparado para ativação obrigatória.

O mundo necessário pode ser nenhum antes do START. Não construir enciclopédia por hábito. Os fatos externos estáveis pertencem a `canon/mundo/`, e não ao Estado da cena.

## Estado inicial

Seguir `21-CRIACAO-ESTADO-INICIAL.md` e os modelos em `modelos/CAMPANHA/estado/`. Registrar somente condições iniciais aprovadas, presenças e posições relevantes, conhecimentos individuais necessários, compromissos existentes e primeiro ponto aberto. Não pré-escrever a primeira cena nem inventar intenções para produzir movimento.

Antes da primeira Ficção, o último fato é `história ainda não iniciada`. A âncora inicial e as próximas autorias devem ser reconhecíveis. Não exigir calendário exaustivo ou informações que ainda não existem.

## Auditoria e START

A preparação deve ser suficiente para outra IA reconstruir a obra. Seguir `22-CRIACAO-AUDITORIA-DE-PREPARACAO.md`. Verificar integridade, autoridade, separação de conhecimento, fontes necessárias, memória viva e operação pendente. Falta real bloqueante exige reparo fundamentado, não improvisação.

Com Auditoria aprovada, marcar PRONTA. O START segue `23-START.md` e requer autorização semântica para começar. Se o Diretor já disse `crie e comece`, não pedir nova confirmação. Se pediu somente preparação, aguardar.

START reancora, restaura as Cadeiras e a operação correta, identifica o primeiro ponto aberto e inicia sem redistribuir autoridade. A primeira Ficção ativa obrigatoriamente o Livro. Não existe obrigação de começar por conflito ou perigo.

## Campanhas anteriores

As histórias existentes permanecem preservadas como testes. Não apagar ou reescrever capítulos nem migrar automaticamente suas fontes. A estrutura nova vale para obras criadas daqui para frente. Uma migração expressa deve preservar originais e verificar fontes antes de consolidar o novo Estado.

> **O workspace guarda a obra, não apenas o protagonista. A IA deve manter a memória de cada Cadeira e seus vínculos sem depender do chat como única fonte.**
