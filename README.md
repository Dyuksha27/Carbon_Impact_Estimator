# Carbon_Impact_Estimator

This repository contains the **Carbon Impact Estimator Dataset**, developed as part of a research project at **Netaji Subhas University of Technology (NSUT), Delhi, India**.  
The dataset is designed to support studies on **product-level carbon footprint prediction** using machine learning.

---

## Description

The dataset consists of **8,523 product records** and **17 features** capturing essential environmental factors across different stages of a product’s lifecycle.  
It includes attributes related to **production, packaging, and delivery**, such as:

- `Item_Type` – Category or type of product  
- `Item_Weight` – Weight of the product (kg)  
- `Packaging_Type` – Material used for packaging  
- `Supplier_Location`, `Warehouse_Location` – For calculating transport distance  
- `Transport_Mode` – Type of delivery medium (e.g., road, air, ship)  
- `Distance_km` – Distance in km  
- `Product_Emissions`, `Packaging_Emissions`, `Delivery_Emissions` – Stage-wise CO₂e emissions  
- `Total_Emissions` – Aggregated emission target variable (in kg CO₂e)

---

## Model Evaluation

We evaluated multiple regression models to predict total product emissions, including:

- Linear Regression  
- Polynomial Regression (degree 2)  
- Support Vector Regressor (SVR)  
- Decision Tree Regressor  
- Random Forest Regressor  

A **5-Fold Cross Validation** (`KFold(n_splits=5, shuffle=True, random_state=42)`) was performed to ensure robustness.  
The **Random Forest Regressor** achieved the best performance with:

> **Success Rate (±10% tolerance): 94.01%**

---

## Research Paper

**IEEE Xplore:** https://ieeexplore.ieee.org/document/11565046

---

## Usage

The dataset file is available as:  
`Carbon_estimator_dataset.csv`
