# NovaDrive-ELT-Airflow-Snowflake-dbt

### Pipeline de Dados e Camada Analítica

---

## ⚙️ Descrição do Projeto

Este projeto demonstra a construção de um pipeline de **ELT (Extract, Load, Transform)** para uma camada analítica de dados de vendas da empresa fictícia NovaDrive Motors. A solução é orquestrada pelo **Apache Airflow** e utiliza o **Snowflake** como Data Warehouse.

O objetivo principal é processar dados brutos a partir de um banco de dados **PostgreSQL** e transformá-los em um modelo analítico robusto e pronto para consumo, garantindo que as informações de negócio sejam consistentes e confiáveis.

---

## 🏛️ Arquitetura do Sistema

A arquitetura do pipeline é construída para ser escalável e eficiente, seguindo o padrão de um fluxo de dados moderno na nuvem.

### Fluxo de Trabalho

`PostgreSQL (Dados de Origem)` -> **`AWS`** -> **`Airflow`** -> `Snowflake (Data Warehouse)` -> **`dbt`** -> `Snowflake (Camada Analítica)`

### Componentes Chave

* **Extração e Carga:** Um DAG no Airflow é responsável por extrair dados de tabelas específicas do PostgreSQL e carregá-los diretamente no Snowflake.
* **Transformação e Modelagem:** O dbt é utilizado para transformar os dados brutos, criando uma camada analítica com modelos de fato e dimensão otimizados para consultas de BI e relatórios.

---

## 🛠️ Tecnologias

* **Orquestração:** Apache Airflow
* **Infraestrutura:** AWS EC2 (com Docker para o Airflow)
* **Data Warehouse:** Snowflake
* **Modelagem de Dados:** dbt
* **Linguagens:** Python e SQL

---
##  Link do LookerStudio
https://lookerstudio.google.com/reporting/aaf570ce-dee7-47a1-9082-6ae70c0b1f45
