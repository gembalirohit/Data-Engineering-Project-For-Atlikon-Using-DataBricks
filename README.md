# 🚀 FMCG Data Engineering Project using Databricks

## 📌 Overview

This project demonstrates an **end-to-end data engineering pipeline** built using **Databricks (Free Edition)** for an FMCG use case.

It integrates data from **parent and child companies**, processes both **full load and incremental data**, and creates **analytics-ready datasets** using modern data engineering practices.

---

## 🏗️ Architecture

* Data Sources: Parent & Child Company datasets
* Processing: Databricks (PySpark)
* Storage: Delta Lake
* Modeling: Star Schema (Fact & Dimension Tables)
* Load Types: Full Load + Incremental Load

---

## 📂 Project Structure

```
project-de-fmcg-atlikon/
│
├── 0_data/
│   ├── 1_parent_company/
│   │   ├── full_load/
│   │   ├── incremental_load/
│   │
│   ├── 2_child_company/
│       ├── full_load/
│       │   ├── customers/
│       │   ├── gross_price/
│       │   ├── orders/
│
├── notebooks/ (Databricks notebooks - if present)
├── scripts/
└── README.md
```

---

## ⚙️ Key Features

* ✅ Handles **multi-source data integration** (Parent & Child companies)
* ✅ Supports **full load and incremental load pipelines**
* ✅ Built using **PySpark on Databricks**
* ✅ Implements **Delta Lake (ACID transactions + upserts)**
* ✅ Designed using **Star Schema (Fact & Dimension tables)**
* ✅ Scalable and production-ready pipeline design

---

## 🔄 Data Pipeline Flow

1. **Ingest Data**

   * Load raw CSV files from parent and child company datasets

2. **Data Cleaning & Transformation**

   * Standardize schema across sources
   * Handle missing/null values

3. **Full Load Processing**

   * Load complete datasets into Delta tables

4. **Incremental Load Processing**

   * Process new/updated records
   * Perform **upserts (MERGE)** using Delta Lake

5. **Data Modeling**

   * Create:

     * Fact Table → `orders`
     * Dimension Tables → `customers`, `products`, `gross_price`

6. **Final Output**

   * Analytics-ready tables for BI tools

---

## 🛠️ Tech Stack

* **Databricks**
* **PySpark**
* **Python**
* **SQL**
* **Delta Lake**
* **ETL Pipelines**

---

## 📊 Use Cases

* Sales Analysis
* Customer Insights
* Revenue Tracking
* Business Intelligence Reporting

---

## 🚀 How to Run

1. Upload project data to **Databricks File System (DBFS)**
2. Import notebooks into Databricks workspace
3. Execute notebooks in order:

   * Data Ingestion
   * Transformation
   * Full Load
   * Incremental Load
4. Query final Delta tables

---

## 📈 Future Improvements

* Add orchestration using **Azure Data Factory / Airflow**
* Integrate **Power BI dashboards**
* Implement **data quality checks & monitoring**
* Automate pipeline scheduling

---

## 👤 Author

**Rohit Gembali**

---

## ⭐ Highlights

* Real-world **FMCG data engineering use case**
* Covers **end-to-end pipeline design**
* Demonstrates **industry-level practices (ETL + Delta Lake + Incremental Loads)**

---
