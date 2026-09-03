# 🏪 Sistema de Controle de Estoque

[![Status do Projeto](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)](https://github.com/seu-usuario/sistema-estoque)
[![Versão](https://img.shields.io/badge/versão-0.1.0-blue)](https://github.com/seu-usuario/sistema-estoque)
[![Licença](https://img.shields.io/badge/licença-MIT-green)](https://opensource.org/licenses/MIT)
[![Equipe](https://img.shields.io/badge/equipe-5%20colaboradores-purple)](https://github.com/seu-usuario/sistema-estoque)

## 📋 Sobre o Projeto

Sistema de controle de estoque desenvolvido para gerenciar produtos, fornecedores, movimentações e vendas de uma loja de médio porte. O projeto segue uma abordagem profissional, tratando-se de um sistema de **porte médio-alto** (analogia "prédio comercial"), que exige planejamento arquitetural, equipe multidisciplinar e processos bem definidos.

### 🎯 Objetivos

- Gerenciar cadastro de produtos, fornecedores e clientes
- Controlar entradas e saídas de estoque em tempo real
- Gerar relatórios gerenciais (curva ABC, giro de estoque, margem de lucro)
- Integrar com sistemas de pagamento e nota fiscal eletrônica (NF-e)
- Garantir rastreabilidade de lotes e validade de produtos
- Oferecer interface intuitiva para operadores de caixa e gestores

---

## 🏗️ Arquitetura e Dimensionamento

Baseado na lógica **"casinha x prédio"**, este sistema é classificado como:

| Aspecto | Característica |
|---------|---------------|
| **Porte** | Prédio comercial de médio porte |
| **Complexidade** | Média a alta |
| **Módulos** | Produtos, Fornecedores, Clientes, Movimentações, Relatórios, Usuários |
| **Usuários estimados** | 10-50 simultâneos |
| **Equipe inicial** | 5 desenvolvedores + Analista de Negócios |
| **Manutenção** | 2-3 pessoas ao longo do tempo |

### 📊 Diagrama de Módulos

┌─────────────────────────────────────────────────────┐
│ SISTEMA DE CONTROLE DE ESTOQUE │
├─────────────┬─────────────┬─────────────────────────┤
│ Módulo │ Módulo │ Módulo │
│ Produtos │ Fornecedor │ Clientes │
├─────────────┼─────────────┼─────────────────────────┤
│ Módulo │ Módulo │ Módulo │
│ Estoque │ Vendas │ Relatórios │
├─────────────┼─────────────┼─────────────────────────┤
│ Módulo │ Módulo │ Módulo │
│ Usuários │ NF-e │ Integrações │
└─────────────┴───────────


---

## 🚀 Tecnologias Utilizadas

### Backend
- **Linguagem:** Python / Java / Node.js *(definir conforme equipe)*
- **Framework:** Django / Spring Boot / Express *(definir)*
- **Banco de Dados:** PostgreSQL / MySQL
- **Cache:** Redis
- **Filas:** RabbitMQ / Apache Kafka

### Frontend
- **Framework:** React / Angular / Vue.js
- **Estilização:** Tailwind CSS / Material-UI
- **Gerenciamento de Estado:** Redux / Context API

### Infraestrutura
- **Containers:** Docker
- **Orquestração:** Docker Compose / Kubernetes
- **CI/CD:** GitHub Actions / GitLab CI
- **Monitoramento:** Prometheus + Grafana
- **Logs:** ELK Stack (Elasticsearch, Logstash, Kibana)

### Ferramentas
- **Controle de Versão:** Git + GitHub
- **Gerenciamento de Projeto:** GitHub Projects / Jira / Trello
- **Documentação:** Swagger / Postman
- **Testes:** Jest / Pytest / JUnit

---

## 📁 Estrutura do Projeto
sistema-estoque/
├── .github/
│ └── workflows/ # CI/CD pipelines
├── docs/
│ ├── justificativa.md # Documento de justificativa do projeto
│ ├── requisitos.md # Levantamento de requisitos
│ └── arquitetura.md # Documentação arquitetural
├── backend/
│ ├── src/
│ │ ├── controllers/ # Controladores da API
│ │ ├── models/ # Modelos de dados
│ │ ├── services/ # Regras de negócio
│ │ ├── repositories/ # Camada de acesso a dados
│ │ ├── middleware/ # Middlewares (autenticação, etc)
│ │ └── utils/ # Utilitários
│ ├── tests/
│ ├── Dockerfile
│ └── requirements.txt
├── frontend/
│ ├── src/
│ │ ├── components/ # Componentes reutilizáveis
│ │ ├── pages/ # Páginas da aplicação
│ │ ├── services/ # Consumo da API
│ │ ├── store/ # Gerenciamento de estado
│ │ └── styles/ # Estilos globais
│ ├── public/
│ ├── Dockerfile
│ └── package.json
├── database/
│ ├── migrations/ # Migrations do banco
│ └── seeds/ # Dados iniciais
├── docker-compose.yml
├── .gitignore
├── LICENSE
└── README.md




---

## 🛠️ Como Executar o Projeto

### Pré-requisitos

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/)
- [Node.js](https://nodejs.org/) (versão 18+)
- [Python](https://www.python.org/) (versão 3.10+) ou Java 17+ *(dependendo da stack)*

### Passo a Passo

#### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/sistema-estoque.git
cd sistema-estoque


cp .env.example .env
# Edite o arquivo .env com suas configurações


docker-compose up -d


4. Acesse a aplicação
Frontend: http://localhost:3000

Backend API: http://localhost:8080/api

Documentação API: http://localhost:8080/api/docs

Banco de Dados: http://localhost:5432 (se exposto)


# Backend
cd backend
pytest

# Frontend
cd frontend
npm test



📝 Funcionalidades Principais
✅ Módulo Produtos
□ Cadastro, edição e exclusão de produtos
□ Controle de categorias e subcategorias
□ Gerenciamento de fornecedores
□ Controle de lotes e validade
□ Histórico de preços
✅ Módulo Estoque
□ Entrada e saída de produtos
□ Controle de estoque mínimo e ponto de reposição
□ Transferência entre depósitos
□ Inventário físico
□ Ajustes de estoque
✅ Módulo Vendas
□ Registro de vendas
□ Cálculo automático de impostos
□ Integração com PDV (Ponto de Venda)
□ Emissão de cupom fiscal
□ Devoluções e cancelamentos
✅ Módulo Relatórios
□ Curva ABC de produtos
□ Giro de estoque
□ Margem de lucro
□ Produtos mais vendidos
□ Previsão de demanda
✅ Módulo Usuários
□ Controle de acesso (RBAC - Role Based Access Control)
□ Perfis: Administrador, Gerente, Comprador, Caixa, Estoquista
□ Autenticação JWT
□ Log de atividades
🧪 Testes e Qualidade
Cobertura de Testes
□ Testes unitários (back-end e front-end)
□ Testes de integração
□ Testes de carga e performance
□ Testes end-to-end (E2E)


Ferramentas
bash
# Backend
pytest --cov=src tests/          # Cobertura de código
pytest --benchmark tests/        # Performance

# Frontend
npm run test:coverage            # Cobertura
npm run test:e2e                 # Testes E2E com Cypress


🤝 Como Contribuir
Fork o projeto

Crie uma branch para sua feature (git checkout -b feature/nova-funcionalidade)

Commit suas mudanças (git commit -m 'feat: adiciona nova funcionalidade')

Push para a branch (git push origin feature/nova-funcionalidade)

Abra um Pull Request

Padrão de Commits
Usamos Conventional Commits:

bash
feat: nova funcionalidade
fix: correção de bug
docs: documentação
style: formatação
refactor: refatoração
test: testes
chore: tarefas administrativas
📅 Roadmap
Fase 1 - Planejamento (Sprint 1-2)
☑ Levantamento de requisitos
☑ Documentação de justificativa
☑ Definição da arquitetura
□ Configuração do ambiente
Fase 2 - MVP (Sprint 3-6)
□ CRUD de produtos e fornecedores
□ Controle básico de estoque
□ Autenticação e perfis de usuário
□ Relatórios básicos
Fase 3 - Escalabilidade (Sprint 7-10)
□ Integração com NF-e
□ Módulo de vendas e PDV
□ Relatórios gerenciais avançados
□ Otimização de performance
Fase 4 - Evolução (Sprint 11+)
□ Integração com e-commerce
□ Aplicativo mobile
□ Machine Learning para previsão de demanda
□ Multi-loja / Multi-tenant
🐛 Problemas Conhecidos
Veja a seção de Issues para problemas em aberto.

📚 Documentação Adicional
Justificativa do Projeto - Por que este sistema é um "prédio" e não uma "casinha"

Requisitos Funcionais - Detalhamento de todas as funcionalidades

Arquitetura Técnica - Decisões arquiteturais e tecnologias

Guia de Desenvolvimento - Como configurar o ambiente de dev

API Reference - Documentação completa da API (Swagger)

👥 Equipe
Nome	Papel	GitHub	Responsabilidades
Adna Cecilia	Desenvolvedora Full Stack	@adnacecilia	Frontend + Integrações
Mário Melo	Desenvolvedor Backend	@mariomelo	API + Regras de negócio
Nando	Desenvolvedor Full Stack	@nando	Backend + Banco de Dados
Nathiara Santos	Desenvolvedora Frontend	@nathiarasantos	UI/UX + Componentes React
Saul	Analista de Negócios / QA	@saul	Requisitos + Testes + Documentação


## 📄 Arquivo de Justificativa (docs/justificativa.md)

Agora vou criar o arquivo específico com a justificativa que você pediu, já personalizado para a equipe:

```markdown
# 📋 Justificativa do Sistema de Controle de Estoque

**Projeto:** Sistema de Controle de Estoque para Loja de Médio Porte  
**Equipe:** Adna Cecilia, Mário Melo, Nando, Nathiara Santos, Saul  
**Disciplina:** Conceitos e Contextualização  
**Data:** Setembro/2026

---

## 🎯 Contexto e Objetivo

Este documento tem como objetivo justificar a abordagem escolhida para o desenvolvimento do sistema de controle de estoque, utilizando a analogia **"casinha x prédio"** estudada em sala de aula. A justificativa serve como base para o planejamento do projeto e para alinhar a equipe sobre a complexidade e os desafios envolvidos.

---

## 🏠 "Casinha" x 🏢 "Prédio": Onde nosso sistema se encaixa?

### Analogia aplicada

| Característica | Casinha | Prédio (NOSSO SISTEMA) |
|----------------|---------|------------------------|
| **Tamanho** | Pequeno, poucos cômodos | Grande, múltiplos andares e setores |
| **Complexidade** | Baixa, estrutura simples | Média-alta, com muitas interconexões |
| **Planejamento** | Rápido, improvisado | Detalhado, com plantas e engenheiros |
| **Manutenção** | Feita por 1 pessoa | Exige equipe especializada |
| **Evolução** | Difícil de expandir | Projetado para crescer |
| **Usuários** | 1-2 pessoas | 10-50 pessoas simultâneas |

---

## 1️⃣ Que tamanho e complexidade esse sistema provavelmente teria?

O sistema de controle de estoque se enquadra como um **prédio comercial de médio porte** pelos seguintes motivos:

### 📊 Dimensionamento Técnico

- **Módulos envolvidos:**
  - Produtos e Categorias
  - Fornecedores
  - Clientes
  - Movimentações de Estoque (entrada/saída)
  - Vendas e PDV
  - Relatórios Gerenciais
  - Usuários e Permissões
  - Nota Fiscal Eletrônica (NF-e)
  - Integrações externas

- **Regras de negócio complexas:**
  - Cálculo de estoque mínimo e ponto de reposição
  - Controle de lotes e datas de validade
  - Curva ABC de produtos
  - Cálculo automático de impostos
  - Giro de estoque e margem de lucro

- **Integrações necessárias:**
  - Sistema de pagamento (TEF)
  - Impressoras fiscais
  - Nota Fiscal Eletrônica (NF-e)
  - Futuro e-commerce

### 📈 Estimativa de Complexidade
Complexidade: (Média-Alta: 7/10)
Tamanho de Código: ~50.000 - 100.000 linhas
Banco de Dados: 15-20 tabelas inter-relacionadas
Tempo de Desenvolvimento: 4-6 meses (MVP)

2️⃣ Quantas pessoas usariam, e quantas pessoas provavelmente trabalhariam nele ao longo do tempo?

### 👥 Usuários Finais

| Perfil | Quantidade | Função |
|--------|------------|--------|
| Operadores de Caixa | 5-15 | Registrar vendas, movimentações |
| Estoquistas | 2-5 | Controlar entradas/saídas físicas |
| Compradores | 1-2 | Gerenciar reposição de estoque |
| Gerentes | 1-3 | Acompanhar relatórios e metas |
| Administradores | 1-2 | Configurar sistema e permissões |
| **TOTAL** | **10-27 simultâneos** | |

### 👨‍💻 Equipe de Desenvolvimento



3️⃣ O que poderia dar errado se ele fosse construído de forma "artesanal", sem processo, sem planejamento?

### 🚨 Riscos e Impactos

| Risco | Consequência | Impacto |
|-------|--------------|---------|
| **Inconsistência de dados** | Produto baixado do estoque sem ser vendido ou vice-versa | Prejuízo financeiro e perda de credibilidade |
| **Erros fiscais** | Cálculo incorreto de impostos | Multas da Receita Federal e problemas legais |
| **Falta de rastreabilidade** | Não saber quais clientes compraram lote defeituoso | Risco à saúde, processos judiciais |
| **Código monolítico** | Mudança em um módulo quebra outro | Sistema para de funcionar do nada |
| **Segurança frágil** | Senhas expostas, permissões incorretas | Roubo de mercadorias virtuais |
| **Performance ruim** | Caixa espera 3 segundos para registrar item | Filas enormes, perda de vendas |
| **Sem backup** | Perda de dados em queda de energia | Recuperação impossível, loja para |


 4️⃣ Por que programar bem não seria suficiente para esse sistema específico?

Programar bem (código limpo, boas práticas, padrões de projeto) é **necessário mas NÃO SUFICIENTE**. Veja por quê:

### 🔍 Domínio de Negócio

> *"Um excelente programador pode criar um código perfeito que resolve o problema errado"*

**Exemplo:** O programador pode criar um sistema de estoque impecável tecnicamente, mas se não entender:
- Como funciona a **curva ABC** de produtos
- O que é **estoque de segurança**
- Como calcular **margem de lucro** considerando impostos

...o sistema será inútil para o gestor da loja.

### 🏗️ Arquitetura e Integrações

O sistema não existe isolado. Ele precisa se comunicar com:
┌──────────────┐ ┌──────────────┐
│ Sistema de │◄────►│ Impressora │
│ Estoque │ │ Fiscal │
└──────────────┘ └──────────────┘
│
▼
┌──────────────┐ ┌──────────────┐
│ TEF/Pagto │◄────►│ E-commerce │
└──────────────┘ └──────────────┘

 📊 Resumo: Por que isso é um "PRÉDIO"?

| Critério | Justificativa |
|----------|---------------|
| **Tamanho** | Múltiplos módulos, 50k+ linhas de código |
| **Complexidade** | Regras fiscais, integrações, performance crítica |
| **Equipe** | 5 pessoas no desenvolvimento, 3 na manutenção |
| **Usuários** | 10-50 simultâneos, perfis variados |
| **Riscos** | Financeiros, legais, operacionais graves |
| **Planejamento** | Essencial para evitar falhas catastróficas |

---

## ✅ Conclusão

O Sistema de Controle de Estoque **NÃO é uma "casinha"** que pode ser construída de forma artesanal por um único desenvolvedor em poucos dias.

É um **"PRÉDIO"** que exige:

1. **Planejamento arquitetural** (plantas)
2. **Equipe multidisciplinar** (engenheiros especializados)
3. **Processos definidos** (metodologia de construção)
4. **Testes rigorosos** (controle de qualidade)
5. **Documentação completa** (manual do prédio)

Programar bem é essencial, mas sem análise de negócio, arquitetura, UX, testes e gestão de projeto, o sistema será frágil, inseguro e insustentável a longo prazo.

