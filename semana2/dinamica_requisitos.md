# Dinâmica de Requisitos — Semana 2

## 1. Identificação do Sistema

**Sistema:** Sistema de Controle de Estoque para uma loja de eletrônicos de médio porte.

**Disciplina:** Engenharia de Software I

**Semana:** 2

## 2. Divisão de Papéis

| Integrante           | Papel                    |
| -------------------- | ------------------------ |
| Nathiara Santos      | Engenheira de Requisitos |
| Adna Cecilia         | Dona do Sistema          |
| Augusto Saul         | Usuário Final            |
| Fernando de Carvalho | Stakeholder Externo      |
| Mário Melo           | Gestor do Sistema        |

## 3. Personas

### 3.1 Dona do Sistema — Adna Cecilia
*Marina Alves, Proprietária da loja. Possui pouca familiaridade com sistemas complexos e busca uma visão clara do estoque, redução de perdas e informações confiáveis para auxiliar nas decisões.*

### 3.2 Usuário Final — Augusto Saul
*Gael Barbosa, Estoquista da Loja de eletrônicos, recentemente empregado, 
mais apto com tecnologias atuais.*

### 3.3 Stakeholder Externo — Fernando de Carvalho
*Ricardo Mendes, Consultor fiscal da loja. Precisa de informações organizadas e confiáveis sobre as movimentações do estoque para consultas, conferências e possíveis auditorias.*

### 3.4 Gestor do Sistema — Mário Melo
*Carlos Eduardo, Gerente operacional da loja e responsável pelo suporte técnico digital da loja. Acompanha o estoque, as compras e a equipe da loja, além de dar suporte à operação digital. Precisa de informações atualizadas sobre produtos, quantidades, movimentações e reposição. Solicita um painel centralizado para gerenciar as permissões dos usuários, como vendedores, estoque e gerência, além de recursos para acompanhar a operação do sistema. Busca a implantação de um sistema automatizado para substituir as conferências manuais.*

## 4. Entrevistas

### 4.1 Entrevista com a Dona do Sistema
### Perguntas

**1. Quais são as principais necessidades da loja em relação ao controle de estoque?**
**2. Quais problemas no controle de estoque mais preocupam você como dona da loja?**
**3. Quais informações sobre os produtos e o estoque você considera importantes para acompanhar o funcionamento da loja?**
**4. Que informações você gostaria de conseguir consultar rapidamente para tomar decisões?**
**5. Quais tipos de movimentação de estoque você considera importante que sejam registrados?**
**6. Você considera importante saber quem realizou cada movimentação? Por quê?**
**7. Existe alguma informação ou registro que você considera importante manter para consultas futuras?**
**8. Quais erros no controle de estoque poderiam trazer maiores prejuízos para a loja?**
**9. O que você espera que o sistema melhore em relação à forma como o estoque é controlado atualmente?**
**10. O que faria você considerar que o sistema realmente atende às necessidades da loja?**

### Respostas

*1. Saber o que temos, o que está acabando e o que está parado; registrar entradas e saídas com segurança.
2. Perder vendas por falta de produto, comprar em excesso e não perceber desvios/furtos.
3. Quantidade disponível, valor total, produtos mais vendidos, baixa saída, datas de entrada/saída.
4. Saldo por produto, alertas de estoque mínimo, movimentações recentes, valor investido.
5. Entradas por compra, saídas por venda, devoluções, ajustes de inventário, perdas/avarias.
6. Sim, para responsabilizar e identificar erros/desvios.
7. Histórico de movimentações, relatórios mensais, registros de inventário.
8. Falta de produto, excesso de compras, erros de contagem, registros incorretos.
9. Mais agilidade, menos erros manuais, informações em tempo real, relatórios confiáveis.
10. Confiar nos números, reduzir perdas, decidir com base no sistema.*

### 4.2 Entrevista com o Usuário Final

**1. Quais atividades relacionadas ao estoque você realiza no dia a dia?**
**2. Como essas atividades são realizadas atualmente?**
**3. Quais são as principais dificuldades encontradas nesse processo?**
**4. Quais informações sobre um produto você precisa consultar durante o trabalho?**
**5. Em quais situações você precisa registrar uma entrada ou saída?**
**6. O que pode causar erros ou dificuldades durante esses registros?**
**7. O que você considera importante para que o sistema seja fácil de utilizar?**
**8. Que informações você gostaria de encontrar rapidamente?**
**9. Existe alguma tarefa relacionada ao estoque que você considera demorada atualmente?**
**10. O que você gostaria que o sistema facilitasse no seu trabalho?**

