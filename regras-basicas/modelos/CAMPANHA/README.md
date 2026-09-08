# Modelo de campanha

Este diretório é a referência de estrutura do W4D vigente. Ao criar uma obra, copiar/adaptar somente os documentos necessários e substituir instruções e campos de modelo por informações aprovadas. Não transformar exemplos em fatos da história.

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
├── operacao.md              # se houver processo a preservar
└── livro/
    ├── README.md
    └── 001-....md
```

`INICIO.md` nasce com a obra. A Direção e as fichas aparecem conforme a preparação. Os quatro arquivos de Estado são criados quando houver realidade inicial suficiente, inclusive quando algum deles apenas declarar que ainda não existem pendências estabelecidas. Diretórios de mundo e vínculos crescem por necessidade, não por obrigação de preencher conteúdo. O Livro ganha capítulos apenas depois de Ficção válida.

A fonte normativa é [25-MEMORIA-DE-CAMPANHA.md](../../25-MEMORIA-DE-CAMPANHA.md). A criação segue [07-CRIAR-CAMPANHA.md](../../07-CRIAR-CAMPANHA.md). Atualização e retomada seguem [06-REGISTRO-E-RETOMADA.md](../../06-REGISTRO-E-RETOMADA.md).
