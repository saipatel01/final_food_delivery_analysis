# Food Delivery Dataset Integration & Analysis

This repository contains the final submission for the GenAI Internship assessment.  
The objective of this project is to integrate multiple data sources into a single dataset and perform analytical queries to extract meaningful insights.


## 📄 Problem Overview
The task involves working with three different data formats:
- CSV (Transactional data)
- JSON (User master data)
- SQL (Restaurant master data)

These datasets are merged using appropriate join keys to create a unified dataset that serves as the single source of truth for analysis.

## 📂 Input Data Sources
- **orders.csv** – Contains order-level transactional details
- **users.json** – Contains user information and membership details
- **restaurants.sql** – Contains restaurant details such as cuisine and rating

## 🔗 Data Integration Approach
- `orders.csv` is merged with `users.json` using **user_id**
- `orders.csv` is merged with `restaurants.sql` using **restaurant_id**
- Join type used: **LEFT JOIN**, ensuring no order records are lost

## 📊 Analysis Highlights
The analysis focuses on:
- Order distribution by membership type
- Revenue analysis across cities and cuisines
- Average order value calculations
- Impact of restaurant ratings on order volume
- Validation of merged dataset integrity

All analytical questions are answered using the final merged dataset only.

## 📁 Repository Contents
- `final_food_delivery_analysis.ipynb` – Jupyter Notebook with full workflow
- `final_food_delivery_dataset.csv` – Final merged dataset
- `orders.csv` – Raw order data
- `users.json` – Raw user data
- `restaurants.sql` – Raw restaurant data

## 🛠️ Technologies Used
- Python
- Pandas
- SQLite
- Jupyter Notebook

