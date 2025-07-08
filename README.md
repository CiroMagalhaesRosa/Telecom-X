# 📊 Análise de Evasão de Clientes (Churn)

Este projeto tem como objetivo analisar os principais fatores que levam à evasão de clientes (churn) em uma empresa de serviços de telecomunicações. Através de uma abordagem de **Análise Exploratória de Dados (EDA)**, tratamos os dados, investigamos padrões e extraímos insights valiosos que podem apoiar estratégias de retenção.

## 🧠 Objetivo

Identificar perfis e comportamentos de clientes com maior propensão ao cancelamento, fornecendo recomendações estratégicas com base nos dados analisados.

## 🗂️ Estrutura do Projeto

- `TelecomX_Data.json`: arquivo original de dados.
- `notebook.ipynb`: notebook com todas as etapas da análise.
- `README.md`: este arquivo com a descrição do projeto.

## ⚙️ Etapas da Análise

### 1. Importação e Entendimento dos Dados
- Base JSON carregada direto do GitHub.
- Visualização geral e compreensão das variáveis.

### 2. Limpeza e Tratamento
- Remoção de valores nulos em `Churn` (linhas com 224 valores ausentes).
- Substituição dos nulos em `TotalCharges` por `MonthlyCharges` (clientes com menos de 1 mês de contrato).
- Conversão de variáveis categóricas em binárias.
- Renomeação da coluna `tenure` para `ContractDuration`.

### 3. Análise Exploratória (EDA)
- Visualização da taxa geral de churn (~26%).
- Análise por variáveis categóricas (contrato, serviços extras, método de pagamento).
- Análise por variáveis numéricas (tempo de contrato, valor mensal, valor total, contas diárias).
- Identificação de padrões e grupos de risco.

### 4. Principais Insights
- Contratos do tipo "Month-to-month" têm alto churn.
- Serviços como segurança e suporte reduzem churn.
- Clientes com `MonthlyCharges` altos e `ContractDuration` baixos têm maior chance de cancelamento.
- Método de pagamento "Electronic check" está associado a maior evasão.

### 5. Recomendações
- Estímulo a contratos de longo prazo.
- Ofertas de pacotes com serviços adicionais (segurança, suporte, backup).
- Monitoramento de clientes com gastos altos e baixa fidelidade.
- Melhor experiência nos métodos de pagamento manuais.

## 🧰 Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## 📎 Como Rodar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
