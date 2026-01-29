# 📊 Dashboard de Performance de Vendas - Jan/Fev 2025

Este projeto demonstra o ciclo completo de análise de dados, desde a extração de dados brutos (Raw Data) via SQL até a criação de um dashboard estratégico no Power BI para suporte à tomada de decisão.
[Perfomance de Vendas](Perfo_Corri.png)
## 🚀 Visão Geral do Projeto
O objetivo foi transformar uma base de dados de vendas inconsistente em um painel de indicadores (KPIs) claro, permitindo monitorar o faturamento, comportamento de produtos e saúde financeira da operação.
[Banco de Dados](Print_SQL_Vendas.png)

[Banco de Dados Tratado](SQl_Vendas_Corri.png)
### 🛠️ Etapa 1: ETL e Tratamento com SQL
Os dados originais apresentavam diversos desafios comuns no mundo real. Utilizei **SQLite** para realizar a limpeza:
* **Correção de Outliers:** Identifiquei uma venda de 1000 unidades de "Smartphone X" que distorcia o faturamento total. O valor foi saneado para 1 unidade após análise de integridade.
* **Padronização:** Normalização de categorias (ex: 'eletronicos' e 'ELETRONICOS' para 'Eletrônicos').
* **Tratamento de Nulos:** Preenchimento de preços e quantidades nulas para garantir a precisão dos cálculos de Ticket Médio.
* **Formatos de Data:** Padronização para o formato ISO (AAAA-MM-DD).

### 📈 Etapa 2: Análise e Visualização (Power BI)
No dashboard, foquei em trazer os indicadores mais críticos para o negócio:
* **Faturamento Total:** R$ 14,2 Mil.
* **Ticket Médio:** R$ 1 Mil por pedido.
* **Status de Pedidos:** Monitoramento em tempo real de pedidos Concluídos (86%), Pendentes (6%) e Cancelados (2%).
* **Mix de Categoria:** Identificação de que a categoria **Eletrônicos** representa 76% do volume de vendas.
* **Tendência de Vendas:** Gráfico de linha mostrando a evolução diária e picos de demanda entre Janeiro e Fevereiro.

## 🧰 Tecnologias Utilizadas
* **Banco de Dados:** SQLite
* **Linguagem:** SQL (DML e DDL)
* **Visualização:** Power BI (DAX para medidas e Power Query para modelagem final)
* **Documentação:** Markdown

---
*Projeto desenvolvido para fins de estudo e portfólio de análise de dados.*
