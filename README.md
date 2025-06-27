# FIRST STEPS WITH DATABRICKS: FROM ZERO TO LAKEHOUSE 

Welcome to the hands-on workshop for learning **Databricks Lakehouse Architecture** using the analogy of a **Library System**. This end-to-end demo showcases how to build scalable data pipelines using Bronze, Silver, and Gold layers to transform and prepare data for reliable analytics and reporting.

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
4. **Insights (Visualization Dashboard)**

---

## Dataset Overview

- `books.csv` — ~1,000 books with metadata
- `borrowers.csv` — ~10,000 borrowing records
- `staff.csv` — ~20 staff members


## How to Run the Project

> **Prerequisites**: Databricks Free Version or Enterprise Account Edition

### 1. Clone the repository onto your local

   - open your terminal and type the following code:
      git clone `https://github.com/Rashidomar/workshop_demo_databricks.git`
      This will clone the project onto your local machine
     
     **Please note location of your cloned repo**
     
   - On Mac, Windows and Linux, Enter the command below to give the location of cloned repo
      command : pwd
     
      **This location will be required to upload your notebooks onto the databricks platform**

### 2. Create Notebooks on Databricks account by following the below steps

   1. Navigate to  `Workspace` on Databricks
       - From the left menu, go to the user workspace by:  
       - clicking on Workspace > Users > `username@email_domain.com`: when you get here, create a folder called `workshop_demo_databricks`
   2. Notebook Upload: To upload the notebook:
      - Open the newly created folder workshop_demo_databricks
      - Click on the three dotted icon on the top right-hand side
      - From the pop up, select import.
      - From the import window, click on browse, Navigate to where your repo was cloned
      - Select the three notebooks from the SQL_Notebook folder, that is `bronze_layer`,`silver_layer` and `gold_layer`
      - Click on import
      - On successful import, you will see the message: **Successfully imported 3 files**
   3. You can now view and run the imported notebooks from your Databricks Workspace

### The Medallion Architecture of the library System
#### A medallion architecture is a data design pattern we are going to use to logically organize data with the goal of incrementally and progressively improving the structure and quality of data as it flows through each layer of the architecture from **Bronze ⇒ Silver ⇒ Gold layer tables**
![screenshot](images/Medal.png)


### The Data Model of the library System
#### The data model defines the structure and relationships within your data. It serves as a blueprint for how data is stored, understood, and used across the organization. This is going general view of our datasets.

![screenshot](images/model.png)


### The Visualization Dashboard
#### A dashboard translates data into actionable insights through visual storytelling. It allows decision-makers to monitor, explore, and act on key metrics in real time.

![screenshot](images/Dash.png)

---

## Workshop Learning Goals

✅ Understand the Databricks Lakehouse concept  
✅ Apply Medallion Architecture best practices  
✅ Build an end-to-end ETL   
✅ Learn Delta Lake, Spark SQL, PySpark in context  

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
- TheDataLead AI : www.thedatalead.ai
- All participants building the future with data
---

