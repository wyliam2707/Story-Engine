# W4D — Story Engine

W4D é uma arquitetura de autoria narrativa distribuída, criada a partir de RPG puramente narrativo. Pode ser usada para coautoria de histórias com IA, ficção seriada, fanfic, sala de roteiro e jogos narrativos.

> **O Diretor conduz. As Cadeiras decidem as personagens. A Mesa alinha o que precisa ser fechado. O Narrador apresenta a Ficção. O Registro preserva.**

O sistema não possui Juiz permanente, teste universal, dificuldade universal ou RNG para descobrir secretamente o resultado da história.

## BOOT

Uma IA deve começar por [regras-basicas/README.md](regras-basicas/README.md) e [09-BOOT-E-ESCOLHA-DE-OPERACAO.md](regras-basicas/09-BOOT-E-ESCOLHA-DE-OPERACAO.md). O núcleo inclui obrigatoriamente `24-CICLO-DE-AUTORIA.md` e `25-MEMORIA-DE-CAMPANHA.md`.

Depois do BOOT, quando o pedido ainda não identificar a operação, perguntar se o usuário deseja criar uma história nova ou continuar uma existente. Se já identificou, não repetir a pergunta.

## Autoria e execução

```text
IDEIA / DIREÇÃO / QUESTÃO
→ MESA com julgamento próprio das Cadeiras pertinentes
→ discussão e refinamento pelo tempo desejado pelo Diretor
→ autorização expressa
→ Ficção no escopo aprovado
→ Registro do que foi estabelecido
```

O padrão é `MESA: CICLO OBRIGATÓRIO`, salvo política diferente escolhida expressamente. O Diretor pode dispensar a consulta em um escopo local. A execução já autorizada não exige nova Mesa para cada gesto. `Faça como achar melhor` delega a escolha em discussão, não toda a vontade da Personagem do Diretor.

A Cadeira oferece julgamento próprio, não concordância automática nem resistência artificial. O Narrador pode emitir Parecer quando houver questão real, mas não aprova novamente a vontade de uma Cadeira. Resultados materiais importantes ainda abertos podem voltar à Mesa. Uma decisão fechada não autoriza a personagem a conhecer o futuro.

Uma única IA pode operar várias Cadeiras e o Narrador, mantendo conhecimento, vontade, relações e agendas separados. A Personagem do Diretor recebe execução textual plena dentro da delegação, sem transferência de sua vontade.

## Memória de campanha

O padrão vigente usa uma entrada curta, cânone duradouro, Estado vivo, Operação separada e Livro histórico. A IA deve manter esses registros durante a execução e consultá-los ao retomar, em vez de depender somente da memória do chat.

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
├── operacao.md                 # quando necessária
└── livro/
```

O modelo completo está em [modelos/CAMPANHA](regras-basicas/modelos/CAMPANHA/README.md). As regras estão em [25-MEMORIA-DE-CAMPANHA.md](regras-basicas/25-MEMORIA-DE-CAMPANHA.md) e [06-REGISTRO-E-RETOMADA.md](regras-basicas/06-REGISTRO-E-RETOMADA.md).

O comando **`atualizar`** suspende a progressão, confere o que mudou desde o último checkpoint, atualiza somente as fontes afetadas e retorna ao mesmo ponto. Não fecha capítulo nem cria Ficção. A manutenção normal continua sendo responsabilidade da IA.

A normalidade pertence à experiência de cada pessoa. Conhecimento, cultura, vínculos e perspectivas externas não são compartilhados automaticamente. Amigos e familiares podem surpreender-se, brincar, julgar, discordar ou aceitar conforme suas próprias Cadeiras. Não suavizar toda reação nem inventar conflito por obrigação.

## Criar e continuar

- [Criar uma história](regras-basicas/10-INICIAR-HISTORIA-COM-IA.md) e [materializar o workspace](regras-basicas/07-CRIAR-CAMPANHA.md).
- [Continuar uma história](regras-basicas/11-CONTINUAR-HISTORIA-COM-IA.md) e [reancorar](regras-basicas/06-REGISTRO-E-RETOMADA.md).

As histórias existentes são testes e permanecem preservadas. A nova estrutura é o padrão de agora em diante; migração de uma obra antiga exige decisão expressa e não reescreve seus acontecimentos.

## Módulos e fontes

O Livro é obrigatório com a primeira Ficção. Arco Preparado, Opositor e Romance são opcionais conforme a obra. A Edição de Leitura é derivada e não substitui o Livro canônico.

A pasta `regras-basicas/` contém as normas vigentes. O arquivo mais específico governa seu assunto; `24` governa ciclo, delegação e agendas, `25` governa a estrutura e manutenção da memória, e `06` governa registro e retomada. O histórico Git preserva versões anteriores, mas uma versão antiga não prevalece sobre uma regra vigente.

## Lema

> **Aprender antes de operar. Propor para ouvir. Discutir para construir. Determinar para fechar. Narrar para existir. Registrar para preservar.**
