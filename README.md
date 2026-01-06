🌍 Countries by GDP – Data Engineering ETL Project
📌 Project Overview

This project simulates a real-world Data Engineering task where an international firm requires an automated solution to extract, transform, and store country GDP data published by the International Monetary Fund (IMF).

As a Junior Data Engineer, the goal is to build an ETL pipeline that:

Extracts GDP data from the IMF website

Transforms it into a clean, structured format

Stores it in both JSON and SQLite database

Logs the full execution process

Validates results using SQL queries

🛠️ Technologies Used

Python

Web Scraping (Requests / BeautifulSoup / Pandas)

JSON

SQL

Logging

🔄 ETL Pipeline Workflow
1️⃣ Extract

Scrapes the list of countries and their GDP values from the IMF website.

GDP values are extracted in USD billions.

2️⃣ Transform

Rounds GDP values to 2 decimal places.

Sorts countries by GDP in descending order.

3️⃣ Load

Saves the transformed data to:

Countries_by_GDP.json

SQLite database: World_Economies.db

Table name: Countries_by_GDP

Columns:

Country

GDP_USD_billion




This query displays countries with economies exceeding 100 billion USD.

📝 Logging

The entire ETL execution process is logged in:

etl_project_log.txt

Logs include:

Start and end time

Extraction status

Transformation steps

Load confirmation

Errors (if any)

📁 Project Structure
├── Countries_by_GDP.json
├── World_Economies.db
├── etl_project_log.txt
├── etl_script.py
└── README.md

🎯 Key Skills Demonstrated

Real-world ETL pipeline design

Data extraction from external sources

Data transformation and validation

Database creation and querying

Automation and logging

Data Engineering best practices
