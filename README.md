# 🏅 Tokyo Olympics Data Pipeline & Analytics  

This project showcases an **end-to-end data engineering pipeline** for analyzing the Tokyo 2020 Olympics dataset.  
It leverages **Azure Data Factory (ADF), Azure Databricks (PySpark), and Azure Synapse Analytics** to build a modern, scalable data solution for ingesting, transforming, and analyzing large volumes of event and athlete data.  

---

## 🚀 Project Workflow  

1. **Data Ingestion**  
   - Raw CSV files (`athletes.csv`, `coaches.csv`, `entriesgender.csv`, `medals.csv`, `teams.csv`) stored in GitHub.  
   - ADF pipeline fetches data from GitHub via **HTTP connector**.  
   - Files ingested into **Azure Data Lake Gen2** under `raw_data/`.  

2. **Data Transformation**  
   - Azure Databricks reads raw data from the lake.  
   - Applied **data cleaning, type casting, deduplication, and enrichment** with PySpark.  
   - Outputs written into `transformed_data/` as curated CSV/Parquet.  

3. **Data Loading**  
   - Data loaded into **Azure Synapse Analytics (SQL Pool)**.  
   - Created structured tables: `athletes`, `coaches`, `entriesgender`, `medals`, `teams`.  

4. **Analytics & Visualization**  
   - Performed SQL-based analysis in Synapse Studio.  
   - Built dashboards in **Power BI** to showcase medal counts, gender participation, and country-level performance.  

---

## 🛠️ Tech Stack  

- **Azure Data Factory (ADF)** – Orchestrates ingestion from GitHub to Azure Data Lake  
- **Azure Data Lake Gen2 (ADLS)** – Stores raw and transformed Olympic datasets  
- **Azure Databricks (PySpark)** – Performs data cleaning, enrichment, and transformation  
- **Azure Synapse Analytics** – Hosts analytical tables for querying and reporting  
- **Power BI / Tableau** – Visualizes medal counts, gender participation, and country performance  
- **SQL** – Analytical queries for trend analysis and performance reporting  
- **Python** – Data manipulation and transformation scripts  

---

## 📂 Repository Structure  

```plaintext
tokyo-olympics-data-pipeline/
│
├── datasets/                  # Raw Olympic datasets (CSV files from GitHub)
│
├── notebooks/                 # Databricks PySpark notebooks for transformations
│
├── docs/                      # Documentation and architecture diagrams
│   ├── pipeline_architecture.png
│   ├── data_flow.png
│   └── data_catalog.md
│
├── scripts/                   # SQL scripts for Synapse Analytics
│
├── dashboards/                # Power BI / Tableau dashboards
│
├── tests/                     # Validation queries and test scripts
│
└── README.md                  # Project overview
```

---

## 🎯 Key Skills Demonstrated  

- Building **end-to-end data pipelines** with Azure ADF, Databricks, and Synapse.  
- Implementing **data lakehouse architecture** for structured reporting.  
- Writing **PySpark transformations** for scalable data cleaning and enrichment.  
- Designing **SQL-based analytics** for medal trends, gender participation, and country performance.  
- Delivering **interactive dashboards** with Power BI for real-world event insights.  

---

## 📈 Example Insights  

- **Medal distribution** by country, gender, and sport.  
- **Athlete participation trends** across categories and nations.  
- **Coach and team-level performance analytics**.  
- **Comparative gender analysis** showing participation rates across events.  

---
