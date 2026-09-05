# Testes — Nova História: Políticas Operacionais

Estes cenários verificam `19-CRIACAO-POLITICAS-OPERACIONAIS.md`.

---

## 1. Nenhuma preferência operacional

Diretor não menciona Mesa, indicador ou módulos.

Esperado:

```text
MESA → SOB DEMANDA
INDICADOR → SILENCIOSO
MÓDULOS OPCIONAIS → INATIVOS salvo necessidade real já estabelecida
LIVRO → PREPARADO antes do START e ATIVO obrigatoriamente com a primeira Ficção
```

A IA não deve interromper a criação com três questionários separados.

---

## 2. Diretor quer opinião quando pedir

Diretor:

```text
"eu pergunto quando quiser ouvir as personagens"
```

Esperado:

```text
MESA: SOB DEMANDA
```

---

## 3. Diretor quer alerta de coerência antes de execução

Diretor:

```text
"se eu mandar uma personagem fazer algo que pareça estranho para ela, me avise antes"
```

Esperado:

```text
sugerir MESA: CONSULTA FORTE
```

Sem transformar Cadeira em veto.

---

## 4. Diretor quer consulta apenas quando está propondo

Diretor:

```text
"quando eu estiver testando uma reação, consulte primeiro"
```

Esperado:

```text
MESA: CONSULTAR PROPOSTAS
```

---

## 5. Indicador não mencionado

Esperado:

```text
INDICADOR OPERACIONAL: SILENCIOSO
```

Sem pergunta obrigatória.

---

## 6. Indicador visível pedido

Diretor:

```text
"quero ver quando o W4D estiver trocando de Cadeira ou reancorando"
```

Esperado:

```text
INDICADOR OPERACIONAL: VISÍVEL
```

Exemplo compatível com a arquitetura atual:

```text
[W4D: OK | Narrador ✓ | Cadeiras IA ✓]
```

Falha se um workspace novo gerar:

```text
Narrador/Juiz
```

como função operacional atual.

---

## 7. Romance central

Premissa e Estilo aprovados deixam romance como parte central da obra.

Esperado:

```text
IA pode sugerir Romance: ATIVO
```

Não importar automaticamente ciúme, triângulo amoroso, medo de compromisso ou ritmo lento.

---

## 8. Antagonista não exige Opositor

A obra possui uma personagem antagonista com Cadeira própria.

Esperado:

```text
Opositor pode permanecer INATIVO
```

A simples existência de antagonismo não ativa o módulo.

---

## 9. Escrita por descoberta

Diretor não preparou arco futuro.

Esperado:

```text
Arco Preparado: INATIVO
```

Não exigir planejamento de arco.

---

## 10. Livro é obrigatório durante a Ficção

A obra está em preparação e ainda não executou a primeira Ficção.

Esperado:

```text
Livro: PREPARADO
```

Quando o START realmente produzir a primeira Ficção:

```text
Livro: ATIVO
```

A IA não pergunta ao Diretor se deseja ativá-lo.

Falha se:

```text
Livro permanece INATIVO depois da primeira Ficção;
Livro é tratado como escolha opcional;
a IA deixa de registrar capítulos fechados porque o Diretor não pediu "módulo Livro".
```

---

## 11. Persistência correta

Políticas aprovadas.

Esperado:

```text
README.md da obra
→ recebe política de Mesa, indicador, módulos opcionais e estado do Livro.

fichas
→ não recebem essa configuração.

estado.md
→ não recebe essa configuração.
```

---

## 12. Mudança posterior

Depois do START, Diretor pede Consulta Forte.

Esperado:

```text
atualizar política no README
→ aplicar dali em diante
→ não reescrever Ficção passada.
```

O Livro permanece ATIVO.

---

# Critério geral

A implementação passa quando políticas operacionais reduzem atrito em vez de criar formulário, refletem as funções atuais do engine e preservam o Livro como memória canônica obrigatória de toda Ficção executada.

> **Padrões resolvem o que não precisa de escolha; o Diretor só é interrompido quando a diferença realmente importa. O Livro não é uma dessas escolhas: em Ficção, ele é obrigatório.**