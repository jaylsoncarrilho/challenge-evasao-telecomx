# 📊 Análise de Evasão de Clientes (Churn) — Telecom X

Este projeto tem como objetivo entender os padrões de comportamento dos clientes da **Telecom X**, identificar fatores que influenciam a evasão (churn) e propor estratégias para reduzir a perda de clientes com base em análise exploratória de dados (EDA).

---

## 🧪 Tecnologias Utilizadas

- **Python 3.10+**
- **Pandas**
- **NumPy**
- **Matplotlib & Seaborn**
- **Google Colab**
- Fonte de dados: JSON via API hospedada no GitHub

---

## 📌 Objetivo

Analisar os dados de clientes da Telecom X para responder às perguntas:

- Quem são os clientes com maior risco de churn?
- Quais características estão mais associadas à evasão?
- Como os serviços, formas de pagamento e contratos impactam o comportamento do cliente?
- Quais ações a empresa pode tomar para reter esses clientes?

---

## ⚙️ Etapas Realizadas

### 1. Importação dos Dados  
- Leitura de dados JSON via `requests.get().json()`  
- Transformação da estrutura aninhada com `pd.json_normalize()`  

### 2. Limpeza e Pré-Processamento  
- Conversão de colunas para tipos corretos (ex: `TotalCharges`)  
- Verificação de valores ausentes e duplicados  
- Criação da variável `Contas_Diarias` (valor médio diário pago por cliente)

### 3. Análise Exploratória  
- Gráficos de distribuição de churn  
- Análise por variáveis categóricas (`Contract`, `PaymentMethod`, `InternetService`)  
- Comparação de variáveis numéricas (`tenure`, `TotalCharges`) entre clientes fiéis e evadidos

### 4. Conclusões e Recomendações  
- Padrões que indicam alto risco de churn  
- Ações estratégicas de retenção  
- Propostas para modelagem preditiva futura

---

## 🔍 Principais Insights

- Clientes com **contratos mensais** e **pagamento manual** (como boleto eletrônico) apresentaram maior taxa de churn.  
- Aqueles com **maior tempo de contrato** e **pagamento automático** tendem a permanecer.  
- Serviços adicionais (streaming, segurança online) correlacionam com maior fidelidade.

---

## 💡 Recomendações

- Incentivar contratos mais longos com benefícios associados  
- Estimular pagamento automático com recompensas ou descontos  
- Monitorar clientes com pouco tempo e baixo gasto para ações preventivas  
- Criar bundles de serviços que aumentem o engajamento

---

*(suporte na realização das Análises e criação do ReadMe atráves da IA Copilot)*
