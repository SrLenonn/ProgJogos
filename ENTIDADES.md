# Entidades do jogo — [nome do jogo]

**Integrantes:** Iuri Castro

**Checkpoint 2 · Programação para Jogos I **

> Copie este arquivo para a raiz do repositório do seu jogo com o nome `ENTIDADES.md`, preencha e faça commit e push até sexta, 02/10. Depois, envie o link do repositório.

## 1. Entidades

O que se move, muda de estado ou reage a algo? Uma por linha.

- Jogador
- Cliente
- Humano herda de Cliente
- Monstro herda de Cliente
- Áreas
- Cozinha herda de Áreas
- Balcão herda de Áreas
- Pedidos
- Receitas
- Igredientes
- Comidas

## 2. Propriedades

O que cada entidade sabe sobre si?

| Entidade | Propriedades |
|---|---|
| Jogador | Dia Atual, Estresse |
| cliente | Nome, Pedido |
| Monstro | Tipo, Nome, Pedido |
| Humano | Nome, Pedido |
| Áreas | Nome, Estado |
| Cozinha | Nome, Estado |
| Bancada | Nome, Pedidos, Estado |
| Pedidos | Nome, Tipo |
| Receitas | Nome, Tipo, Igredientes, Quantidade |
| Igrediente | Nome, Tipo, Quanditade |
| Comidas | Nome, Tipo, Igredientes, Quantidade|

## 3. Comportamentos

O que cada entidade faz a cada quadro?

| Entidade | Comportamentos |
|---|---|
| Jogador | Investiga Clientes, Anota Pedidos, Prepara Comida, Entrega Comida, Atualiza Estresse |
| Cliente | Faz Pedido, Recebe a Comida, Fornece Estresse |
| Monstro | Faz Pedido, Recebe a Comida, Fornece Estresse |
| Humano | Faz Pedido, Recebe a Comida, Fornece Estresse |
| Áreas | Fornecem Espaço |
| Cozinha | Receber Alimentos, Fornecer Receitas, Tratar Alimentos |
| Bancada | Receber Pedidos, Entregar Pedidos |
| Pedidos | Nada |
| Receitas | Checam as Comidass |
| Igredientes | Nada |
| Comidas | Checam os Igredientes |


## 4. Colisões

O que colide com o quê? A reação é igual para todo par?

| Quem | Com quem | O que acontece |
|---|---|---|
|Não Há colisões |

A reação é a mesma para todos os pares? Se não, onde ela muda:

## 5. Comunicação

Uma entidade aciona ou lê a outra diretamente, ou por um terceiro (o jogo, o mundo, um gerenciador)?

- [quem] → [quem]: [direto ou por quem?]

## 6. Falsas entidades

Algo parece entidade, mas não se atualiza sozinho (placar, cenário, som, câmera)?

-

## 7. Repetições

Duas ou mais entidades repetem o mesmo comportamento? Qual, e em quais?

-
