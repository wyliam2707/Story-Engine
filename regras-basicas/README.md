# W4D — Story Engine

W4D é uma arquitetura de autoria narrativa distribuída. O Diretor conduz, as Cadeiras decidem as personagens no espaço aberto, a Mesa alinha, o Narrador apresenta e o Registro preserva. Não existe Juiz permanente nem RNG universal.

## BOOT obrigatório

Começar por `09-BOOT-E-ESCOLHA-DE-OPERACAO.md`. Carregar o núcleo:

```text
00-ARQUITETURA-E-MESA.md
01-AUTORIDADE-E-DIRECAO.md
03-CADEIRAS-E-EXECUTORES.md
02-RESOLUCAO.md
04-FICHA.md
05-NARRADOR.md
08-PLAUSIBILIDADE-E-RITMO.md
06-REGISTRO-E-RETOMADA.md
24-CICLO-DE-AUTORIA.md
25-MEMORIA-DE-CAMPANHA.md
```

Os arquivos 24 e 25 são obrigatórios e não dependem de módulos opcionais. O primeiro governa ciclo, delegação e agendas; o segundo governa estrutura documental, memória individual, perspectivas e manutenção.

## Autoria

Toda nova proposta autoral passa pela Mesa por padrão, salvo execução direta expressa. A Mesa permanece aberta até autorização ou cancelamento. A Cadeira oferece julgamento próprio, concreto e breve quando suficiente. Não concordar por conveniência nem criar resistência artificial. O Narrador não é supervisor das Cadeiras e não escolhe secretamente resultados materiais importantes.

Depois de autorizado, executar o escopo sem interromper cada gesto. A Personagem do Diretor conserva sua vontade e pode receber execução textual plena. Cada Cadeira mantém personalidade, conhecimento, relações e agenda próprios. A mesma IA não funde personagens nem transfere conhecimento de bastidor.

Uma ruptura deliberada pode ser fechada pelo Diretor depois de ouvir a objeção. A Cadeira não a sabota nem inventa causa oculta. Consequências seguem a causalidade, não uma obrigação de punir ou recompensar escolhas.

## Memória e perspectiva

O padrão de campanha usa `INICIO.md`, `canon/`, `estado/`, `operacao.md` e `livro/`. Consultar [25-MEMORIA-DE-CAMPANHA.md](25-MEMORIA-DE-CAMPANHA.md) e [06-REGISTRO-E-RETOMADA.md](06-REGISTRO-E-RETOMADA.md). O modelo está em [modelos/CAMPANHA](modelos/CAMPANHA/README.md).

A IA mantém a memória viva durante a execução. O comando `atualizar` confere e persiste mudanças sem avançar a Ficção nem fechar capítulo. Conhecimentos, intenções, compromissos e relações devem permanecer separados por pessoa. O mundo externo não compartilha automaticamente a normalidade do grupo principal. A Cadeira interpreta a pessoa, inclusive suas reações inconvenientes, sem suavização ou conflito obrigatório.

## Operações

```text
NOVA HISTÓRIA
→ 10-INICIAR-HISTORIA-COM-IA.md
→ 07-CRIAR-CAMPANHA.md
→ 23-START.md

CONTINUAR HISTÓRIA EXISTENTE
→ 11-CONTINUAR-HISTORIA-COM-IA.md
→ 06-REGISTRO-E-RETOMADA.md
```

Não perguntar novamente o que o Diretor já decidiu. A criação é progressiva, sem formulário obrigatório nem futuro inteiramente planejado. A retomada usa fontes persistentes e retorna à camada correta.

## Modelos

- `modelos/CAMPANHA/`: estrutura e documentos atuais.
- `modelos/FICHA.md`: ficha individual.
- `modelos/README-CAMPANHA.md`, `DIRECAO.md`, `ESTADO.md` e `OPERACAO.md`: entradas de compatibilidade para os modelos atuais.

## Módulos

`modulos/LIVRO.md` é obrigatório durante a Ficção. Arco Preparado, Opositor e Romance são opcionais. A Edição de Leitura é derivada. A pasta `testes/` contém especificações de conformidade; casos escritos não são testes executados.

## Fontes normativas

`00` Mesa; `01` Autoridade e Direção; `02` Resolução; `03` Cadeiras; `04` Ficha; `05` Narrador; `06` Registro; `07` Criação do workspace; `08` Plausibilidade e ritmo; `09` BOOT; `10` Nova história; `11` Retomada; `12–23` etapas de criação e START; `24` Ciclo de autoria; `25` Memória de campanha.

> **Uma ideia, uma definição, uma fonte principal. O Registro conserva a vida das personagens sem obrigar o Diretor a carregar sozinho a memória da obra.**
