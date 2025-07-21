# Customer-Lifetime-Value-CLV-Prediction-Using-BG-NBD-and-Gamma-Gamma-Models


## 📌 Introduction

In today’s competitive retail environment, understanding and predicting customer value is essential for strategic decision-making. This project leverages the UCI Online Retail Dataset to estimate Customer Lifetime Value (CLV) using probabilistic models. Specifically, the BG/NBD (Beta Geometric/Negative Binomial Distribution) and Gamma-Gamma models are applied to capture purchasing frequency and monetary value respectively.


The goal is to identify high-value customers and support data-driven marketing strategies such as personalized offers, customer segmentation, and retention efforts.



## 🧾 Dataset Overview

Source: UCI Machine Learning Repository – Online Retail

Data Range: December 2010 – December 2011

Key Columns:

InvoiceNo: Unique transaction code

StockCode: Product identifier

Description: Product name

Quantity: Units purchased

InvoiceDate: Date of transaction

UnitPrice: Price per unit

CustomerID: Unique customer ID

Country: Country of customer



## ⚙️ Tools and Libraries

Programming Language: Python

Libraries:

pandas, numpy: Data manipulation

lifetimes: CLV modeling

matplotlib, seaborn: Visualization



## 🧼 Data Preprocessing

Steps:

Removed null CustomerIDs

Filtered out cancelled/negative transactions

Created TotalPrice as Quantity * UnitPrice

Parsed and standardized InvoiceDate


## 📊 Modeling Approach

1. BG/NBD Model – Predict Purchase Frequency
   
The BG/NBD model estimates:

How often a customer will make a purchase in a given time window

The probability that a customer is still "alive" (i.e., active)

2. Gamma-Gamma Model – Predict Average Spend
   
This model assumes:

Transaction monetary value is independent of purchase frequency

Gamma distributions govern individual-level monetary averages

3. CLV Estimation
   
CLV is calculated over a 6-month horizon with a monthly discount rate.


## 📈 Results and Insights

Predicted future purchases and monetary values for each customer

Identified top 10 customers with the highest CLV

Generated visual insights to support business targeting


## ✅ Conclusion

This project demonstrates how probabilistic models can be applied to real-world e-commerce data to derive actionable insights. By using BG/NBD and Gamma-Gamma models, we accurately estimated future customer behavior and value, enabling more informed marketing strategies.

