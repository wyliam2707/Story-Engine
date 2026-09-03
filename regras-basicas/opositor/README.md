# Opositor

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta contém **somente as regras e modelos da função opcional `OPOSITOR`**.

A função não é obrigatória em toda campanha.

> **Conflito, perigo ou antagonismo não exigem Opositor. Ativar esta função somente quando forças adversariais persistentes sem cadeira própria se beneficiarem de uma autoridade estratégica dedicada.**

Nenhum plano real, prazo real ou estado vivo de campanha deve ser salvo aqui.

```text
regras-basicas/opositor/
→ regras e modelos da função opcional.

campanhas/<nome>/opositor/
→ dados reais somente quando a campanha possuir Opositor ativo
  e houver informação adversarial persistente que precise de registro próprio.
```

A ausência de `campanhas/<nome>/opositor/` é válida e não indica campanha incompleta.

## Quando usar

Ativar Opositor quando houver forças adversariais persistentes que:

```text
não possuam cadeira própria
+
tenham objetivos, planos ou recursos próprios
+
continuem agindo além de uma reação local
+
se beneficiem de uma autoridade separada do Narrador / Juiz
```

Exemplos possíveis:

```text
facção organizada
quadrilha persistente
corporação adversarial
exército genérico
rede de perseguidores
força hostil recorrente sem personagem dedicada
processo adversarial organizado
```

Não ativar apenas porque existe:

```text
perigo ambiental
processo impessoal
conflito entre personagens com cadeiras próprias
dificuldade circunstancial
NPC que pode receber cadeira própria ou eventual
```

## Conteúdo

```text
registro-reservado.md
→ regra e modelo para o registro adversarial quando essa estrutura for usada.
```

Também pertencem a esta área, quando forem definidos e necessários:

- regras de controle de forças adversariais sem cadeira própria;
- uso de fichas e Poderes de oponentes sob esse escopo;
- escolha de alvos e prioridades;
- administração de recursos adversariais;
- planejamento fora de cena;
- fiscalização de prazos e consequências registradas.

## Ativação durante a campanha

Uma campanha pode começar sem Opositor e ativá-lo depois.

Nesse caso:

```text
CONFIGURAÇÃO DAS CADEIRAS
→ registrar OPOSITOR: ATIVO
→ registrar EXECUTOR
→ registrar ESCOPO
```

A ativação é prospectiva.

```text
ATIVAR OPOSITOR AGORA
≠
inventar que planos, recursos ou contramedidas sempre existiram.
```

Se deixar de existir necessidade funcional, a campanha pode desativar a função depois de consolidar os fatos que continuam verdadeiros no mundo e no Estado.

## Visibilidade

Os arquivos reais do Opositor dentro de uma campanha devem permanecer claros, visíveis e fáceis de localizar quando a função estiver ativa.

`Reservado` não significa oculto do responsável pela campanha ou protegido contra leitura.

Significa apenas que o conteúdo não pode ser usado como conhecimento de uma personagem que ainda não o descobriu na ficção.

```text
ARQUIVO VISÍVEL
≠
CONHECIMENTO DA PERSONAGEM
```

Isso permite revisar e auditar planos adversariais sem alterar as regras de conhecimento das cadeiras.

## Separação de autoridade

Quando ativo:

```text
OPOSITOR
→ decide o que forças adversariais sem cadeira própria dentro de seu escopo pretendem fazer.

CADEIRA DE PERSONAGEM
→ continua decidindo sua personagem mesmo quando ela é antagonista.

NARRADOR / JUIZ
→ julga possibilidade, meios, conhecimento, tempo e consequência.

CAMPANHA
→ preserva o que foi legitimamente estabelecido para aquele lado adversarial.
```

O conhecimento operacional do Opositor não se torna automaticamente conhecimento das forças que ele representa.

Quando a função estiver inativa:

```text
OPOSITOR
→ não participa.

PERSONAGENS COM CADEIRA
→ continuam decidindo por si.

MUNDO / ESTADO / PROCESSOS
→ continuam produzindo fatos e consequências.

CADEIRAS EVENTUAIS
→ podem assumir NPCs que precisem de agência própria.
```

> **Regra do Opositor fica aqui. Dados do Opositor só existem em `campanhas/<nome>/opositor/` quando a campanha realmente usa essa função.**