### Respostas

*1- Contagem de produtos e analise de avarias.
2- Manualmente com uma prancheta e um caderno.
3- Falhas de contagem e ineficiencia.
4- Nome, ID, Lote, entrada e saída de produtos.
5- Quando há recebimento de um lote novo e em todas as vendas.
6- Grande quantidade de produtos em estoque e só eu trabalhando.
7- Simplicidade pra contabilizar os produtos e uma boa interface.
8- O ID do produto, nome, lote e quantidade.
9- A contagem de produtos e a analise de avarias.
10- Eu gostaria que fosse mais automatizado, tipo a contagem e a identificação, que eu precisasse só escanear.*

### 4.3 Entrevista com o Stakeholder Externo
### Perguntas

**1. Quais informações relacionadas ao estoque você considera importante que a loja mantenha registradas?**
**2. Por que é importante manter esses registros?**
**3. Que informações deveriam constar em um registro de movimentação?**
**4. Existe alguma preocupação em relação à alteração ou exclusão desses registros?**
**5. É importante identificar quem realizou cada movimentação? Por quê?**
**6. Por quanto tempo essas informações deveriam ficar disponíveis?**
**7. O que pode comprometer a confiabilidade dos registros?**
**8. Em uma fiscalização ou auditoria, quais informações poderiam ser necessárias?**
**9. Que situações relacionadas ao controle de estoque poderiam gerar problemas para a loja?**
**10. Qual seria sua principal expectativa em relação ao sistema?**

### Respostas

*1. Registros de produtos, quantidades, entradas, saídas, datas, fornecedores, vendas e responsáveis.
2. Para garantir organização, transparência e facilitar a identificação de erros ou irregularidades.
3. Produto, quantidade, tipo de movimentação, data, horário, motivo e responsável.
4. Sim. Alterações ou exclusões devem ser controladas e manter um histórico.
5. Sim. Para garantir a rastreabilidade e identificar quem realizou cada operação.
6. Pelo período exigido pela legislação e necessário para fiscalização e auditoria.
7. Erros, movimentações não registradas, alterações indevidas, falhas no sistema e acessos não autorizados.
8. Entradas, saídas, estoque, compras, vendas, ajustes, datas, horários e responsáveis.
9. Divergências de estoque, falta de registros, perdas sem justificativa e alterações indevidas.
10. Um sistema confiável, organizado e seguro, com histórico e rastreabilidade das movimentações.*

### 4.4 Entrevista com o Gestor do Sistema
### Perguntas

**1. Quais informações você precisa acompanhar para gerenciar o estoque?**
**2. Quais atividades de estoque precisam ser acompanhadas pela gestão?**
**3. Quais problemas de estoque você gostaria de identificar rapidamente?**
**4. Que tipos de relatórios ou consultas seriam úteis para a gestão?**
**5. Quais movimentações deveriam ficar disponíveis para consulta posterior?**
**6. Você considera importante acompanhar quem realizou cada movimentação?**
**7. Existem diferentes tipos de usuários que deveriam ter diferentes responsabilidades no sistema?**
**8. Que informações você gostaria de visualizar para auxiliar na tomada de decisões?**
**9. Quais problemas o sistema deveria ajudar a evitar?****
**10. O que você considera essencial para que o sistema atenda às necessidades da gestão?**

### Respostas

