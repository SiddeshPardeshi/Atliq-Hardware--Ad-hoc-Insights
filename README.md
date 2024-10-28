# Atliq-Hardware-Ad-hoc-Insights

# Problem Statement
Atliq Hardware (imaginary company), a top player in the computer hardware industry both in India and internationally, has hit a roadblock. The management has noticed that they’re not getting the insights they need to make quick and smart decisions based on data. This lack of timely information is holding them back from responding effectively to market demands and competition. To tackle this challenge, Atliq Hardware has decided to launch an SQL challenge aimed at digging into their sales, product, and customer data.The goal? To uncover valuable insights that will help management make informed decisions, adapt their strategies, and ultimately drive the business forward.

# Tasks
Conduct sales, product, and customer data analysis to address specific business questions.
Use SQL for data extraction and trend identification.
Communicate insights effectively to support high-level management decisions.

# Dataset Overview
The analysis was conducted using data from the 'gdb023' (atliq_hardware_db) database, which includes six main tables.

1. dim_customer: contains customer-related data
2. dim_product: contains product-related data
3. fact_gross_price: contains gross price information for each product
4. fact_manufacturing_cost: contains the cost incurred in the production of each product
5. fact_pre_invoice_deductions: contains pre-invoice deductions information for each product
6. fact_sales_monthly: contains monthly sales data for each product.

# Tools Used
- SQL: For querying and analyzing the data.
- Visualization Tool: Power Bi for data visualisation.
- Microsoft PowerPoint: For Presentation.

# Ad-hoc Requests & SQL Queries

## 1. Provide the list of markets in which customer "Atliq Exclusive" operates its business in the APAC region.
```sql
SELECT market FROM dim_customer
WHERE customer = 'Atliq Exclusive' AND region = 'APAC';


