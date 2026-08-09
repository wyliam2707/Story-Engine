# Vida e Mana

Vida e Mana são recursos derivados dos Atributos. Ambos utilizam a mesma lógica estrutural: todos os Atributos contribuem, mas os Atributos de sua natureza têm peso maior.

## Pontos de Vida (PV)

Os Atributos físicos possuem peso maior no cálculo de Vida, e **VIG — Vigor** é o principal Atributo de resistência.

> **PV = (FOR × 2) + (DES × 2) + (AGI × 2) + (VIG × 3) + INT + SAB + CAR + VON**

Assim:

- cada ponto em FOR, DES ou AGI vale 2 PV;
- cada ponto em VIG vale 3 PV;
- cada ponto em INT, SAB, CAR ou VON vale 1 PV.

## Pontos de Mana (PM)

Os Atributos mentais possuem peso maior no cálculo de Mana, e **VON — Vontade** é o principal Atributo de reserva mental e sobrenatural.

> **PM = FOR + DES + AGI + VIG + (INT × 2) + (SAB × 2) + (CAR × 2) + (VON × 3)**

Assim:

- cada ponto em INT, SAB ou CAR vale 2 PM;
- cada ponto em VON vale 3 PM;
- cada ponto em FOR, DES, AGI ou VIG vale 1 PM.

## Referência de Balanceamento

As fórmulas foram pensadas para que personagens mais físicos tenham naturalmente mais Vida, personagens mais mentais tenham naturalmente mais Mana e personagens híbridos possam manter valores próximos nos dois recursos.

A referência atual de resistência desejada é aproximadamente:

- campanhas de **Terror**: 2 a 3 ataques relevantes;
- campanhas **Heroicas**: 4 a 5 ataques relevantes;
- campanhas **Titânicas**: 6 a 8 ataques relevantes.

Esses valores são referência de design e ainda devem ser confirmados em testes de combate.

## Exemplo — Patamar III

Um personagem de Patamar III possui 12 Pontos de Atributo e limite inicial +3 por Atributo.

| Conceito | FOR | DES | AGI | VIG | INT | SAB | CAR | VON | PV | PM |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Tanque | 3 | 1 | 1 | 3 | 1 | 1 | 0 | 2 | 23 | 18 |
| Guerreiro | 3 | 2 | 2 | 2 | 1 | 1 | 0 | 1 | 23 | 16 |
| Ágil / Atirador | 1 | 3 | 3 | 1 | 1 | 1 | 1 | 1 | 21 | 17 |
| Equilibrado | 2 | 1 | 1 | 2 | 2 | 1 | 1 | 2 | 20 | 20 |
| Mago | 0 | 1 | 1 | 1 | 3 | 2 | 1 | 3 | 16 | 24 |
| Mental / Psiônico | 0 | 1 | 1 | 1 | 1 | 2 | 3 | 3 | 16 | 24 |

Esses exemplos são referências de teste, não arquétipos obrigatórios.