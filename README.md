# 🛒 Retail Transaction Data Cleaning & Revenue Analysis

## 📌 Project Overview

This project demonstrates a complete **end-to-end data pipeline**, transforming a large-scale raw retail dataset into a **clean, structured, and business-ready dashboard**. The main focus was on **data cleaning, preprocessing, validation, and financial modeling** to extract actionable business insights from over **10,000+ transaction records**.

The final output includes a **fully interactive Excel dashboard** powered by **Pivot Tables, Power Query, and calculated financial metrics**, enabling efficient decision-making and performance monitoring.

---

## 📄 Dataset Information

| Attribute     | Details                                                 |
| ------------- | ------------------------------------------------------- |
| Filename      | `dataset.csv`                       |
| Total Records | 10,000+ transactions                                    |
| Primary Key   | Transaction_ID                                          |
| Tools Used    | Excel, Power Query, Pivot Tables, Dashboard Design      |
| Objective     | Clean raw data and generate actionable revenue insights |

---

## 📊 Data Dictionary

### Original Columns

| Column Name        | Description                              | Data Type   |
| ------------------ | ---------------------------------------- | ----------- |
| Transaction_ID     | Unique identifier for each transaction   | String      |
| Transaction_Date   | Raw transaction date                     | String      |
| Customer_ID        | Unique identifier for customers          | String      |
| Product_Name       | Product category or name                 | Categorical |
| Quantity           | Number of units purchased                | Integer     |
| Price              | Unit price                               | Float       |
| Return_Flag        | Indicates if product was returned (0/1)  | Binary      |
| Payment_Method     | Method of payment used                   | Categorical |
| Transaction_Status | Status of transaction (Completed/Failed) | Categorical |

---

### Cleaned & Derived Columns

| Column Name      | Description                               | Data Type |
| ---------------- | ----------------------------------------- | --------- |
| Cleaned_Date     | Standardized ISO format date (YYYY-MM-DD) | Date      |
| Cleaned_Quantity | Validated and corrected quantity values   | Integer   |
| Cleaned_Price    | Standardized and validated price values   | Float     |
| Revenue          | Quantity × Cleaned Price                  | Float     |
| Return_Revenue   | Revenue impact of returned items          | Float     |
| Year             | Extracted year for trend analysis         | Integer   |
| Month            | Extracted month for time-series analysis  | Integer   |

---

## 🛠 Data Cleaning & Processing

The dataset underwent extensive cleaning and validation to ensure **100% data integrity**.

### ✔ Date Normalization

* Converted inconsistent date formats into standard ISO format.
* Removed invalid or corrupted date entries.

### ✔ Categorical Standardization

* Fixed inconsistent values caused by:

  * Typos
  * Case sensitivity
  * Duplicate category variations

### ✔ Numerical Validation

* Corrected negative or invalid quantities.
* Standardized currency values.
* Ensured all numeric fields were properly formatted.

### ✔ Feature Engineering

Created new business-critical metrics:

| Feature        | Formula                  | Purpose                            |
| -------------- | ------------------------ | ---------------------------------- |
| Revenue        | Quantity × Cleaned Price | Total revenue per transaction      |
| Return_Revenue | Revenue × Return Flag    | Measures revenue loss from returns |
| Year           | Extracted from Date      | Trend analysis                     |
| Month          | Extracted from Date      | Monthly performance tracking       |

---

## 📈 Key Analysis & Insights

### 💰 Revenue Performance

* Total Revenue exceeded **$911M**
* Clear identification of high-performing product categories

### 🏆 Product Performance

* Top Performers: Smartphones, Laptops
* High Return Categories: Headphones

### 💳 Payment Trends

* Most used methods:

  * PayPal
  * Credit Cards
* Indicates strong preference for digital payment systems

### 📉 Financial Health Monitoring

* Compared Completed vs Failed transactions
* Identified revenue loss areas
* Evaluated return impact on profitability

---

## 🖥 Interactive Dashboard Features

The final dashboard enables real-time business monitoring.

### 🎛 Dynamic Filters (Slicers)

* Filter by:

  * Year
  * Product
  * Payment Method
  * Return Status

### 📊 KPI Cards

* Total Revenue
* Total Transactions
* Return Rate
* Average Revenue

### 📈 Visual Analytics

* Monthly Revenue Trends
* Product Performance Distribution
* Payment Method Analysis
* Return Impact Visualization

---

## ⚙ Tools & Technologies Used

| Tool             | Purpose                            |
| ---------------- | ---------------------------------- |
| Microsoft Excel  | Data cleaning, analysis, dashboard |
| Power Query      | Data transformation                |
| Pivot Tables     | Aggregation and analysis           |
| Excel Charts     | Visualization                      |
| Dashboard Design | Business intelligence reporting    |

---

## 🚀 Project Workflow

```
Raw Dataset
    ↓
Data Cleaning (Power Query)
    ↓
Data Validation & Standardization
    ↓
Feature Engineering
    ↓
Pivot Tables & Analysis
    ↓
Interactive Excel Dashboard
    ↓
Business Insights
```

---

## 📊 Business Value Delivered

* Improved data accuracy to **100% clean dataset**
* Enabled clear visibility into **revenue trends**
* Identified **top products and revenue drivers**
* Provided decision-ready **interactive dashboard**
* Supported **data-driven strategic planning**

