# 📊 E-Commerce Sales & Profitability Analysis

## 📌 Project Overview

This project analyzes **e-commerce sales, customer behavior, product performance, profitability, and delivery operations** using **Excel, SQL, and Power BI**.

The project follows a complete Data Analyst workflow:

**Raw Data → Excel Cleaning → SQL Analysis → Power BI Dashboard → Business Insights**

The objective is to transform raw e-commerce data into meaningful insights that can support business and operational decision-making.

---

## 🎯 Business Objectives

The analysis focuses on:

* Understanding overall sales and profit performance
* Analyzing monthly sales trends
* Identifying top-performing categories and products
* Understanding customer segments
* Analyzing regional and state-wise performance
* Measuring profitability and profit margins
* Evaluating delivery performance
* Identifying high-value customers
* Creating an interactive Power BI dashboard

---

# 🛠️ Tools & Technologies

| Tool                | Purpose                                   |
| ------------------- | ----------------------------------------- |
| **Microsoft Excel** | Data cleaning, validation and preparation |
| **SQL Server**      | Data analysis and business logic          |
| **Power BI**        | Dashboard development and visualization   |
| **GitHub**          | Project documentation and version control |

---

# 🔄 End-to-End Project Workflow

```text
Raw E-Commerce Dataset
        ↓
Excel Data Cleaning
        ↓
Data Validation
        ↓
SQL Data Analysis
        ↓
Business KPI Calculation
        ↓
Power BI Data Modeling
        ↓
Interactive Dashboard
        ↓
Business Insights
```

---

# 📂 Dataset

The dataset contains e-commerce transaction information related to:

* Orders
* Customers
* Products
* Categories
* Customer segments
* Regions
* States
* Sales
* Profit
* Quantity
* Discounts
* Shipping
* Delivery status

### Key Columns

```text
order_id
order_date
customer_id
customer_first_name
customer_last_name
customer_segment
customer_region
customer_state
product_name
category_name
order_quantity
sales_per_order
profit_per_order
order_item_discount
shipping_type
delivery_status
days_for_shipment_scheduled
days_for_shipment_real
```

---

# 🧹 Excel Data Cleaning

**Microsoft Excel was used as the first stage of data preparation.**

The raw dataset was imported into Excel and reviewed before being loaded into SQL and Power BI.

### Data Cleaning Activities

#### 1. Missing Value Check

Checked important columns for:

* Blank values
* Missing customer information
* Missing product information
* Missing category values
* Missing sales/profit values
* Missing dates

Used Excel functions such as:

```excel
=COUNTBLANK(A:A)
```

and

```excel
=IF(A2="","Missing","Available")
```

---

#### 2. Duplicate Check

Duplicate records were identified using Excel's **Remove Duplicates** functionality and duplicate-checking formulas.

Example:

```excel
=COUNTIF($A:$A,A2)
```

This helped identify records where the same Order ID appeared multiple times.

---

#### 3. Data Type Validation

Validated the correct data types for:

* Order Date → Date
* Sales → Number
* Profit → Number
* Quantity → Whole Number
* Discount → Number
* Customer ID → Text/Identifier

---

#### 4. Date Cleaning

The `order_date` field was reviewed and standardized so that it could be used consistently for:

* Monthly analysis
* Yearly analysis
* Time-series reporting
* Power BI date filtering

---

#### 5. Text Cleaning

Customer, product, category, and location fields were checked for inconsistent formatting.

Functions used included:

```excel
=TRIM(A2)
```

```excel
=CLEAN(A2)
```

```excel
=PROPER(A2)
```

---

#### 6. Error Handling

Excel was used to identify and handle common data errors.

Examples:

```excel
=IFERROR(A2/B2,0)
```

```excel
=IF(ISBLANK(A2),"Unknown",A2)
```

---

#### 7. Numerical Validation

Checked for:

* Negative sales
* Negative/incorrect quantities
* Unusual discount values
* Profit inconsistencies
* Incorrect shipment durations

---

#### 8. Data Validation

Before moving the data to SQL, key fields were checked for consistency and completeness.

The cleaned dataset was then used for SQL analysis and Power BI reporting.

---

# 🗄️ SQL Data Analysis

After Excel cleaning, SQL Server was used for business analysis.

### SQL Concepts Used

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* `COUNT`
* `COUNT DISTINCT`
* `SUM`
* `AVG`
* `CASE WHEN`
* `HAVING`
* `CTE`
* Date functions
* Conditional aggregation
* Window functions
* `RANK()`

### Key SQL Analysis

* Overall business KPIs
* Monthly sales and profit
* Category performance
* Top products
* Customer segment analysis
* State-wise performance
* Profit margin analysis
* Delivery performance
* Customer value segmentation
* Customer ranking

---

# 📊 Power BI Dashboard

The cleaned and analyzed data was used to create an interactive Power BI dashboard.

### Key KPIs

* 💰 Total Sales
* 📈 Total Profit
* 🛒 Total Orders
* 👥 Total Customers
* 📦 Total Quantity
* 💵 Average Order Value

### Dashboard Analysis

The dashboard provides analysis of:

* Sales trends
* Profit trends
* Category performance
* Product performance
* Customer segments
* Regional performance
* State-wise sales
* Delivery status
* Profitability

### Interactive Filters

Users can filter the dashboard by:

* Date
* Category
* Customer Segment
* Region
* State
* Product
* Delivery Status

---

# 📈 Business Insights

The analysis helps identify:

### Revenue Drivers

Categories, products, customer segments, and regions contributing to sales.

### Profitability

Comparison of revenue and profit to identify profitable and less-profitable areas.

### Customer Value

Customer segmentation based on purchasing contribution.

### Product Performance

Top-performing and low-performing products based on sales and profit.

### Operational Performance

Delivery and shipment performance across different order types.

---

# 📁 Repository Structure

```text
Ecommerce-Sales-Analysis/
│
├── 📂 Data/
│   └── ecommerce_data.csv
│
├── 📂 Excel/
│   └── ecommerce_cleaned.xlsx
│
├── 📂 SQL/
│   └── ecommerce_analysis.sql
│
├── 📂 PowerBI/
│   └── ecommerce_dashboard.pbix
│
├── 📂 Screenshots/
│   └── dashboard.png
│
└── README.md
```

---

# 🚀 Skills Demonstrated

### Excel

* Data cleaning
* Missing-value handling
* Duplicate detection
* Error handling
* Data validation
* Text cleaning
* Date cleaning
* Data preparation

### SQL

* Data aggregation
* `CASE WHEN`
* CTEs
* Date analysis
* Conditional aggregation
* Window functions
* Ranking
* Business KPI analysis

### Power BI

* Data modeling
* KPI development
* Interactive dashboards
* Data visualization
* Slicers and filters
* Business reporting

### Business Analysis

* Sales analysis
* Profitability analysis
* Customer analysis
* Product analysis
* Regional analysis
* Operational analysis

---

# 💡 Project Value

This project demonstrates a complete **end-to-end Data Analyst workflow**:

```text
Raw Data
   ↓
Excel Cleaning
   ↓
Data Validation
   ↓
SQL Analysis
   ↓
KPI Development
   ↓
Power BI Visualization
   ↓
Business Insights
```

It demonstrates how raw transactional data can be transformed into a structured analytical dataset and finally presented through an interactive business intelligence dashboard.

---

# 👨‍💻 Project Type

**Data Analyst Portfolio Project**

**Tools:** Excel | SQL Server | Power BI | GitHub

**Domain:** E-Commerce Analytics

**Focus:** Sales | Profitability | Customers | Products | Operations
