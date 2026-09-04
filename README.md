


## 📄 Arquivo de Justificativa (docs/justificativa.md)



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



