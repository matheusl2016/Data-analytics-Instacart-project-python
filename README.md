# Análise de Comportamento e Compras dos clientes da Instacart  
## Sprint 3 – Projeto de Análise Exploratória de Dados (AED)

### Visão Geral  
Este projeto analisa o comportamento de compra dos clientes da **Instacart**, uma plataforma de entrega de supermercado similar ao iFood e Uber Eats.  
O objetivo é limpar, explorar e visualizar os dados para entender padrões de consumo, frequência de pedidos, produtos mais populares e repetições de compra.

Os dados foram originalmente disponibilizados pela Instacart em uma competição do Kaggle (2017) e adaptados para este estudo com inclusão de valores ausentes e duplicados para prática de pré-processamento.

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
- Identificação e preenchimento de valores faltantes

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

## Principais Insights (exemplo genérico)
- Pico de compras à noite e aos fins de semana  
- Alguns produtos dominam os pedidos recorrentes  
- Clientes apresentam padrões consistentes de recompra  
- Itens populares variam por departamento

*(Essa seção pode ser ajustada depois com base nos resultados do seu notebook.)*

---

## Ferramentas e Tecnologias

- **Linguagem:** Python  
- **Bibliotecas:** pandas, numpy, matplotlib
- **Ambiente:** Jupyter Notebook

---
