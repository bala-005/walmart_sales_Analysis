# Walmart Sales Analysis: End-to-End SQL + Python Project

## Overview

This project provides an end-to-end data analysis solution for extracting business insights from Walmart sales data. We leverage Python for data processing, SQL for advanced querying, and structured problem-solving techniques to answer key business questions. This project is ideal for data analysts looking to enhance their skills in data manipulation, SQL querying, and data pipeline creation.

---

## Project Workflow

### 1. Environment Setup
- **Tools Used**: Visual Studio Code (VS Code), Python, SQL (MySQL & PostgreSQL)
- **Objective**: Create a well-structured workspace for efficient development and data handling.

### 2. Kaggle API Configuration
- **Steps**:
  - Download the Kaggle API key (`kaggle.json`) from your [Kaggle profile](https://www.kaggle.com/).
  - Save it in the `.kaggle` folder.
  - Use `kaggle datasets download -d <dataset-path>` to fetch datasets.

### 3. Data Acquisition
- **Dataset**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)
- **Storage**: Save downloaded data in the `data/` directory.

### 4. Library Installation & Data Loading
- **Install Dependencies**:
  ```bash
  pip install pandas numpy sqlalchemy mysql-connector-python psycopg2
  ```
- **Load Data**: Use Pandas to read the dataset into a DataFrame for analysis.

### 5. Exploratory Data Analysis (EDA)
- **Objective**: Understand data distribution, column types, and potential issues.
- **Key Methods**:
  - `.info()`, `.describe()`, `.head()`

### 6. Data Cleaning
- **Tasks**:
  - Remove duplicate records.
  - Handle missing values (drop or fill appropriately).
  - Standardize data types (`datetime`, `float`, etc.).
  - Format currency values.

### 7. Feature Engineering
- **Enhancements**:
  - Create a new column: `Total Amount = unit_price * quantity`.
  - Improve dataset usability for SQL queries.

### 8. Data Ingestion into MySQL & PostgreSQL
- **Connections**:
  - Use `sqlalchemy` to connect Python with databases.
  - Automate table creation and data insertion.
- **Validation**:
  - Run SQL queries to ensure data integrity.

### 9. SQL Analysis & Business Insights
- **Key Queries**:
  - Revenue trends by branches & categories.
  - Best-selling product categories.
  - Sales performance by time, city, and payment method.
  - Peak sales periods & customer buying patterns.
  - Profit margin analysis.
- **Documentation**: Maintain clear descriptions of each query's purpose and results.

### 10. Project Documentation & Publishing
- **Documentation**:
  - Maintain detailed project notes in Markdown or Jupyter Notebook.
- **Publishing**:
  - Upload project files to GitHub, including:
    - `README.md`
    - Jupyter Notebooks (if used)
    - SQL scripts
    - Data access steps

---

## Requirements

- **Python**: 3.8+
- **Databases**: MySQL, PostgreSQL
- **Libraries**:
  - `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`, `psycopg2`
- **Kaggle API Key** (for data downloading)

## Getting Started

1. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up Kaggle API, download data, and follow the workflow.

---

## Project Structure

```plaintext
|-- data/                     # Raw and processed data
|-- sql_queries/              # SQL scripts for analysis
|-- notebooks/                # Jupyter notebooks (if applicable)
|-- README.md                 # Project documentation
|-- requirements.txt          # Python dependencies
|-- main.py                   # Main script for data processing
```

---

## Key Insights

- **Sales Trends**: Identified top-performing categories, branches, and preferred payment methods.
- **Profitability Analysis**: Most profitable products and locations.
- **Customer Behavior**: Insights into ratings, payment preferences, and peak shopping hours.

## Future Enhancements

- Integrate a dashboard (e.g., Power BI, Tableau) for visualization.
- Incorporate additional data sources for deeper insights.
- Automate data pipelines for real-time analysis.


## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart business case studies on sales and supply chain optimization

