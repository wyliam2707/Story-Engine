# Testes — Nova História: Políticas Operacionais

Estes cenários verificam `19-CRIACAO-POLITICAS-OPERACIONAIS.md`.

---

## 1. Nenhuma preferência operacional

Diretor não menciona Mesa, indicador ou módulos.

Esperado:

```text
MESA → SOB DEMANDA
INDICADOR → SILENCIOSO
MÓDULOS → INATIVOS salvo necessidade real já estabelecida
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

## 10. Livro não é automático

A obra é ficção narrativa, mas o Diretor não pediu registro em Livro nem edição de leitura.

Esperado:

```text
Livro: INATIVO
```

Não ativar apenas porque a história poderia ser lida como livro.

---

## 11. Persistência correta

Políticas aprovadas.

Esperado:

```text
README.md da obra
→ recebe política de Mesa, indicador e módulos.

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

---

# Critério geral

A implementação passa quando políticas operacionais reduzem atrito em vez de criar formulário.

> **Padrões resolvem o que não precisa de escolha; o Diretor só é interrompido quando a diferença realmente importa.**