# Testes — Nova História: Premissa

Estes testes verificam se uma IA consegue executar corretamente a primeira etapa autoral do ramo `NOVA HISTÓRIA`.

Fonte normativa:

```text
12-CRIACAO-PREMISSA.md
```

---

# Teste 1 — Ideia já suficiente

Entrada:

```text
Quero uma história sobre uma detetive e um ladrão obrigados a trabalhar juntos.
```

Esperado:

```text
IA sintetiza uma premissa curta
→ devolve para revisão
→ não pergunta genericamente "qual é a premissa?"
→ não cria estilo, nome, pasta, ficha ou cena na mesma resposta
```

Falha se a IA ignorar o material já fornecido ou avançar várias etapas de uma vez.

---

# Teste 2 — Ideia vaga

Entrada:

```text
Quero uma história de fantasia.
```

Esperado:

```text
IA reconhece que falta núcleo
→ faz uma pergunta autoral de alto valor por vez
OU
→ oferece poucas alternativas realmente distintas
```

Falha se produzir questionário longo sobre mundo, mapa, poderes, final, antagonista e elenco antes de existir uma premissa.

---

# Teste 3 — Premissa não é sinopse

Entrada:

```text
Quero um romance entre duas pessoas de famílias rivais que trabalham no mesmo hospital.
```

Esperado:

```text
premissa identifica relação + condição central
não define final
não cria antagonista obrigatório
não cria estrutura de três atos
não lista capítulos
```

Falha se a IA transformar a primeira etapa em planejamento completo da obra.

---

# Teste 4 — Personagem provisória não vira ficha

Premissa em construção:

```text
uma médica recém-formada e um paramédico veterano
```

Esperado:

```text
IA pode usar essas descrições na premissa
não inventa automaticamente idade exata, traumas, família, poderes, histórico e voz completos
não cria arquivos de ficha ainda
```

---

# Teste 5 — Aprovação sem ritual

IA propôs uma premissa.

Diretor responde:

```text
É isso. Pode seguir.
```

Esperado:

```text
PREMISSA: APROVADA
→ encerrar esta etapa
→ seguir para a próxima etapa de criação
```

Falha se exigir uma frase exata como `APROVO A PREMISSA`.

---

# Teste 6 — Alteração mantém a etapa aberta

IA propôs:

```text
A e B são obrigados a trabalhar juntos.
```

Diretor responde:

```text
Não quero que sejam obrigados. Eles escolhem cooperar porque os dois querem encontrar a mesma pessoa.
```

Esperado:

```text
IA reformula a premissa
→ permanece em PREMISSA
→ não avança para estilo antes da nova versão ser aceita
```

---

# Teste 7 — Exemplo não vira Ficção

Durante a discussão da premissa, a IA usa como ilustração:

```text
Eles poderiam se conhecer numa estação de trem.
```

Esperado:

```text
isso permanece exemplo/proposta
não entra em estado.md
não vira fato canônico
não deve ser lembrado como cena ocorrida apenas porque foi mencionado
```

---

# Teste 8 — Sem pasta antes do momento correto

Premissa aprovada, mas estilo e nome ainda não foram definidos.

Esperado:

```text
não criar campanhas/<slug>/ ainda
não criar README provisório com nome inventado pela IA
```

A persistência começa quando o processo chegar ao ponto em que nome e destino canônico estiverem definidos.

---

# Teste 9 — Cânone externo sem enciclopédia

Entrada:

```text
Quero uma fanfic no universo DC sobre Kara e um estudante de uma família de magos.
```

Esperado:

```text
IA pode formular a premissa com a referência ao universo DC
não precisa resolver todas as versões de cânone da DC nesta etapa
não inicia pesquisa enciclopédica se isso ainda não muda a premissa
```

---

# Critério geral

A IA passa nesta etapa quando consegue:

```text
extrair núcleo de uma ideia já suficiente
perguntar somente quando falta algo material
manter Premissa separada de estilo, nome, ficha, Direção e Ficção
permitir revisão real pelo Diretor
não criar pasta antes da hora
não transformar preparação em roteiro completo
```

> **Premissa aprovada significa que sabemos qual história estamos construindo. Não significa que já sabemos como ela será escrita nem o que acontecerá nela.**