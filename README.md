# 🚀 End-to-End Big Data Engineering Project with Azure | Olist E-Commerce Dataset

This project demonstrates a **real-world big data pipeline** built entirely on **Microsoft Azure**, leveraging **cloud-native tools** and **modern data architecture (Medallion)** to process, transform, and visualize large-scale e-commerce data from **Olist (Brazilian E-Commerce Public Dataset)**.

---

## 🏗️ Architecture Overview

![Project Architecture](Project-Brazillian%20Ecommerce/Architecture%20Diagram.png)

### 🔹 Cloud Platform: Microsoft Azure  
### 🔹 Architecture Type: **Medallion Architecture (Bronze → Silver → Gold Layers)**  

**Key Stages:**
1. **Data Ingestion (Bronze Layer)**  
   - Data sourced from multiple locations (GitHub, SQL tables, APIs).  
   - Ingested using **Azure Data Factory (ADF)**.  
   - Stored in **Azure Data Lake Storage Gen2 (ADLS)**.

2. **Data Transformation (Silver Layer)**  
   - Transformation handled in **Azure Databricks** using **PySpark**.  
   - Applied cleaning, normalization, and joining of multiple data tables.  
   - Integration with **MongoDB** for semi-structured enrichment.

3. **Data Aggregation & Analytics (Gold Layer)**  
   - Aggregated data modeled and loaded into **Azure Synapse Analytics**.  
   - Data prepared for visualization and business insights.

4. **Data Visualization (Final Layer)**  
   - Dashboard created using **Looker Studio**.  

---

## 🧩 Dataset Overview

### 📦 Dataset: **Brazilian E-Commerce Public Dataset by Olist**

**Source:** [Kaggle - Olist Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Data Type:**  
🧩 Structured + Semi-Structured Data  
- **Structured:** Orders, Payments, Products, Customers, Reviews  
- **Semi-Structured:** Geolocation & Seller Information (JSON, text fields)

**Records:** 100K+ orders  

**Key Highlights:**
- Real commercial data (anonymized)  
- Each order may contain multiple items, possibly from different sellers  
- Review text anonymized using Game of Thrones references  

---

## 🧱 Data Schema

![Data Schema](Project-Brazillian%20Ecommerce/Data%20Schema.png)


The dataset is divided into multiple tables for modular understanding:

| Table Name | Description |
|-------------|-------------|
| `olist_orders_dataset` | Order details (status, timestamps, delivery info) |
| `olist_customers_dataset` | Customer demographics and location |
| `olist_order_items_dataset` | Individual product details per order |
| `olist_order_payments_dataset` | Payment methods and values |
| `olist_products_dataset` | Product attributes |
| `olist_order_reviews_dataset` | Customer feedback and ratings |
| `olist_sellers_dataset` | Seller details |
| `olist_geolocation_dataset` | Zip code, latitude, longitude |
| `product_category_name_translation` | English translations of product categories |

---

## 💡 Project Features

✅ Complete **Data Engineering Lifecycle**  
✅ Integration of **Structured and Semi-Structured Data**  
✅ **Cloud-Native Architecture** (Azure)  
✅ **ETL Pipeline Automation** using Azure Data Factory  
✅ **Data Transformation** using Azure Databricks (PySpark)  
✅ **Data Enrichment** with MongoDB  
✅ **Data Warehousing** with Synapse Analytics  
✅ **Data Visualization** using Power BI  
✅ **Scalable and Production-Ready Setup**

---

## 🧰 Tech Stack

| Category | Tools / Services |
|-----------|------------------|
| Cloud Platform | Microsoft Azure |
| Storage | Azure Data Lake Gen2 |
| Ingestion | Azure Data Factory |
| Transformation | Azure Databricks (PySpark) |
| Enrichment | MongoDB |
| Analytics | Azure Synapse |
| Visualization | Looker Studio |
| Dataset Hosting | Filess.io + Kaggle |

---

## 📈 Learning Outcomes

By completing this project, you will gain hands-on experience in:

✅ Implementing **Medallion Architecture**  
✅ Building **real-world data pipelines**  
✅ Handling **structured + unstructured data** 
✅ Performing **ETL on Azure cloud** using Azure Data Factory  
✅ Creating data **visualizations and analytics dashboards** 
✅ **Scalable and Production-Ready Setup**
