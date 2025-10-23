# 🍹 Bevio & Co. – Dashboard de Vendas em Power BI

Projeto fictício de Business Intelligence desenvolvido para analisar o desempenho de vendas da **Bevio & Co.**, uma empresa do setor de bebidas que fornece produtos como cervejas, bebidas não alcoólicas e refrigerantes para bares, restaurantes e lojas.

O objetivo é simular um ambiente real de **análise de desempenho comercial**, com foco em modelagem de dados, medidas DAX e visualizações interativas no Power BI.

---

## 📦 Base de Dados

A base de dados é **fictícia** e representa as principais entidades do negócio da Bevio & Co.:

- **Orders (Pedidos):** `order_id`, `order_date`, `user_id`, `item_id`, `quantity`, `revenue`  
- **Targets (Metas):** metas mensais e anuais por produto e região  
- **Users (Clientes):** informações dos estabelecimentos (bar, restaurante, loja, distribuidor)  
- **Items (Produtos):** catálogo com `item_id`, `nome`, `categoria`, `preço`

Os dados foram modelados e integrados no **Power BI Desktop**, com colunas calculadas e medidas DAX para análise de receita, metas e desempenho.

---

## 📊 Página 1 – Painel Executivo

### 🧭 Visão Geral
O **Painel Executivo** resume os principais indicadores de desempenho da empresa em uma única página, permitindo uma visão rápida e estratégica.

**Principais KPIs:**
- **Revenue Total**
- **Revenue Target**
- **Target Achievement (% de atingimento da meta)**
- **Orders (quantidade de pedidos)**

**Visualizações:**
- Tendência Anual de Receita (linha + previsão)  
- Revenue por Tipo de Produto (barras)  
- Indicador de desempenho mensal (vermelho quando abaixo da meta)  
- Produto mais vendido (Beer)  
- Tabela com `item_id`, `categoria`, `quantidade` e `revenue`

**Principais insights:**
- 🍺 *Beer* é o produto mais vendido e de maior receita: **US$ 4,2M**  
- *NAB* é o segundo, com **US$ 1M**, mostrando grande diferença entre categorias  
- Receita mensal abaixo da meta → necessidade de ações comerciais  
- Projeção de leve desaceleração nas próximas semanas

---

## 🍾 Página 2 – Product Detail

### 🎯 Objetivo
Apresentar o desempenho detalhado por produto, comparando resultados com metas e permitindo seleção dinâmica de itens.

**Visualizações:**
- Indicador de atingimento da meta (customizável por produto)  
- Gráfico de tendência de receita por produto  
- Dois gráficos de pizza:  
  - Quantidade vendida por tipo de produto  
  - Pedidos por tipo de produto  
- Tabela com maiores receitas (top 4 produtos)

**Insights:**
- *Beer* domina em volume e receita  
- *NAB* e refrigerantes mantêm desempenho estável  
- Receita concentrada em poucos SKUs

---

## 🧑‍💼 Página 3 – User Detail

### 🎯 Objetivo
Analisar o perfil e o desempenho dos clientes, identificando principais compradores e regiões de maior relevância.

**Visualizações:**
- Receita média por usuário  
- Total de usuários  
- Top user por receita  
- Gráficos de pizza:  
  - Pedidos por categoria de cliente (bar, restaurante, loja)  
  - Pedidos por cidade  
- Tabela detalhada com `user_id`, `categoria`, `cidade` e `revenue`  

**Insights:**
- Bares e restaurantes concentram a maior parte das vendas  
- Rio de Janeiro é a cidade com mais pedidos  
- O cliente com maior faturamento é um **bar em Campinas**

---

## 🧠 Ferramentas e Técnicas

- **Power BI Desktop** → dashboards, medidas DAX, KPIs  
- **Excel / CSV** → base de dados e tratamento inicial  
- **Modelagem de Dados** → relacionamentos entre `orders`, `users`, `items` e `targets`  
- **Visualização** → tendências, previsões e segmentações dinâmicas  

---
