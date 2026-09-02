# 🏗️ SQL Data Warehouse Project (PostgreSQL + Medallion Architecture)

Welcome to my **SQL Data Warehouse Project**! This repository showcases an end-to-end data warehousing solution built using **PostgreSQL**, following the **Medallion Architecture** (Bronze → Silver → Gold). The project demonstrates how raw data can be ingested, cleaned, transformed, and modeled into business-ready insights using pure SQL.

---

## 🏛️ Data Architecture

The project follows the **Medallion Architecture**, consisting of three layers:

1. **🥉 Bronze Layer** – Stores raw, unprocessed data exactly as ingested from source files (CSV) into PostgreSQL tables. No transformations are applied here.
2. **🥈 Silver Layer** – Cleans, standardizes, and normalizes the Bronze data. Handles missing values, duplicates, and inconsistent formats to make data analysis-ready.
3. **🥇 Gold Layer** – Houses business-ready, aggregated data modeled for reporting and analytics (e.g., star schema, views).

---

## 📖 Project Overview

This project involves:

- **Data Architecture**: Designing a modern data warehouse using the Medallion (Bronze, Silver, Gold) architecture in PostgreSQL.
- **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse using SQL scripts.
- **Data Modeling**: Building fact and dimension tables optimized for analytical queries.
- **Filtering & Cleaning**: Applying filters, joins, and transformations to remove noise and prepare high-quality datasets.
- **Analytics & Reporting**: Writing SQL queries to generate insights such as trends, aggregations, and performance reports.

---

## 🎯 Objective

The goal is to build a modern data warehouse using PostgreSQL to:

- Consolidate data from multiple sources into a single, reliable warehouse.
- Perform data cleaning, filtering, and quality checks to resolve inconsistencies.
- Enable fast, efficient SQL-based analytics for business reporting.

---

## 🗂️ Repository Structure

```
sql-data-warehouse-projects/
│
├── datasets/               # Raw source datasets (CSV files) used for the project
│
├── docs/                   # Project documentation, architecture diagrams, and data catalog
│
├── scripts/                # SQL scripts for ETL and transformations
│   ├── bronze/              # Scripts to load raw data into the Bronze layer
│   ├── silver/              # Scripts to clean and transform data into the Silver layer
│   └── gold/                 # Scripts to build the final analytical models in the Gold layer
│
├── tests/                  # SQL scripts for data quality checks and validation
│
└── README.md               # Project overview and instructions
```

---

## 🚀 Getting Started

### Prerequisites

- [PostgreSQL](https://www.postgresql.org/download/) installed (v13 or later recommended)
- [pgAdmin](https://www.pgadmin.org/) or any PostgreSQL client
- Git (for cloning the repository)

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/PixelNomad-lang/sql-data-warehouse-projects.git
   cd sql-data-warehouse-projects
   ```

2. **Create the database**
   - Open your PostgreSQL client and create a new database (e.g., `datawarehouse`).

3. **Load the Bronze layer**
   - Run the scripts inside `scripts/bronze/` to create tables and load raw data from `datasets/`.

4. **Build the Silver layer**
   - Run the scripts inside `scripts/silver/` to clean and transform the Bronze data.

5. **Build the Gold layer**
   - Run the scripts inside `scripts/gold/` to create the final, business-ready views/tables.

6. **Run tests**
   - Execute scripts in the `tests/` folder to validate data quality across all layers.

---

## 🛠️ Tools & Technologies

- **Database**: PostgreSQL
- **Architecture**: Medallion (Bronze, Silver, Gold)
- **Language**: SQL
- **Version Control**: Git & GitHub

---

## 📊 Key Operations Performed

- Data ingestion from CSV files into PostgreSQL
- Data filtering, deduplication, and cleaning
- Joins and transformations across multiple tables
- Aggregations for reporting (sales trends, customer insights, etc.)
- Data quality/validation checks

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repository, raise issues, or submit pull requests to improve the project.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

Got questions or suggestions? Feel free to open an issue on this repository.
