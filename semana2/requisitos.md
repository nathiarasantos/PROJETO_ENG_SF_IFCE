# Documento de Requisitos

## Índice

1. [Identificação](#1-identificação)

2. [O Sistema](#2-o-sistema)

3. [Requisitos Funcionais](#3-requisitos-funcionais)

4. [Requisitos Não-Funcionais](#4-requisitos-não-funcionais)

5. [Requisitos Relacionados](#5-requisitos-relacionados)

---

## 1. Identificação

| Campo | Preencher |
|---|---|
| Grupo | Sistema de Controle de Estoque para uma loja de eletrônicos de médio porte |
| Integrantes | Nathiara Santos, Adna Cecilia, Augusto Saul, Fernando de Carvalho e Mário Melo |
| Disciplina | Engenharia de Software I |
| Semana | 2 |
| Data | 19/09/2026 |

## 2. O Sistema

O sistema tem como objetivo auxiliar no controle de estoque de uma loja de eletrônicos de médio porte. Ele deve permitir o acompanhamento dos produtos, das entradas e saídas, das perdas e ajustes, além de manter informações das movimentações para facilitar o controle e a consulta do estoque.

---

## 3. Requisitos Funcionais

| ID | Descrição |
|---|---|
| RF-01 | O sistema deve permitir cadastrar produtos com informações necessárias para sua identificação. |
| RF-02 | O sistema deve permitir registrar a entrada de produtos no estoque. |
| RF-03 | O sistema deve permitir registrar a saída de produtos do estoque. |
| RF-04 | O sistema deve permitir registrar perdas, avarias, devoluções e ajustes de inventário. |
| RF-05 | O sistema deve permitir consultar a quantidade e as informações dos produtos disponíveis no estoque. |
| RF-06 | O sistema deve manter o histórico das movimentações realizadas, registrando a data, o horário, o tipo de movimentação e o responsável. |

## 4. Requisitos Não-Funcionais

| ID | Categoria | Descrição |
|---|---|---|
| RNF-01 | Usabilidade | O sistema deve possuir uma interface simples e fácil de utilizar. |
| RNF-02 | Usabilidade | As informações dos produtos e do estoque devem ser encontradas de forma rápida durante as consultas. |
| RNF-03 | Confiabilidade | Os registros de entrada, saída, perdas e ajustes devem ser mantidos de forma consistente. |
| RNF-04 | Segurança | O acesso às informações do sistema deve respeitar as permissões definidas para cada usuário. |
| RNF-05 | Segurança | As movimentações realizadas devem identificar o usuário responsável pela operação. |
| RNF-06 | Confiabilidade | O histórico das movimentações deve permanecer disponível para consultas posteriores. |

---

## 5. Requisitos Relacionados

| RF | RNF relacionado(s) |
|---|---|
| RF-01 | RNF-01, RNF-03, RNF-04 |
| RF-02 | RNF-03, RNF-05 |
| RF-03 | RNF-03, RNF-05 |
| RF-04 | RNF-03, RNF-05 |
| RF-05 | RNF-01, RNF-02, RNF-04 |
| RF-06 | RNF-03, RNF-04, RNF-05, RNF-06 |

---

### Checklist antes de entregar

- [x] Cada requisito é **verificável** (dá pra testar se foi atendido ou não)
- [x] Cada requisito é **não ambíguo** (só uma leitura possível)
- [x] Cada requisito é **atômico** (descreve uma coisa só)
- [x] Nenhum requisito descreve uma **solução de projeto** (tecnologia, banco de dados, biblioteca específica)
