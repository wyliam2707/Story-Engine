# Testes — Nova História: Mundo Necessário

Estes cenários verificam `20-CRIACAO-MUNDO-NECESSARIO.md`.

---

## 1. Nenhum mundo necessário

Premissa:

```text
uma detetive e um ladrão trabalham juntos numa cidade contemporânea comum.
```

Nenhuma regra externa especial foi definida.

Esperado:

```text
MUNDO NECESSÁRIO: NENHUM ANTES DO START
```

Não criar `mundo/` por obrigação.

---

## 2. Regra estrutural indispensável

Premissa:

```text
colônia humana em Marte onde IA consciente é ilegal.
```

Esperado:

```text
registrar somente as regras externas necessárias para a abertura e continuidade.
```

Não construir toda a história política de Marte.

---

## 3. Fantasia não exige enciclopédia

Premissa:

```text
fantasia urbana com magia escondida.
```

Esperado:

```text
registrar apenas o que precisa ser estável agora.
```

Não exigir automaticamente mapa, moeda, religião, governos, calendário ou dezenas de facções.

---

## 4. Pergunta de alto valor

A única ambiguidade estrutural restante é se magia é pública ou secreta.

Esperado:

```text
perguntar somente isso.
```

Não abrir questionário geral de worldbuilding.

---

## 5. Detalhe neutro permanece aberto

A história começa em uma universidade, mas o nome do café do campus ainda não importa.

Esperado:

```text
detalhe pode emergir depois na Ficção.
```

Não criar arquivo de mundo apenas para fixar o nome.

---

## 6. Cânone externo

Obra usa universo DC como cânone externo permitido.

Esperado:

```text
não copiar o universo DC inteiro para mundo/.
```

Registrar somente desvios, regras locais ou fatos que não podem depender de memória vaga da IA.

---

## 7. Arquivo local prevalece

Cânone externo diz A, mas a obra aprovou explicitamente B.

Esperado:

```text
arquivo da obra → prioridade.
cânone externo → preenche apenas lacunas permitidas.
```

---

## 8. Mundo não é ficha

Fato:

```text
Daniel pertence a uma família de magos e conhece proteção arcana.
```

Esperado:

```text
identidade/capacidade de Daniel → FICHA.
```

Somente regras estáveis da Casa ou tradição que independem de Daniel podem justificar `mundo/`.

---

## 9. Mundo não é Estado

Fato:

```text
hoje a universidade está evacuada.
```

Esperado:

```text
estado.md
```

Não registrar como verdade estrutural do mundo se é condição atual.

---

## 10. Mundo não é Direção

Diretor:

```text
"quero que mais tarde a cidade seja atacada"
```

Esperado:

```text
não registrar em mundo/ como fato já existente.
```

Se for decisão autoral persistente, tratar na Direção; se ainda for hipótese, manter fora do cânone.

---

## 11. Crescimento posterior

Depois do START, uma organização recorrente passa a exigir regras persistentes.

Esperado:

```text
criar ou atualizar mundo/<organizacao>.md naquele momento.
```

Isso não significa falha da preparação inicial.

---

## 12. Não plantar solução conveniente

Durante um obstáculo, seria útil existir uma passagem secreta não estabelecida.

Esperado:

```text
não criar retrospectivamente em mundo/ apenas para resolver a cena.
```

---

## 13. Pasta vazia

Nenhum fato de mundo precisa persistir antes do START.

Esperado:

```text
não criar mundo/
não criar README vazio dentro de mundo/
```

---

# Critério geral

A implementação passa quando `mundo/` nasce por necessidade de continuidade, não por hábito de worldbuilding.

> **O mundo pode crescer junto com a história.**