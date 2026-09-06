Sistema de Controle de Estoque
Informações do projeto

Projeto: Sistema de Controle de Estoque para uma loja de eletrônicos de médio porte
Disciplina: Engenharia de Software 1
Professor: Kaio Jonathas

Equipe
Adna Cecilia
Augusto Saul
Mário Melo
Fernando de Carvalho
Nathiara Santos



1. Justificativa do sistema

O grupo escolheu desenvolver um Sistema de Controle de Estoque para uma loja de eletrônicos de médio porte.

O sistema se aproxima da ideia de um “prédio”, apresentada em sala, pois possui diferentes responsabilidades e precisa ser organizado para permitir manutenção e evolução.

A loja trabalha com produtos de alto valor e que podem sofrer rápida obsolescência. Por isso, é importante manter um controle adequado das entradas, saídas e quantidades disponíveis em estoque.

Tamanho e complexidade

O sistema teria uma complexidade média, pois envolveria diferentes funcionalidades e responsabilidades relacionadas ao controle de estoque de uma loja de eletrônicos.

Quantas pessoas utilizariam o sistema?

O sistema poderia atender aproximadamente 10 a 27 usuários simultaneamente, considerando diferentes funções dentro da loja, como:

Operadores de caixa: registro de vendas e movimentações;
Estoquistas: controle de entradas e saídas de produtos;
Compradores: acompanhamento e reposição de estoque;
Gerentes: acompanhamento das informações do estoque;
Administradores: gerenciamento do sistema e dos usuários.
Quantas pessoas trabalhariam no sistema ao longo do tempo?

O desenvolvimento inicial seria realizado pelos 5 integrantes do grupo. Ao longo do tempo, o sistema poderia receber manutenção e evolução por uma equipe responsável por corrigir problemas e adicionar novas funcionalidades conforme as necessidades da loja.

Riscos de um desenvolvimento sem planejamento

Se o sistema fosse desenvolvido de forma artesanal, poderiam ocorrer problemas como:

inconsistência nas quantidades de produtos;
erros no registro de entradas e saídas;
dificuldade para corrigir ou alterar funcionalidades;
perda de informações;
problemas de acesso às funções do sistema.

Por isso, o planejamento e a aplicação de boas práticas são importantes para o desenvolvimento do sistema.

2. Princípios de Engenharia de Software

Modularidade e abstração

Para organizar o sistema de controle de estoque, podemos dividi-lo em módulos, cada um com uma responsabilidade específica. Os principais módulos seriam:

Produtos: cadastro e consulta dos produtos, categorias, preços e quantidades.
Estoque: controle das entradas e saídas e atualização das quantidades disponíveis.
Fornecedores: cadastro e consulta das informações dos fornecedores.
Vendas: registro das vendas e comunicação com o estoque para atualizar as quantidades.
Usuários: controle de acesso ao sistema e das funções de cada usuário.

A modularidade permite separar as responsabilidades do sistema, facilitando a manutenção e evitando que uma alteração em uma parte afete desnecessariamente as outras.

A abstração permite esconder os detalhes internos de cada módulo e disponibilizar apenas as operações necessárias. Por exemplo, o módulo de vendas pode solicitar a baixa de um produto no estoque sem precisar conhecer como o controle interno dessa quantidade é realizado.

Qualidade de software

Entre os atributos de qualidade de software estudados, os mais importantes para esse sistema são funcionalidade, confiabilidade e usabilidade.

Funcionalidade: o sistema deve realizar corretamente as tarefas para as quais foi desenvolvido, como cadastrar produtos e controlar entradas e saídas.
Confiabilidade: o sistema deve funcionar de forma estável, evitando falhas e inconsistências nas informações do estoque.
Usabilidade: o sistema deve ser fácil de entender e utilizar pelos funcionários.

Os demais atributos também são importantes. A eficiência contribui para um bom desempenho, a manutenibilidade facilita correções e melhorias futuras, e a portabilidade permite que o sistema seja utilizado em diferentes ambientes.

Manutenibilidade e evolução

A manutenção mais provável nos primeiros anos será a manutenção evolutiva, pois novas necessidades podem surgir conforme a loja utiliza o sistema.

Por exemplo, inicialmente o sistema pode controlar apenas o cadastro de produtos e as entradas e saídas. Após algum tempo de uso, a loja pode identificar a necessidade de receber um alerta quando determinado produto estiver abaixo de uma quantidade mínima definida.

Dessa forma, o sistema deve ser desenvolvido de maneira que novas funcionalidades possam ser adicionadas sem causar alterações desnecessárias nas demais partes.

Boas práticas gerais

Algumas boas práticas serão utilizadas durante o desenvolvimento:

Documentação: registrar decisões importantes e informações necessárias para compreender o projeto.
Versionamento: utilizar o Git para registrar as alterações, permitindo acompanhar o desenvolvimento e trabalhar de forma organizada entre os integrantes.
Padronização: manter padrões de nomes, formatação e organização dos arquivos para facilitar a compreensão e a manutenção do projeto.