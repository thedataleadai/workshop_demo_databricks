# FIRST STEPS WITH DATABRICKS: FROM ZERO TO LAKEHOUSE 

Welcome to the hands-on workshop for learning **Databricks Lakehouse Architecture** using the analogy of a **Library System**. This end-to-end demo showcases how to build scalable data pipelines using Bronze, Silver, and Gold layers, and train a machine learning model to predict **late book returns**.

---

## Project Summary

This project simulates a public library managing:
- Books
- Borrowers
- Library staff

It walks participants through:
1. **Raw data ingestion (Bronze)**
2. **Data cleaning & enrichment (Silver)**
3. **Analytics (Gold)**
4. 4. **Insigts (Visualization Dashboard)**

---

## Dataset Overview

The data is synthetically generated with realistic fields and scale:
- `books.csv` — ~1,000 books with metadata
- `borrowers.csv` — ~10,000 borrowing records
- `staff.csv` — ~20 staff members


## How to Run the Project

> **Prerequisites**: Databricks Community or Enterprise Workspace

### 1. Clone the repository into Databricks

Upload the notebooks or use Git integration if you're using Databricks Repos.

### 2. Load dataset inoto volune 

Generates synthetic datasets and stores them in `/Volumes/demo_catalog/library_schema/library_volume/`.

### 3. Run `02_medallion_pipeline.py`

- Ingests raw data to **Bronze**
- Cleans and enriches to **Silver**
- Aggregates analytics in **Gold**

---


## 📈 Gold-Level Outputs

| Table | Description |
|-------|-------------|
| `most_borrowed_books.gold` | Top borrowed books by count |
| `delay_by_genre.gold` | Avg delay days per genre |
| `staff_count_by_role_gold` | Total  number of staff per role|

---

## Workshop Learning Goals

✅ Understand the Databricks Lakehouse concept  
✅ Apply Medallion Architecture best practices  
✅ Build an end-to-end ETL   
✅ Learn Delta Lake, Spark SQL, PySpark, in context  

---

## Built With

- Databricks free edition
- PySpark / Spark SQL
- Delta Lake
---

## License

This project is open for educational use under the MIT License.
---

## Acknowledgments

Special thanks to:
- TheDatalead AI
- All participants building the future with data
---

