# Instacart Customer Behavior and Purchase Analysis  
## Sprint 3 – Exploratory Data Analysis (EDA) Project

### Overview  
This project analyzes customer purchasing behavior from Instacart, a grocery delivery platform similar to Uber Eats or iFood.  
The goal is to clean, explore, and visualize the data to understand consumer patterns, order frequency, popular products, and reorder behavior.

The original dataset was released by Instacart in a 2017 Kaggle competition and later adapted for this project, including missing values and duplicates to practice preprocessing tasks.

All analyses and visualizations are developed in the file:  
`instacart_analysis.ipynb`

---

## Project Objectives

- Clean and preprocess raw data  
- Explore user purchasing habits  
- Generate visual insights on order frequency and behavior  
- Identify top purchased and reordered items  
- Create a report answering mandatory analytical questions  

---

## Dataset Description

The project uses 5 CSV files, each representing part of the Instacart ecosystem:

### 1. `instacart_orders.csv`  
Each row represents an order.  
Key columns:
- `order_id`
- `user_id`
- `order_number`
- `order_dow` (0 = Sunday)
- `order_hour_of_day` (0 to 23)
- `days_since_prior_order`

### 2. `products.csv`  
Products available on the platform.  
Columns:
- `product_id`
- `product_name`
- `aisle_id`
- `department_id`

### 3. `order_products.csv` (not uploaded due to file size)  
Items included in each order.  
Columns:
- `order_id`
- `product_id`
- `add_to_cart_order`
- `reordered`

### 4. `aisles.csv`
- `aisle_id`
- `aisle`

### 5. `departments.csv`
- `department_id`
- `department`

---

## Data Preprocessing

The following steps were applied:

### Data Types
- Converted IDs to integers  
- Adjusted numerical columns

### Missing Values
- Identified and handled null entries

### Duplicates
- Detected and removed duplicate rows  
- Documented reasoning for each decision

---

## Analyses Performed

### [A] Mandatory Analyses
- Validation of `order_hour_of_day` (0–23) and `order_dow` (0–6)  
- Chart: Orders by hour of day  
- Chart: Purchases by day of the week  
- Distribution of time until next order

### [B] Mandatory Analyses
- Comparison between Wednesday and Saturday (`order_dow`)  
  - Histograms on the same plot  
- Distribution of number of orders per customer  
- Top 20 most purchased products (ID + name)

### [C] (at least 2 completed)
- Distribution of number of items per order  
- Top 20 most recurring items in reordered purchases  
- Reorder proportion per product  
- Reorder proportion per customer  
- Top 20 items most frequently added first to the cart

---

## Key Insights (available in `instacart_analysis.ipynb`)

- Peak purchasing occurs in the evening and on weekends  
- A small set of products dominate recurring orders  
- Customers exhibit consistent reorder patterns  
- Popular products vary by department

---

## Tools and Technologies

- Language: Python  
- Libraries: pandas, numpy, matplotlib  
- Environment: Jupyter Notebook

---
#Versão em Português

# Análise de Comportamento e Compras dos clientes da Instacart  
## Sprint 3 – Projeto de Análise Exploratória de Dados (AED)

### Visão Geral  
Este projeto analisa o comportamento de compra dos clientes da **Instacart**, uma plataforma de entrega de supermercado similar ao iFood e Uber Eats.  
O objetivo é limpar, explorar e visualizar os dados para entender padrões de consumo, frequência de pedidos, produtos mais populares e repetições de compra.

Os dados foram originalmente disponibilizados pela Instacart em uma competição do Kaggle (2017) e adaptados para este estudo com inclusão de valores ausentes e duplicados para prática de pré-processamento.

Todo o projeto está desenvolvido no arquivo instacart_analysis.ipynb

---

## Objetivos do Projeto

- Realizar limpeza e pré-processamento dos dados  
- Explorar os hábitos de compra dos usuários  
- Gerar gráficos e insights sobre comportamento e frequência de pedidos  
- Identificar produtos mais comprados e repetidos  
- Criar um relatório com respostas às perguntas analíticas obrigatórias  

---

## Descrição dos Dados

O projeto utiliza 5 arquivos CSV, cada um com uma parte do ecossistema da Instacart:

### 1. `instacart_orders.csv` 
Cada linha representa um pedido.
**Colunas principais:**
- `order_id`
- `user_id`
- `order_number`
- `order_dow` (0 = domingo)
- `order_hour_of_day` (0 a 23)
- `days_since_prior_order`

### 2. `products.csv`
Produtos disponíveis na plataforma.  
Colunas:
- `product_id`
- `product_name`
- `aisle_id`
- `department_id`

### 3. `order_products.csv` -> não foi possível carregar no Github, arquivo muito grande!
Itens incluídos em cada pedido.  
Colunas:
- `order_id`
- `product_id`
- `add_to_cart_order`
- `reordered`

### 4. `aisles.csv`
- `aisle_id`
- `aisle`

### 5. `departments.csv`
- `department_id`
- `department`

---

## Pré-Processamento de Dados

As seguintes etapas foram realizadas:

### ✅ Tipos de dados
- Conversão de IDs para inteiros  
- Ajuste de colunas numéricas

### ✅ Valores ausentes
- Identificação e preenchimento de valores ausentes

### ✅ Duplicatas
- Detecção e remoção de registros duplicados  
- Justificativa para métodos utilizados

---

## 📊 Análises Realizadas

### ✅ [A] Análises Obrigatórias
- Verificação dos limites de `order_hour_of_day` (0–23) e `order_dow` (0–6)  
- Gráfico: pedidos por hora do dia  
- Gráfico: compras por dia da semana  
- Distribuição do tempo até o próximo pedido

### ✅ [B] Análises Obrigatórias
- Comparação entre quarta-feira e sábado (`order_dow`)  
  - Histogramas no mesmo gráfico  
- Distribuição do número de pedidos por cliente  
- Top 20 produtos mais comprados (ID + nome)

### ✅ [C] (mínimo 2 concluídas)
- Distribuição do número de itens por pedido  
- Top 20 itens mais recorrentes em pedidos repetidos  
- Proporção de “reordered” por produto  
- Proporção de pedidos repetidos por cliente  
- Top 20 itens adicionados primeiro ao carrinho

---

## Principais Insights presentes no arquivo instacart_analysis.ipynb
- Pico de compras à noite e aos fins de semana  
- Alguns produtos dominam os pedidos recorrentes  
- Clientes apresentam padrões consistentes de recompra  
- Itens populares variam por departamento

---

## Ferramentas e Tecnologias

- **Linguagem:** Python  
- **Bibliotecas:** pandas, numpy, matplotlib
- **Ambiente:** Jupyter Notebook

---
---
