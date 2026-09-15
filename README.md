# EasyCart – E-Commerce Sales & Customer Analytics

## 📌 Project Overview

EasyCart is a fictional e-commerce analytics project developed to analyze sales, customers, products, sellers, orders, deliveries, and returns.

The project uses **SQL for data analysis** and **Power BI for interactive business reporting and visualization**.

The main objective is to understand business performance and identify useful insights from e-commerce transaction data.

---

## 🎯 Business Objectives

- Analyze overall sales and order performance
- Identify top-performing products and categories
- Analyze customer spending and purchasing behavior
- Evaluate seller performance
- Analyze monthly revenue trends
- Understand order status distribution
- Analyze city-wise revenue
- Monitor delivery and shipment performance
- Analyze product return reasons
- Create an interactive Power BI dashboard

---

## 🛠️ Tools & Technologies

- **MySQL** – Database creation and SQL analysis
- **Power BI** – Data modeling, DAX and dashboard development
- **Microsoft Excel / CSV** – Dataset preparation
- **GitHub** – Project documentation and version control

---

## 🗄️ Database Structure

The EasyCart database contains 13 related tables:

1. Customers
2. Customer Sessions
3. Brands
4. Categories
5. Products
6. Sellers
7. Orders
8. Order Items
9. Payments
10. Warehouses
11. Shipments
12. Returns
13. Reviews

### Business Flow

Customer → Session → Product → Order → Payment → Shipment → Delivery → Review / Return

---

## 📊 SQL Analysis

The project includes 30 SQL queries covering:

### Sales & Orders

- Total orders and revenue
- Total quantity sold
- Average Order Value
- Order status analysis
- Monthly revenue
- Monthly order count

### Products & Categories

- Top products by quantity
- Top products by revenue
- Category-wise revenue
- Category-wise quantity
- Brand-wise revenue
- Average selling price by category

### Customers

- Top customers by spending
- Customer order analysis
- Repeat customer analysis
- Average customer spending
- City-wise customer analysis
- City-wise revenue

### Sellers

- Seller revenue performance
- Seller order count
- Seller rating vs performance

### Delivery & Returns

- Average delivery time
- Delayed shipments
- Warehouse shipment performance
- Return reason analysis

### Advanced SQL

- RANK()
- DENSE_RANK()
- LAG()
- Running total using SUM() OVER()
- CTE
- CASE-based customer segmentation

---

## 📈 Power BI Dashboard

The Power BI dashboard provides an interactive view of EasyCart's business performance.

### Key KPIs

- **Total Orders:** 300
- **Total Revenue:** ₹2.11M
- **Average Order Value:** ₹7.02K
- **Total Quantity Sold:** 913

### Dashboard Visuals

- Monthly Revenue Trend
- Revenue by City
- Revenue by Category
- Top 10 Products by Revenue
- Orders by Status
- Seller Revenue Performance

### Filters

- Order Date
- Product Category

---

## 💡 Key Business Insights

- EasyCart generated approximately **₹2.11M in revenue** from 300 orders.
- A total of **913 product units** were sold.
- **Toys** generated the highest category revenue.
- **UrbanX** generated the highest brand revenue.
- **UrbanX Board Game** was the top product by revenue.
- **Pune** generated the highest city-wise revenue.
- **Delivered** orders represented the largest share of total orders.
- Monthly revenue showed noticeable fluctuations, with strong performance in **April and July**.
- Seller performance varied significantly across sellers, providing opportunities for performance comparison.

---

## 📂 Project Structure

```text
EasyCart-Ecommerce-Analytics
│
├── Dashboard
│   └── EasyCart_Dashboard.png
│
├── Dataset
│   ├── customers.csv
│   ├── customer_sessions.csv
│   ├── brands.csv
│   ├── categories.csv
│   ├── products.csv
│   ├── sellers.csv
│   ├── orders.csv
│   ├── order_items.csv
│   ├── payments.csv
│   ├── warehouses.csv
│   ├── shipments.csv
│   ├── returns.csv
│   └── reviews.csv
│
├── Power BI
│   └── EasyCart_Ecommerce_Analytics.pbix
│
└── SQL
    └── easycart_sql_queries.sql
```

---

## 🚀 Project Workflow

```text
Raw CSV Data
      ↓
MySQL Database
      ↓
SQL Analysis
      ↓
Power BI Data Model
      ↓
DAX Measures
      ↓
Interactive Dashboard
      ↓
Business Insights
```

---

## 🧮 Power BI DAX Measures

The dashboard uses DAX measures for important business KPIs such as:

- Total Revenue
- Total Orders
- Average Order Value
- Total Quantity Sold

Example:

```DAX
Total Revenue =
SUMX(
    'easycart order_items',
    'easycart order_items'[quantity] *
    'easycart order_items'[unit_price]
    - 'easycart order_items'[discount]
)
```

---

## 📷 Dashboard Preview

The dashboard screenshot is available in the **Dashboard** folder.

The Power BI `.pbix` file is available in the **Power BI** folder.

---

## 📚 Skills Demonstrated

- SQL
- MySQL
- Data Analysis
- Relational Databases
- Data Modeling
- Table Relationships
- SQL Joins
- Aggregations
- Subqueries
- CTEs
- Window Functions
- DAX
- Power BI
- Interactive Dashboards
- KPI Development
- Business Insights

---

## ▶️ How to Use

### SQL

1. Open MySQL Workbench.
2. Create the `easycart` database.
3. Import the CSV files from the **Dataset** folder.
4. Use the SQL queries available in the **SQL** folder.
5. Execute the queries to reproduce the analysis.

### Power BI

1. Open `EasyCart_Ecommerce_Analytics.pbix`.
2. Connect to the EasyCart data source if required.
3. Refresh the data.
4. Use the available filters and visuals to explore the dashboard.

---

## ⚠️ Note

**EasyCart is a fictional e-commerce project created for educational, analytical, and portfolio purposes.**

The dataset is created for project analysis and does not represent a real company's confidential data.

---

## 👨‍💻 Author

### Jeet Kalal

**BCA Student | Aspiring Data Analyst**

**Skills:** SQL | Python | Pandas | NumPy | Excel | Power BI

---

⭐ If you find this project useful, feel free to explore the SQL analysis, dataset, and Power BI dashboard.
