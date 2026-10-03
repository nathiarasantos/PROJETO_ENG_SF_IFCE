# Planejamento do Sistema de Estoque Interligado: Matriz e Franquia

Este documento apresenta a persona do franqueado, o roteiro de entrevista de alinhamento e a proposta de solução técnica para resolver o impasse de visibilidade do estoque entre a matriz e a nova unidade física.

---

## 👤 1. Persona do Franqueado.

### RA - Franqueado.
* **Motivações:** 
  * Fazer o novo negócio prosperar rapidamente para reaver o capital investido.
  * Garantir o suporte prometido pela matriz.
  * Evitar a perda de vendas por falta de mercadoria local (ruptura de estoque).

---

## 📋 2. Roteiro de Entrevista: Matriz x Franqueado

### 2.1 Sobre a Gestão de Vendas
* **Pergunta da Matriz:** RA, por que para você é vital ter visibilidade em tempo real de cada item do estoque da nossa loja matriz?
* **Resposta do Franqueado:** "Porque se um cliente entrar na minha loja procurando um casaco tamanho G que acabou no meu estoque, eu preciso saber *imediatamente* se vocês têm esse item na matriz para eu oferecer uma transferência. Se eu não puder ver, eu perco a venda na hora para o concorrente."

### 2.2 Sobre a Confiança na Operação
* **Pergunta da Matriz:** Você aceitaria um modelo onde o sistema aponta apenas se o produto *está disponível para transferência*, sem abrir o saldo total de peças ou os custos da matriz?
* **Resposta do Franqueado:** "Isso resolve parte do problema comercial, mas me preocupa a transparência. Como vou saber se o sistema está me mostrando a verdade ou se a matriz está 'escondendo' estoque de produtos que vendem muito para abastecer a loja própria primeiro? Preciso ter certeza de que seremos tratados como parceiros iguais."

### 2.3 Sobre a Autonomia e Logística
* **Pergunta da Matriz:** Se permitirmos a visualização, você concorda que o pedido de transferência deve passar por uma aprovação prévia da matriz, ou você espera automatizar isso?
* **Resposta do Franqueado:** "Entendo que a matriz dita as regras, então uma aprovação faz sentido para não desfalcar vocês de surpresa. Porém, esse processo precisa ser rápido. Se o sistema rodar uma atualização de estoque apenas uma vez por dia, eu posso vender algo que vocês já venderam de manhã. A integração precisa ser ágil."

### 2.4 Buscando o Meio-Termo
* **Pergunta da Matriz:** E se criarmos um 'Estoque Regulador Centralizado' no sistema, onde uma parte do estoque da matriz fica carimbada como 'Disponível para Franquias'? Assim você enxerga esse lote global sem ver o estoque interno da nossa loja. O que acha?
* **Resposta do Franqueado:** "Me parece uma excelente alternativa. Se eu tiver visibilidade garantida sobre essa cota e o processo de envio for rápido, não preciso ver o estoque íntimo da loja de vocês. O que eu quero é segurança de abastecimento."
---

## 💡 3. Proposta de Solução Técnica (Níveis de Acesso)

Para proteger os dados estratégicos da matriz e atender à necessidade comercial do franqueado, o sistema deve adotar o modelo de **Visibilidade Restrita por Contexto**:

| Funcionalidade | Visão da Matriz | Visão do Franqueado |
| :--- | :--- | :--- |
| **Saldo da Loja Matriz** | Quantidade exata (Ex: 42 un.) | Status binário (Disponível/Indisponível) |
| **Dados Financeiros** | Custo, margem e preço de compra | Apenas preço de venda ao consumidor |
| **Solicitação de Transferência** | Aprova ou recusa pedidos recebidos | Cria pedidos e acompanha o status do envio |
| **Estoque Mínimo / Alerta** | Configura regras globais da rede | Configura apenas regras da própria loja |
