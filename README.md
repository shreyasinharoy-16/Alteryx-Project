# Alteryx Sales Analytics Pipeline

A multi-workflow **ETL (Extract, Transform, Load)** and **Sales Analytics** solution built using **Alteryx Designer**. This project demonstrates end-to-end data integration, transformation, and sales reporting by processing customer, product, and sales data from multiple data sources.

---

## Project Overview

The pipeline is divided into three independent workflows that prepare and integrate data for sales analysis. The final workflow combines all processed datasets to generate summarized sales reports and business insights.

---

## Workflow 1: Customer Data Workflow

### Description

Processes customer information from multiple file formats, cleans and standardizes the data, and prepares it for downstream analytics.

### Key Tasks

* Import customer data from:

  * CSV
  * Text (.txt)
  * Excel (.xlsx)
  * ZIP files
* Clean and standardize customer records
* Remove inconsistencies and duplicates
* Apply age categorization using Formula tools
* Export the processed dataset

**Output:** `Customer_Final.csv`

---

## Workflow 2: Product Data Workflow

### Description

Processes product information stored in XML format and transforms it into a structured dataset.

### Key Tasks

* Read XML source files
* Parse XML data
* Clean and restructure product records
* Prepare product data for joining with sales transactions
* Export the processed dataset

**Output:** `Product_Final.csv`

---

## Workflow 3: Sales Analysis Workflow

### Description

Combines processed customer and product data with sales transactions to generate analytical reports.

### Key Tasks

* Import sales data from:

  * SQL Database
  * AWS-hosted CSV files
* Standardize date formats
* Calculate shipping duration using **DateTimeDiff**
* Compute running sales totals
* Join sales data with customer and product datasets
* Generate monthly and yearly sales summaries
* Calculate customer counts and other aggregated metrics

**Output:** Sales Summary Reports

---

## Alteryx Tools Used

* Input Data
* Multi-File Input
* XML Parse
* Join
* Formula
* DateTimeDiff
* Running Total
* Summarize
* Select
* Filter
* Output Data

---

## Project Workflow

```
Customer Data
      │
      ▼
Customer_Final.csv
      │
      ├──────────────┐
      │              │
      ▼              ▼
Sales Data      Product_Final.csv
      │              ▲
      │              │
      └────── Join ──┘
              │
              ▼
     Sales Analytics
              │
              ▼
     Summary Reports
```

---

## Output Files

* `Customer_Final.csv`
* `Product_Final.csv`
* Sales Summary Reports

---

## Workflow Screenshots

Add screenshots of each workflow below:

* Customer Data Workflow
<img width="1342" height="525" alt="Customer_Workflow" src="https://github.com/user-attachments/assets/fb2dd5d7-583c-4f75-96a9-4b68db4416d5" />

* Product Data Workflow
<img width="1004" height="299" alt="Product_Workflow" src="https://github.com/user-attachments/assets/085ee943-9850-4c62-ab85-1dee92d9ea0b" />

* Sales Analysis Workflow
<img width="4058" height="546" alt="Sales_Workflow_Complete" src="https://github.com/user-attachments/assets/96a55215-3fae-43b9-a77d-0e300a7727c7" />

---

## Technologies Used

* Alteryx Designer
* SQL
* AWS CSV Data Sources
* XML
* CSV
* Microsoft Excel

---

## Skills Demonstrated

* ETL Pipeline Development
* Data Cleaning & Transformation
* Multi-Source Data Integration
* XML Parsing
* SQL Data Integration
* Data Blending
* Sales Analytics
* Business Reporting
* Workflow Automation
