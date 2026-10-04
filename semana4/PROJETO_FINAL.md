# Projeto Final

## Índice

1. [Identificação](#1-identificação)
2. [Visão Geral do Sistema](#2-visão-geral-do-sistema)
3. [Fundamentos do Sistema (Semana 1)](#3-fundamentos-do-sistema-semana-1)
4. [Requisitos e Viabilidade (Semana 2)](#4-requisitos-e-viabilidade-semana-2)
5. [Modelagem UML (Semana 3)](#5-modelagem-uml-semana-3)
6. [Modelo de Processo (Semana 4)](#6-modelo-de-processo-semana-4)
7. [Cenário de Mudança](#7-cenário-de-mudança)

---

## 1. Identificação

| Campo       | Preencher                                                                      |
| ----------- | ------------------------------------------------------------------------------ |
| Grupo       | Sistema de Controle de Estoque para uma loja de eletrônicos de médio porte     |
| Tema        | Sistema de Controle de Estoque                                                 |
| Integrantes | Nathiara Santos, Adna Cecilia, Augusto Saul, Fernando de Carvalho e Mário Melo |
| Disciplina  | Engenharia de Software I                                                       |

## 2. Visão Geral do Sistema

O sistema tem como objetivo auxiliar no controle de estoque de uma loja de eletrônicos de médio porte e de suas unidades franqueadas. Ele permite o cadastro e acompanhamento dos produtos, registro de entradas, saídas, perdas e ajustes, além da consulta do estoque e do histórico das movimentações. O sistema também considera diferentes níveis de acesso de acordo com o perfil do usuário e a unidade.

---

## 3. Fundamentos do Sistema (Semana 1)

O sistema exige o uso de Engenharia de Software porque envolve diferentes usuários, regras de acesso e várias informações que precisam ser organizadas e mantidas de forma consistente. A aplicação dos princípios e métodos de Engenharia de Software ajuda o grupo a dividir as responsabilidades, organizar os requisitos e facilitar futuras mudanças no sistema.

A modularidade permite separar as diferentes partes do sistema, enquanto a qualidade está relacionada ao funcionamento correto e à organização das informações. A manutenibilidade facilita a realização de alterações quando novas necessidades surgirem. As boas práticas ajudam a manter os artefatos organizados e facilitar o trabalho entre os integrantes.

🔗 [semana1/](semana1/)

## 4. Requisitos e Viabilidade (Semana 2)

Na Semana 2, o grupo realizou a elicitação dos requisitos utilizando atores e entrevistas, considerando diferentes pontos de vista dos envolvidos no sistema. Também foi analisado um conflito entre interesses dos participantes para chegar a uma definição que atendesse às necessidades do sistema.

A partir disso, foram consolidados seis requisitos funcionais e seis requisitos não-funcionais, relacionados principalmente ao cadastro e movimentação de produtos, consulta do estoque, histórico das operações, usabilidade, confiabilidade e segurança.

O estudo de viabilidade analisou os aspectos técnico, econômico e operacional. Ao final, o projeto foi considerado viável dentro do contexto proposto.

🔗 [semana2/requisitos.md](semana2/requisitos_reformulados.md) · [semana2/viabilidade.md](semana2/viabilidade.md)

## 5. Modelagem UML (Semana 3)

Na Semana 3 foram desenvolvidos os diagramas UML para representar diferentes aspectos do sistema. O diagrama de casos de uso apresenta as funcionalidades e a interação dos atores com o sistema. O diagrama de classes representa as principais entidades, seus atributos, operações e relacionamentos. Os diagramas de sequência representam o fluxo de execução das ações do sistema.

### Diagramas produzidos

* [Diagrama de casos de uso](semana3/diagrama_casos_uso.drawio)
* [Diagrama de classes](semana3/diagrama_classes_reformulado.drawio)
* [Diagrama de sequência — Cadastrar Produto](semana3/diagrama_sequência_cadastrar_produto.drawio)
* [Diagrama de sequência — Registrar Saída](semana3/sequencia_registrar_saida.drawio)
* [Diagrama de sequência — Consultar Histórico de Movimentação](semana3/Consultar_Histórico_Movimento.drawio)
* [Diagrama de sequência — Registrar Entrada de Produtos](semana3/Diagrama_Sequencia_Registrar_Produto.drawio)
* [Diagrama de sequência _ Consultar Estoque](semana3/diagrama_sequencia_consultar_estoque.drawio)

Os diagramas de sequência foram divididos entre os integrantes de acordo com as funcionalidades trabalhadas na Semana 2. Nathiara ficou responsável pelo diagrama de Cadastrar Produto e pelo diagrama de classes. Augusto Saul ficou responsável pelo diagrama relacionado ao registro de entrada de produtos. Adna Cecilia ficou responsável pelo registro de saída de produtos. Fernando de Carvalho ficou responsável pelo seu diagrama de sequência e pelos ajustes relacionados ao diagrama de casos de uso. Mário Melo ficou responsável pelo diagrama de sequência de consulta do histórico de movimentações.

## 6. Modelo de Processo (Semana 4)

O grupo escolheu utilizar o modelo Ágil, com o Kanban como framework. Essa escolha foi feita porque o projeto pode passar por mudanças durante o desenvolvimento, como aconteceu com a inclusão do cenário envolvendo o franqueado. O Kanban permite organizar as atividades e acompanhar o que precisa ser feito, o que está em andamento e o que já foi concluído.

O modelo em cascata foi descartado porque trabalha com etapas mais rígidas, tornando mais difícil realizar mudanças depois que uma etapa já foi concluída. O modelo incremental também poderia ser utilizado, mas o grupo considerou o Ágil mais adequado ao perfil da equipe e à possibilidade de ajustes durante o projeto.

Com o Kanban, uma mudança pode ser adicionada como uma nova atividade e analisada antes de alterar os artefatos que realmente serão afetados. Dessa forma, o grupo consegue adaptar o projeto sem precisar refazer todo o trabalho já realizado.

🔗 [semana4/](semana4/)

---

## 7. Cenário de Mudança

### O cenário recebido

O cenário de mudança acrescenta a participação de um franqueado ao sistema. O franqueado precisa consultar informações relacionadas ao estoque da matriz para evitar perdas de vendas e melhorar o atendimento aos clientes. Ao mesmo tempo, a matriz precisa manter o controle sobre suas informações internas, sem disponibilizar ao franqueado dados financeiros ou outras informações que não sejam necessárias para sua operação.

Também foi identificado o interesse do franqueado em solicitar produtos à matriz, enquanto a matriz precisa manter a aprovação e o controle dessas solicitações. Dessa forma, surge a necessidade de considerar diferentes níveis de acesso às informações de acordo com o perfil do usuário e a unidade.

### Tipo de manutenção

O cenário representa principalmente uma manutenção adaptativa, pois envolve a adaptação do sistema a uma nova situação de uso, com a inclusão do franqueado e a necessidade de considerar diferentes unidades.

A mudança não está relacionada à correção de um erro existente, portanto não caracteriza manutenção corretiva. Também não tem como objetivo principal apenas melhorar uma funcionalidade existente, mas adaptar o sistema a uma nova necessidade do contexto de utilização.

### Análise de impacto

A mudança afeta inicialmente os stakeholders, com a inclusão do franqueado como um novo participante do sistema. Isso também altera a análise das permissões, pois o franqueado precisa ter acesso às funcionalidades necessárias para administrar sua própria unidade, sem receber acesso irrestrito às informações da matriz.

Nos requisitos, os requisitos relacionados à segurança e ao controle por unidade passam a ter maior importância. O RNF-04, que estabelece o controle de acesso de acordo com o perfil e a unidade, e o RNF-05, que identifica o usuário e a unidade responsável pelas operações, dão suporte a essa nova necessidade. O RNF-06 também é relevante para manter a separação das informações entre a matriz e as unidades franqueadas.

A análise de viabilidade realizada na Semana 2 também foi considerada. A inclusão do franqueado pode gerar um aumento no esforço de desenvolvimento e manutenção, principalmente pela necessidade de controlar o acesso às informações de acordo com o perfil e a unidade. Mesmo assim, a mudança não torna o sistema inviável. A viabilidade técnica e operacional continua sendo possível com os ajustes necessários, e o possível aumento de custo não altera a conclusão de que o projeto é economicamente viável.

A modelagem UML também é afetada. No diagrama de casos de uso, o franqueado passa a ser considerado um ator com acesso às funcionalidades relacionadas à sua própria unidade. No diagrama de classes, foi acrescentada a classe `Unidade`, relacionada a `Produto`, `Usuário` e `Movimentação`, permitindo representar a relação entre os registros do sistema e cada unidade.

Apesar de o cenário mencionar solicitações de transferência entre unidades, essa funcionalidade não foi incorporada como um novo requisito funcional nesta versão do projeto, pois não fazia parte dos seis requisitos funcionais consolidados anteriormente. A possibilidade de criar funcionalidades de transferência pode ser considerada uma evolução futura do sistema caso seja formalmente incluída no escopo.

Os demais artefatos não precisam ser completamente refeitos. Os requisitos funcionais existentes continuam representando as principais funcionalidades do sistema, enquanto a mudança é tratada principalmente pela adaptação dos atores, das permissões e da estrutura de unidades. Dessa forma, o grupo consegue incorporar o novo cenário sem perder a relação entre os artefatos desenvolvidos ao longo das semanas anteriores.
