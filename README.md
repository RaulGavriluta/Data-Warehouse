# 📊 Data Warehouse Project (Medallion Architecture)

## 📌 Overview
This project implements a **Data Warehouse** using **Microsoft SQL Server (SSMS)**, following the **Medallion Architecture** approach (Bronze, Silver, Gold layers).

It showcases how raw data is ingested, transformed, and refined into **high-quality, analytics-ready datasets**, along with **data quality validation**.

---

## 🏗️ Architecture

The project is structured into three layers:

### 🥉 Bronze Layer (Raw Data)
- Stores raw, unprocessed data from source systems
- Acts as a historical and audit layer

---

### 🥈 Silver Layer (Cleaned Data)
- Cleans and standardizes data
- Handles:
  - Missing values  
  - Duplicates  
  - Data inconsistencies  

---

### 🥇 Gold Layer (Business-Ready Data)
- Contains curated datasets for reporting and analytics
- Structured using **fact and dimension tables**
- Optimized for BI tools

---

## ⚙️ Features
- ETL pipelines implemented in SQL  
- Layered transformations (Bronze → Silver → Gold)  
- Data quality validation scripts  
- Dimensional modeling (Fact & Dimension tables)  
- Modular and reusable SQL scripts  

---

## 🛠️ Tech Stack
- **Database:** Microsoft SQL Server  
- **Tool:** SQL Server Management Studio (SSMS)  
- **Language:** SQL  

---

## 📂 Project Structure
```
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── data_architecture.png           # Data architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.png                   # PNG file for the data flow diagram
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
└── README.md  
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/RaulGavriluta/Data-Warehouse.git
cd Data-Warehouse
```
### 2. Open in SSMS
- Connect to your SQL Server instance
- Open the project scripts

### 3. Run scrips in order

Step 1: Bronze Layer
- Run **ddl_bronze.sql**
- Execute **proc_load_bronze.sql**

Step 2: Silver Layer
- Run **ddl_silver.sql**
- Execute **proc_load_silver.sql**
- Validate using **quality_checks_silver.sql**

Step 3: Gold Layer
- Run **ddl_gold.sql**
- Validate using **quality_checks_gold.sql**

---

## 📊 Data Quality

The project includes data quality checks to ensure:

- Data completeness

- Consistency between layers

- No duplicates or invalid records

---

## 📈 Key Concepts Demonstrated

- Medallion Architecture (Bronze / Silver / Gold)

- ETL Pipelines using SQL

- Data Cleaning & Transformation

- Data Quality Validation

- Dimensional Modeling


