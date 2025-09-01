# 📦 Online Orders Details (MySQL Project)

## 📌 Project Overview  
This project demonstrates how to design and analyze an **Online Orders database** using **MySQL Workbench**.  
It covers database creation, table design, and advanced SQL queries including **aggregations, GROUP BY, HAVING, subqueries, CTEs, and window functions**.  

The analysis generates insights such as:  
- Total Orders and Revenue  
- Orders and Revenue by Payment Method  
- Top Products by Sales Revenue  
- Orders above average order value  
- Products priced above average unit price  
- Top-selling product by revenue  
- Country-level sales and revenue analysis  
- Product ranking using **Window Functions**  

---

## 🎯 Objectives  
- Create a **data repository** inside MySQL Workbench  
- Import raw data from a `.csv` file  
- Apply SQL queries to analyze sales, revenue, and product trends  
- Explore **basic to advanced SQL concepts**:  
  - Aggregations (`COUNT`, `SUM`, `AVG`)  
  - Filtering (`WHERE`, `HAVING`)  
  - Grouping & Ordering (`GROUP BY`, `ORDER BY`)  
  - Subqueries  
  - Common Table Expressions (CTEs)  
  - Window Functions  

---

## ⚙️ Tools Used  
- **MySQL Workbench** → database creation & queries  
- **PowerPoint** → project documentation  

---

## 🛠️ Queries & Results  

### 1. Database & Table Creation  
```sql
CREATE DATABASE Online_Orders_Details;

USE Online_Orders_Details;

CREATE TABLE Orders_Details (
  Order_ID INT PRIMARY KEY,
  Country VARCHAR(20),
  Product_Category VARCHAR(50),
  Product VARCHAR(20),
  Unit_Price INT,
  Quantity INT,
  Total_Price INT,
  Order_Purchased_Date DATE,
  Order_Received_Date DATE,
  Payment_Method VARCHAR(50),
  Review_Rating INT
);
![Image 1](images/image1.jpeg)
