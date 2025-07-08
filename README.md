# Customer Segmentation Using RFM Analysis

This project performs data cleaning, exploratory analysis, and customer segmentation using **RFM analysis** on an e-commerce dataset. The goal is to identify customer loyalty levels for targeted marketing strategies.

---



## Objectives

- Clean and preprocess e-commerce transaction data  
- Perform exploratory data analysis (EDA)  
- Segment customers using RFM (Recency, Frequency, Monetary) method  
- Visualize loyalty levels using treemaps  

---

## 1. Data Cleaning & EDA

- Removed duplicates (6008 rows)  
- Dropped columns with high null values or irrelevant features  
- Removed rows with missing `CustomerID`  
- Converted date fields to datetime format  
- Removed negative prices and verified data consistency  

---

## 2. RFM Customer Segmentation

**RFM** stands for:  
- **Recency** – How recently a customer made a purchase  
- **Frequency** – How often a customer made purchases  
- **Monetary** – How much money a customer spent  

### Steps Performed

- Aggregated transactions per customer  
- Scored customers on R, F, and M using quartiles (1–4 scale)  
- Combined scores into a total RFM score  
- Classified customers into four loyalty levels:  

| Loyalty Level | Description             |
|---------------|-------------------------|
| Platinum      | Most loyal, high spenders |
| Gold          | Frequent buyers         |
| Silver        | Average engagement      |
| Bronze        | Least active customers  |

### Loyalty Distribution

| Loyalty Level | Customers |
|---------------|-----------|
| Platinum      | 1280      |
| Gold          | 1313      |
| Silver        | 966       |
| Bronze        | 790       |

---

## Treemap Visualization

A treemap shows the number of customers per loyalty level.

