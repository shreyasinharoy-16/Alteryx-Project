Alteryx Sales Analytics Pipeline
A multi-workflow ETL and sales analytics solution built in Alteryx Designer.

Workflows:
1. Customer Data Workflow
Imports data from multiple formats: CSV, Text, Excel, ZIP
Blends, cleans and standardises customer records
Applies age categorisation logic
Output: Customer_Final.csv
2. Product Data Workflow
Parses and transforms XML source data
Cleanses and restructures product records
Output: Product_Final.csv
3. Sales Analysis Workflow
Ingests sales data from SQL and AWS CSV sources
Converts and standardises date formats
Calculates shipping duration (DateTimeDiff)
Computes running sales totals
Joins with Customer and Product datasets
Performs monthly/yearly sales aggregation
Output: Sales summary reports with customer counts
Tools Used:
Alteryx Designer, Multi-file Input, XML Parse, Join, Formula, Summarise, DateTimeDiff, Running Total

Workflow Screenshots:
<img width="1004" height="299" alt="Product_Workflow" src="https://github.com/user-attachments/assets/704188ab-2cad-434b-9564-4370590c0a97" />
<img width="4058" height="546" alt="Sales_Workflow_Complete" src="https://github.com/user-attachments/assets/a27a5ac0-3f8a-4b37-8e57-064bb2cb57c1" />
<img width="1342" height="525" alt="Customer_Workflow" src="https://github.com/user-attachments/assets/acddd499-4e4f-432e-85ce-829875b80101" />
