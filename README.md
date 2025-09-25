# 📊 Online Retail Analysis – Business Intelligence Project  

## 📌 Introduction  
This project is tailored to assist a **UK-based online retail company** by developing a **data-driven solution** that enables insightful analysis and informed decision-making.  
It provides valuable insights into:  
- Customer purchasing behavior  
- Product performance  
- Sales trends across different regions and time periods  

---

## 🎯 Business Needs  
- Decide in which **country** to open a physical store  
- Decide which **products** to market more  

---

## 🛠️ Goals  
- **Data Warehouse Implementation:** Create a robust data warehouse for efficient storage, retrieval, and analysis of transactional data  
- **Enhanced Decision-Making:** Provide actionable insights by analyzing historical sales data  
- **Performance Monitoring:** Track sales performance across products, customers, and time  

---

## 📂 Deliverables  
- Comprehensive **data model**  
- Implementation of an **ETL process** to populate the data warehouse  
- **Interactive dashboards** in Power BI  

---

## 🚀 Implemented Phases  

### 1️⃣ Data Collection and Preprocessing  
- Collected raw transactional data (invoices, product details, customer info)  
- Cleaned data: removed inconsistencies, handled missing values, standardized formats  
- Example: Missing customer IDs were replaced with unique IDs  

---

### 2️⃣ ETL Process Implementation  
- **Extraction:** Data from `online_retail.xlsx` and `customers.xlsx`  
- **Transformation:**  
  - Changed data types  
  - Split columns (e.g., date into day, month, year)  
  - Derived new columns (e.g., revenue = unit price × quantity)  
- **Loading:** Exported transformed data as CSV and imported into **PostgreSQL**  

---

### 3️⃣ Data Modeling  
- Designed a **Snowflake schema** with:  
  - Central fact table: `order_fact`  
  - Dimension tables: `customer_dim`, `customer_address_dim`, `time_dim`, `invoice_info_dim`, `product_dim`, `product_category_dim`, `product_info_dim`  
- Chose Snowflake schema to normalize dimensions (e.g., customer table split into related tables)  

---

### 4️⃣ OLAP Implementation  
- Used **Power BI** connected to PostgreSQL  
- Implemented **MOLAP (Import Mode)** → preloads data into memory for fast queries  

---

### 5️⃣ Dashboard Development  
- Created Power BI dashboards with KPIs:  
  - Total sales  
  - Top-selling products  
  - Top-buying customers  
- Added drill-down (year → month → day) and roll-up capabilities  
- Included filters (e.g., gender, country) for deeper insights  

---

## ✅ Conclusion  
Challenges solved:  
- Data quality issues (missing & inconsistent values)  
- Extensive preprocessing and validation steps  

---

## 🔮 Possible Enhancements  
- Automate ETL for better scheduling and monitoring  
- Implement **HOLAP** for balance between storage and query performance  
- Add predictive analytics with ML  
- Expand warehouse with **social media & customer feedback data** for sentiment analysis  

 
