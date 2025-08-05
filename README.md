# [POWER BI] Analyze Purchasing Performance of AdventureWorks - a bicycle manufacturer for Operational Efficiency
## 1. Introduction

### 1.1. Business question
The Purchasing Department requested the Data Analyst Team to build an Operational Dashboard to give leadership a concise and intuitive overview, assisting in decision-making and boosting operational efficiency. This document serves as an introduction to the Dashboard development process, provides user instructions, and includes the team's key recommendations.

### 1.2: Dataset
Dataset: adventureworks2019 (public Google BigQuery dataset)

Dataset Dictionary: Please refer to the 'Data Dictionary' file attached above

Dataset access:
- Log in to your Google Cloud Platform account and create a new project.
- Navigate to the BigQuery console and select your newly created project.
- In the navigation panel, select "Add Data" and then "Star a project by name".
- Enter the project name "adventurework2019"

## 2. Design Thinking Process

### Stage 1: Empathize
- **5W1H**

<img src="https://github.com/user-attachments/assets/8b9a6372-54f8-4838-b38c-8fbc060aceaa" alt="5W1H" width="1050" />

- **Empathy Map**
<img src="https://github.com/user-attachments/assets/5381a46e-ad21-458c-9576-98ac9abf4265" alt="Empathy Map" width="1050" />

### Stage 2: Northstar Metric and POV
<img src="https://github.com/user-attachments/assets/4c898324-cc58-40dd-a19f-731ac4c76f0c" alt="Northstar" height="400" /> <img src="https://github.com/user-attachments/assets/9442edb9-23b4-494b-be71-35f3b7ad43dd" alt="Northstar" height="400" />

### Stage 3: Ideate
![Image](https://github.com/user-attachments/assets/bf482e96-e2c0-4ed7-ba1b-7b7859b8a386)

## 3. Data Modeling
Connect relevant tables from the dataset in BigQuery to Power BI, clean the data, and apply data modeling techniques to organize and optimize it for analysis.
![Image](https://github.com/user-attachments/assets/86e5f449-1f50-4a2c-b40e-e4dc2e7be8d0)

## 4. Visualization
### 4.1. Purchasing Overview
<img width="1304" height="757" alt="Image" src="https://github.com/user-attachments/assets/e74c3d07-c3d2-4339-b111-95ddcc4ecf19" />

- The Net purchase witnessed an increase over time, from Q1 2012 around 2 million USA before reaching a peak at approximately 18 million USA in Q2 2014 (Note: Q3 2014 data is unavailable, so there is no conclusion about a significant decline).
- A majority of purchase is from preferred vendors, accounts for over 90%.
- Rejected Rate is quite low and stable.
- Purchase from vendor with low credit ratings is at acceptable level.
### 4.2. Inventory Report
<img width="1303" height="753" alt="Image" src="https://github.com/user-attachments/assets/9284ce77-0ec0-4674-b508-8a96d8977f9e" />

- Subassembly and Miscellaneous Storage are two locations that have the highest inventory quantity (95K units and 83K units) but have low inventory value ($3.3M and $1.5M respectively). There are many items stored but have low value.
- Some product quantities are under safety stock level that they need purchasing. 

### 4.3. Vendor Performance
<img width="1302" height="756" alt="Image" src="https://github.com/user-attachments/assets/1050ff65-89fe-4ade-8a5c-7fc5a779a1de" />

Present the vendor profiles and performance metrics, allowing the purchasing department to gain insights and conduct future analysis.

## 5. Recommendations
- **Vendor selection**: Remain the current situation with purchasing focuses on preferred vendors and vendor with high credit rating. Try to reduce lead time in order to get purchasing on time.
- **Improve inventory replenishment**: Address 69 SKUs below safety stock level immediate to prevent shortages for production and sales.
- **Inventory tracking over time**: The information about inventory is not updated regularly; therefore, it is essential to build a system for tracking inventory over time to enable analysis, better inventory management decisions.
- **Inventory Management**: Need to balance inventory across locations to avoid overstock and maintain optimal stock levels.


