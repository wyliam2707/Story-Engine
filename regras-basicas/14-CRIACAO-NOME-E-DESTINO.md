# 14 — Criação: Nome e Destino Canônico

Esta é a terceira etapa autoral de NOVA HISTÓRIA. Entra depois de Premissa e Estilo/Tom aprovados. A estrutura de campanha segue `25-MEMORIA-DE-CAMPANHA.md` e `07-CRIAR-CAMPANHA.md`.

> **O nome dá identidade humana à obra; o slug dá identidade técnica. Criar o destino não inicia a Ficção.**

## Nome

Se o Diretor já deu um nome claro, usá-lo sem tentar melhorá-lo por hábito. Se ainda não existe, propor poucas opções realmente diferentes a partir da Premissa e do tom aprovados. Não inventar profecia, lugar, segredo ou trama para produzir um título atraente.

Um nome provisório pode ser usado para persistência quando o Diretor autorizar. O título humano pode mudar depois; o slug permanece estável por padrão.

## Slug e destino

Preferir slug legível, único, em minúsculas, sem acentos quando necessário, com palavras separadas por hífen e sem pontuação desnecessária. Não exigir aprovação ritual de cada hífen quando a escolha for inequívoca.

Verificar se `campanhas/<slug>/` já existe antes de criar. Não sobrescrever outra obra. Se houver conflito, propor alternativa ou consultar o Diretor. Se a pasta é a obra que ele quer continuar, usar o ramo de retomada.

Depois de nome e destino suficientes, criar primeiro:

```text
campanhas/<slug>/INICIO.md
```

Conteúdo mínimo: nome, STATUS EM PREPARAÇÃO, Premissa aprovada e Estilo/Tom aprovado. Acrescentar outras decisões já tomadas, sem inventar o que permanece aberto. O modelo está em `modelos/CAMPANHA/INICIO.md`.

## Persistência progressiva

A partir do nascimento, as próximas etapas usam as fontes vigentes: `canon/personagens/`, `canon/direcao.md`, `canon/mundo/`, `canon/relacoes/`, `estado/`, `operacao.md` e `livro/` conforme necessidade. Não criar toda a árvore com conteúdo fictício nem iniciar a primeira cena.

Uma mudança posterior de título não exige renomear a pasta. Uma migração de slug deve preservar os arquivos e atualizar referências pertinentes.

## Conclusão

A etapa está concluída quando existe nome aprovado ou provisório autorizado, slug único, destino livre, entrada persistida com somente fatos aprovados e nenhuma Ficção iniciada. Seguir para Personagens Centrais.
