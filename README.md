# ☁️ AWS RDS ETL Pipeline Analytics

A **cloud-integrated ETL pipeline** built using **AWS RDS (MySQL) and Pandas**, designed to extract, transform, and analyze relational data for analytics use cases.

This project focuses on **data pipeline engineering**, demonstrating how raw relational data is processed into structured analytical outputs using Python.

---

## 🚀 Features

- ☁️ **Cloud database integration (AWS RDS - MySQL)**
- 🔄 **End-to-end ETL pipeline (Extract → Transform → Load)**
- 🔗 **Multi-table joins and relational data processing**
- 🧠 **Feature engineering using Pandas**
- 📊 **Aggregated analytics metrics generation**
- ⚡ **Notebook-based pipeline execution**

---

## 🧠 What This Project Demonstrates

This project highlights the following **data engineering and backend skills**:

- **Working with cloud-hosted relational databases (AWS RDS)**
- **SQL + Python interoperability**
- **Designing ETL pipelines using Pandas**
- **Relational data modeling and joins**
- **Data cleaning and transformation workflows**
- **Aggregation and analytics dataset creation**

---

## 📂 Project Structure

```
AWS_RDS_ETL_PIPELINE_ANALYTICS/
│
├── ETL_PIPELINE/
│   └── etl_pipeline.ipynb   # Core ETL pipeline implementation
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## ⚙️ Architecture Overview

The project follows a **cloud-based ETL pipeline architecture**.

```
AWS RDS (MySQL)
        │
        ▼
Data Extraction (mysql-connector)
        │
        ▼
Pandas DataFrames
        │
        ▼
Data Transformation
(joins, cleaning, feature engineering)
        │
        ▼
Aggregation Layer
(groupby, metrics computation)
        │
        ▼
Analytical Dataset
```

### Design Principles

- **Separation of extraction, transformation, and aggregation**
- **Relational data processing using Pandas**
- **Cloud-first data access**
- **Reproducible analytics pipeline**

---

## 🔄 ETL Workflow

### 1️⃣ Extract

- Connects to **AWS RDS MySQL instance**
- Retrieves data from multiple tables:
  - `delivery`
  - `player`
  - `player_captain`

---

### 2️⃣ Transform

- Performs **multi-table joins** using keys:
  - `Player_Id`
  - `Match_Id`
- Cleans and filters data
- Handles missing values
- Builds intermediate datasets

Example transformations:

- Mapping players to captaincy status  
- Combining match-level and player-level data  

---

### 3️⃣ Load (Analytical Output)

- Generates aggregated datasets using:
  - `groupby()`
  - conditional filtering  

Computed metrics:

- Total runs  
- Balls faced  
- Number of boundaries (fours)  

---

## 🛠 Installation

### Clone repository

```bash
git clone https://github.com/your-username/AWS_RDS_ETL_PIPELINE_ANALYTICS.git
cd AWS_RDS_ETL_PIPELINE_ANALYTICS
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

1. Create an **AWS RDS MySQL instance**  
2. Create required tables:
   - `delivery`
   - `player`
   - `player_captain`  
3. Insert your dataset  
4. Update DB credentials inside:

```
ETL_PIPELINE/etl_pipeline.ipynb
```

5. Run all notebook cells  

---

## ⚠️ Data Availability

This repository **does NOT include datasets or database access**.

The original AWS RDS instance has been removed intentionally.

---

## 🚧 Limitations

- Notebook-based implementation (not modularized)
- No orchestration (Airflow / Prefect not used)
- No logging or monitoring
- No automated deployment

---

## 📈 Potential Improvements

Future enhancements could include:

- Convert notebook into **modular Python pipeline (`src/` structure)**
- Add **workflow orchestration (Airflow / Prefect)**
- Integrate **AWS S3 for storage layer**
- Add **logging and monitoring (CloudWatch)**
- Containerize using **Docker**
- Add **CI/CD pipeline for deployment**

---

## 🧰 Tech Stack

| Technology | Purpose |
|-----------|--------|
| Python | Programming language |
| AWS RDS | Cloud database |
| MySQL | Relational database |
| Pandas | Data processing |
| mysql-connector-python | Database connection |
| Jupyter Notebook | Development environment |

---

## 🎯 Learning Outcomes

This project helped build understanding of:

- **ETL pipeline design and implementation**
- **Cloud database integration**
- **Relational data transformations**
- **Aggregation pipelines for analytics**
- **Foundations of data engineering systems**

---

## 👤 Author

**Rudra Tyagi**

B.Tech Final Year Student  
Aspiring **ML Systems / MLOps / AI Infrastructure Engineer**