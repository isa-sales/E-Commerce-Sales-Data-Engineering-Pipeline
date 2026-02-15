# E-Commerce-Sales-Data-Engineering-Pipeline
# 🛒 E-Commerce Sales Data Engineering Pipeline

Pipeline completo de Engenharia de Dados para processamento e análise de dados de vendas de e-commerce, utilizando Apache Airflow, Docker, PostgreSQL e Power BI.

---

##  Objetivo

Construir um pipeline de dados moderno que:

- Extraia dados de vendas
- Realize transformações e limpeza
- Carregue os dados em um banco relacional
- Orquestre o fluxo com Apache Airflow
- Disponibilize dados estruturados para análise e visualização

Este projeto simula um ambiente real de Engenharia de Dados.

---

##  Arquitetura

![Arquitetura do Projeto](ecommerce_pipeline_architecture.png)

---

##  Fluxo do Pipeline (ETL)

###  Extração (Extract)
- Leitura do dataset de pedidos de vendas (Sales Order Dataset - Kaggle)
- Ingestão via script Python

### Transformação (Transform)
- Limpeza de dados
- Tratamento de valores nulos
- Conversão de tipos (datas, valores monetários)
- Padronização de colunas
- Criação de métricas:
  - Receita Total
  - Ticket Médio
  - Receita por Região
  - Receita por Categoria

###  Carga (Load)
- Inserção dos dados tratados no PostgreSQL
- Estruturação em modelo analítico

###  Orquestração
- Pipeline automatizado com Apache Airflow
- DAG com tarefas separadas (extract → transform → load)
- Execução agendada

###  Visualização
- Dashboard desenvolvido no Power BI
- Análise de KPIs de vendas

---

## 🛠️ Tecnologias Utilizadas

- Python
- Apache Airflow
- Docker
- PostgreSQL
- Pandas
- Power BI

---

## 📂 Estrutura do Projeto