*1. Para gerenciar o estoque, é importante acompanhar informações como código de barras, descrição, marca, modelo, categoria, número de série, quantidade atual, quantidade mínima, quantidade máxima e quantidade reservada. Também são importantes informações sobre custos, preço de venda, fornecedores e localização física dos produtos.
2. A gestão precisa acompanhar as entradas, saídas, ajustes, inventários, devoluções e a necessidade de reposição dos produtos.
3. É importante identificar rapidamente problemas como furtos ou perdas, obsolescência de produtos, divergências entre o estoque físico e o registrado e falhas na rastreabilidade.
4. Seriam úteis relatórios sobre a situação do estoque, movimentações por período, giro dos produtos, produtos críticos e necessidades de reposição. A curva ABC também pode ajudar no acompanhamento dos produtos.
5. As movimentações devem ficar registradas com informações como data, horário, tipo de movimentação, quantidade e responsável. Manter esse histórico é importante para consultas, auditorias, análise de períodos e identificação de problemas com produtos.
6. Sim. Identificar o responsável por cada movimentação é importante para manter o controle e facilitar possíveis auditorias.
7. Sim. O sistema pode ter diferentes níveis de acesso, como administrador ou proprietário, comprador, operador de estoque e vendedor. Algumas informações, como custos, margens, dados financeiros de fornecedores e faturamento, devem ter acesso restrito.
8. Para auxiliar nas decisões, seria importante visualizar informações sobre o saldo dos produtos, giro do estoque, produtos críticos, valor do estoque, movimentações recentes e necessidades de reposição.
9. O sistema deve ajudar a evitar perdas, falta de produtos, compras desnecessárias, erros de registro, divergências no inventário e problemas relacionados à rastreabilidade.
10. Para atender às necessidades da gestão, o sistema deve oferecer informações confiáveis sobre o estoque, facilitar o acompanhamento das movimentações, manter os dados atualizados e disponibilizar relatórios que auxiliem na tomada de decisões.*

## 5. Mini-workshop de Conflito

### 5.1 Conflito identificado

**Durante a discussão sobre o funcionamento do sistema, surgiu uma preocupação em relação ao acesso às informações do estoque. Foi discutido que nem todos os usuários precisam ter acesso às mesmas informações, principalmente dados como custos, margens, informações de fornecedores e faturamento.
Ao mesmo tempo, foi considerada importante a possibilidade de consultar os registros das movimentações para acompanhar o estoque e permitir conferências e auditorias.**

### 5.2 Mediação

**Para resolver o conflito, o grupo discutiu a possibilidade de separar os níveis de acesso de acordo com a função de cada usuário. Dessa forma, cada pessoa teria acesso às informações necessárias para realizar suas atividades, enquanto informações mais restritas ficariam disponíveis apenas para usuários autorizados.
Também foi considerada importante a manutenção do histórico das movimentações, registrando quem realizou cada operação, para facilitar o acompanhamento e a identificação de possíveis erros ou alterações.**

### 5.3 Decisão do grupo

**O grupo decidiu que o sistema deverá possuir diferentes níveis de acesso de acordo com a função de cada usuário. As informações mais restritas deverão ficar disponíveis apenas para os usuários autorizados, enquanto as movimentações realizadas deverão manter um histórico para garantir o acompanhamento e a rastreabilidade do estoque.**

## 6. Requisitos levantados

### 6.1 Requisitos Funcionais

**RF-01 — Cadastro de produtos:** O sistema deve permitir cadastrar produtos com informações como código, nome, lote, quantidade e demais informações necessárias para sua identificação.

**RF-02 — Registro de entradas:** O sistema deve permitir registrar a entrada de produtos no estoque, informando a quantidade e os dados relacionados à movimentação.

**RF-03 — Registro de saídas:** O sistema deve permitir registrar a saída de produtos do estoque, informando a quantidade e os dados relacionados à movimentação.

**RF-04 — Registro de perdas e ajustes:** O sistema deve permitir registrar perdas, avarias, devoluções e ajustes de inventário.

**RF-05 — Consulta do estoque:** O sistema deve permitir consultar a quantidade e as informações dos produtos disponíveis no estoque.

**RF-06 — Histórico de movimentações:** O sistema deve manter o histórico das movimentações realizadas, registrando informações como data, horário, tipo de movimentação e responsável.

### 6.2 Requisitos Não Funcionais

**RNF-01 — Usabilidade:** O sistema deve possuir uma interface simples e fácil de utilizar.

**RNF-02 — Usabilidade:** As informações dos produtos e do estoque devem ser encontradas de forma rápida durante as atividades de consulta.

**RNF-03 — Confiabilidade:** Os registros de entrada, saída, perdas e ajustes devem ser mantidos de forma consistente.

**RNF-04 — Segurança:** O acesso às informações do sistema deve respeitar as permissões definidas para cada usuário.

**RNF-05 — Segurança:** As movimentações realizadas devem identificar o usuário responsável pela operação.

**RNF-06 — Confiabilidade:** O histórico das movimentações deve permanecer disponível para consultas posteriores.

