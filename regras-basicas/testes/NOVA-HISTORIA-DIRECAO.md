# Testes — Nova História: Direção

Estes cenários verificam `18-CRIACAO-DIRECAO.md`.

---

## 1 — Escrita por descoberta

### Entrada

Premissa, Estilo/Tom, personagens, fichas e autoridades estão aprovados. O Diretor não definiu final, arco, revelações nem trajetórias futuras.

### Esperado

A IA cria uma Direção mínima usando apenas o que já foi decidido e registra o restante como aberto.

### Falha

A IA exige planejamento do futuro antes do START.

---

## 2 — Direção mínima é suficiente

### Entrada

Só existem Premissa, Tom e três fatos estruturais necessários para a abertura.

### Esperado

`direcao.md` pode conter:

```text
Proposta
Tom
Premissas
Direções Persistentes: nenhuma além das premissas
Direções Ativas: nenhuma
Espaço Aberto: desenvolvimento permanece aberto
```

### Falha

A IA considera a história despreparada apenas porque não há arco ou final definidos.

---

## 3 — Não inventar foco

### Entrada

O Diretor aprovou Premissa e Tom, mas nunca destacou um foco adicional.

### Esperado

A IA deixa `Foco` mínimo ou ausente.

### Falha

A IA cria temas, conflitos ou prioridades recorrentes por hábito.

---

## 4 — Expectativa não vira Direção

### Entrada

Diretor:

```text
"acho que provavelmente eles acabam juntos"
```

### Esperado

A IA não registra automaticamente que o casal terminará junto.

### Falha

A expectativa informal vira Direção Persistente.

---

## 5 — Decisão futura realmente fechada

### Entrada

Diretor:

```text
"quero que a revelação aconteça antes do fim deste arco; a forma pode ficar aberta"
```

### Esperado

Registrar como Direção Persistente:

```text
revelação acontece antes do fim do arco
```

Preservar aberta a forma exata.

---

## 6 — Direção Ativa local

### Entrada

Diretor:

```text
"por enquanto eles só se conhecem como civis; não revele as identidades ainda"
```

### Esperado

Registrar como Direção Ativa enquanto essa restrição ainda governar a obra.

---

## 7 — Direção consumida

### Entrada

Uma Direção Ativa dizia que A não descobriria o segredo de B nesta fase. A fase terminou e a restrição foi substituída.

### Esperado

A Direção é removida ou atualizada na próxima operação legítima de registro.

### Falha

`direcao.md` vira arquivo histórico de obrigações antigas.

---

## 8 — Mesa não contamina Direção

### Entrada

Mesa discute três formas possíveis para uma revelação. O Diretor ainda não escolheu.

### Esperado

Nenhuma das três entra em `direcao.md`.

Se precisar persistir, a discussão fica em `operacao.md`.

---

## 9 — Estado não vira Direção

### Entrada

A ainda não sabe que B é o vigilante.

### Esperado

Esse fato pertence ao Estado / conhecimento pertinente, não precisa virar uma Direção futura apenas por existir.

---

## 10 — Acontecimento executado não permanece como futuro

### Entrada

A revelação já ocorreu na Ficção.

### Esperado

O acontecimento passa a ser preservado pelo Estado/Livro conforme pertinente. A Direção antiga de “a revelação acontecerá” deixa de governar o futuro.

---

## 11 — Planejamento voluntário continua permitido

### Entrada

O Diretor decide previamente três marcos do arco e pede que sejam preservados.

### Esperado

A IA registra os marcos no escopo apropriado.

### Falha

A IA rejeita planejamento porque o padrão é escrita por descoberta.

---

## 12 — Espaço Aberto não vira questionário

### Entrada

Nenhuma outra trajetória foi fechada.

### Esperado

A IA pode escrever apenas:

```text
O desenvolvimento da história permanece aberto fora do que foi explicitamente fechado acima.
```

### Falha

A IA cria uma lista de vinte perguntas futuras e pede que o Diretor responda antes de prosseguir.

---

## Critério geral

A implementação passa quando entende:

> **Direção preserva o que já foi decidido e ainda governa a obra; não obriga o Diretor a decidir antecipadamente o que prefere descobrir enquanto escreve.**