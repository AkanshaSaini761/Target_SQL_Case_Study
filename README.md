# 📊 Target Brazil E-Commerce Data Analysis Case Study
## 🏢 About the Company
Target is a globally renowned brand and one of the leading retailers in the United States. With its exceptional guest experience, innovation, and outstanding value, Target has become a preferred shopping destination. This case study focuses on **Target’s operations in Brazil**, analyzing customer orders placed between **2016 and 2018** to uncover actionable insights into their e-commerce performance in the region.

## 🧾 Objective
As a **Data Analyst/Scientist** at Target, your task is to:
* Explore and analyze the dataset of **100,000 Brazilian e-commerce orders**.
* Extract valuable insights regarding customer behavior, operational performance, and sales trends.
* Generate **actionable recommendations** that can help improve Target’s business decisions in Brazil.

## 📂 Dataset Information
The dataset consists of **8 CSV** files:
File Name | Description 
--- | --- 
customers.csv | Contains customer IDs and location (city, state, ZIP)
sellers.csv | Contains seller IDs and location info
order_items.csv | Information about items in each order including price and freight
geolocation.csv | Zip code to latitude/longitude mapping with state and city
payments.csv | Payment details such as type, value, and installments
orders.csv | Details of the order lifecycle and status
reviews.csv | Customer reviews including ratings and messages
products.csv | Product metadata like category, dimensions, and photos

**Dataset schema:**
![image](https://github.com/user-attachments/assets/3c6671fb-5a5d-4542-85ec-3654b359fe66)

## 🔍 Case Study Scope & Analysis Overview
The full analysis — including B**igQuery SQL code**, **screenshots**, and **business insights** — is documented in the attached **PDF**.

### 📌 Exploratory Data Analysis
* Review the **data types** of all columns in the customers table.
* Determine the **time range** of order activity.
* Count the number of **unique cities and states** involved in customer orders.

### 📈 Trend Analysis
* Examine if there is a **year-over-year** growth in the number of orders.
* Explore **monthly** seasonality in order volumes.
* Analyze customer order behavior based on **time of day**:
  * 00–06 hrs → **Dawn**
  * 07–12 hrs → **Morning**
  * 13–18 hrs → **Afternoon**
  * 19–23 hrs → **Night**

### 🌍 Regional E-Commerce Evolution
* Month-on-month **order counts by state**.
* Distribution of customers across **Brazilian states**.

### 💰 Economic Impact Analysis
* Measure the **% increase in payment value** from Jan–Aug 2017 to Jan–Aug 2018.
* Calculate **Total and Average Order Price** by state.
* Calculate **Total and Average Freight Cost** by state.

### 🚚 Sales, Freight & Delivery Performance
* Compute the **delivery time**: `order_delivered_customer_date - order_purchase_timestamp`
* Compute the **estimated vs actual delivery gap**: `order_delivered_customer_date - order_estimated_delivery_date`
* Identify top 5 states by:
  * **Highest & lowest average freight**
  * **Highest & lowest average delivery time**
  * **Fastest average deliveries vs estimates**

### 💳 Payment Insights
* Month-wise count of orders by **payment method**.
* Count of orders grouped by **payment installment** numbers.

## 📎 Deliverables
* 📄 All SQL queries (using **Google BigQuery**) and output screenshots are compiled in the **PDF report**.
* 💡 Final section of the PDF contains **strategic business insights** and **recommendations** based on the analysis.

## 📌 Notes
* All calculations and time-based comparisons are aligned with Brazil’s regional timestamps.
* Payment and freight values are considered in local currency (likely BRL).
* Review performance is evaluated to understand customer satisfaction trends alongside logistics.
