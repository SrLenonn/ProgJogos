# Entidades do jogo — Suspicious Kitchen

**Integrantes:** Iuri Castro e Kaique Fernandes

**Checkpoint 2 · Programação para Jogos I **

## 1. Entidades

O que se move, muda de estado ou reage a algo? Uma por linha.

- Jogador
- Cliente
- Humano herda de Cliente
- Monstro herda de Cliente
- Pedidos
- Receitas
- Ingredientes
- Comidas
- Ferramentas de cozinha

## 2. Propriedades

O que cada entidade sabe sobre si?

| Entidade | Propriedades |
|---|---|
| Jogador | Estresse |
| cliente | Nome, Perfil, Restrições, Preferências, Nível, Estado |
| Monstro | Espécie, Características |
| Humano | Características |
| Pedidos | Nome, Itens Solicitados, Status, Nível, Resultado |
| Receitas | Nome, Modo, Nível |
| Ingrediente | Nome, Categoria, Características |
| Comidas | Nome, Etapa, Ingredientes, Qualidade|
| Ferramentas | Nome, Função, Disponibilidade|

## 3. Comportamentos

O que cada entidade faz a cada quadro?

| Entidade | Comportamentos |
|---|---|
| Jogador | Interagir com Clientes, Anota Pedidos, Entrega Comida, Atualiza Estresse |
| Cliente | Faz Pedido, Avalia Atendimento, Realizar feedback, Encerrar atendimento |
| Monstro | '' |
| Humano | '' |
| Pedidos | Registra Itens, Atualiza Status, Verifica Conclusão, Valida Comida |
| Receitas | Consulta Ingredientes, Consulta Etapa, Valida o Preparo, Valida a Comida |
| Ingredientes | Nada |
| Comidas | Adiciona Ingredientes, Registra Etapa, Valida Finalização |
| Ferramentas | Seleção, Ação, Verifica Compatibilidade, Atualiza Estado do Ingrediente | 


## 4. Colisões

O que colide com o quê? A reação é igual para todo par?

| Quem | Com quem | O que acontece |
|---|---|---|
|Não Há colisões |

## 5. Comunicação

Uma entidade aciona ou lê a outra diretamente, ou por um terceiro (o jogo, o mundo, um gerenciador)?

- Jogador → Cliente : Direto
- Jogador → Comida : Direto
- Cliente → Pedido: Direto
- Pedido → Comida: Direto
- Pedido → Receita: Direto
- Rceita → Comida: Direto
- Receita → Ingrediente: Direto
- Comida → Ingrediente: Direto
- Ferramenta → Ingrediente: Direto

## 6. Falsas entidades

Algo parece entidade, mas não se atualiza sozinho (placar, cenário, som, câmera)?

- Cenários do Jogo: Balcão de atendimento, Cozinha
- Manuais de Interação: Manual de Investigação, Livro de Receitas
- Barras de Status: Barra de Stress

## 7. Repetições

Duas ou mais entidades repetem o mesmo comportamento? Qual, e em quais?

- As Entidades "Monstro" e "Humano" possuem similaridade de comportamento, ambos fazem pedido, verificam o pedido, e fornecem feedback ao jogador, ambas possuem ações herdadas de cliente
