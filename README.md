# Data-Science-Internship-Week8
# E-Commerce Product Performance Analysis (Brazilian Olist Dataset)
## Project Overview

This project is an end-to-end business analysis of an e-commerce platform using the Brazilian Olist multi-table dataset. The goal is to evaluate product and category performance, generate insights, and provide actionable recommendations for business improvement.

The analysis includes revenue, sales volume, customer ratings, and category-level trends, aimed at optimizing the product catalog, improving customer satisfaction, and enhancing revenue generation.

## Dataset

The Brazilian Olist dataset contains 9 CSV files capturing real-world e-commerce operations from 2016 to 2018:

CSV File	Description
olist_orders_dataset.csv	Orders with status, timestamps, and customer IDs
olist_order_items_dataset.csv	Items per order with product IDs, price, and freight
olist_products_dataset.csv	Product details including category ID
product_category_name_translation.csv	Portuguese to English translation for product categories
olist_order_reviews_dataset.csv	Customer reviews and ratings per order
olist_order_payments_dataset.csv	Payment details including total paid and payment type
olist_customers_dataset.csv	Customer demographic and location data
olist_sellers_dataset.csv	Seller information and locations
olist_geolocation_dataset.csv	Geolocation coordinates of customers and sellers

Dataset source: Olist Public Dataset on Kaggle

## Business Problem

E-commerce platforms need to understand which products and categories drive revenue and which underperform. This analysis addresses:

Which products generate the highest revenue?

Which products have high/low customer satisfaction?

Which product categories dominate sales or require improvement?

Recommendations for promotions, discontinuations, or price adjustments.

## Methodology
1. Data Preparation

    Loaded all 9 CSV files into a single analysis-ready dataframe.

    Filtered only delivered orders.

    Merged datasets to associate each order item with:

        Product details

        Category name (translated to English)

        Customer reviews

        Payment info

    Converted date columns to datetime format for temporal analysis.

    Handled missing values and ensured clean, structured data.

2. Exploratory Data Analysis (EDA)

  Calculated key metrics per product and category:

    Total revenue

    Quantity sold

    Average customer rating

  Visualized:

    Top 10 products by revenue

    Top 10 categories by revenue

    Category-wise quantity sold

    Average rating per category

  Used bar charts and heatmaps to highlight trends and outliers.

3. Key Insights

  Identified top-performing products and categories driving most revenue.

  Detected underperforming products with low sales and/or ratings.

  Observed categories with high customer satisfaction but low sales, indicating marketing opportunities.

4. Recommendations
  | Product / Category          | Recommended Action                                                            |
  | --------------------------- | ----------------------------------------------------------------------------- |
  | High Revenue & High Rating  | Promote via marketing campaigns, bundle deals, or feature on homepage         |
  | Low Revenue & Low Rating    | Consider discontinuation, product quality improvements, or targeted discounts |
  | High Rating & Low Sales     | Increase visibility through email campaigns, ads, or homepage features        |
  | High Quantity & Low Revenue | Adjust pricing, bundle offers, or upsell/cross-sell products                  |

## Tools & Libraries
  Python 3

  Pandas – Data cleaning and manipulation

  NumPy – Numerical computations

  Matplotlib & Seaborn – Visualizations

  Google Colab – Cloud-based notebook environment

## Project Workflow

  Define business problem → E-commerce product performance analysis

  Data acquisition → Download and load Olist dataset

  Data preprocessing & cleaning → Merge tables, filter orders, handle missing data

  Exploratory analysis → Revenue, sales, rating, and category-level insights

  Visualization → Bar charts, heatmaps, top product/category plots

  Insights & recommendations → Actionable strategies to optimize business outcomes

  Documentation → Professional README & portfolio-ready notebook

## Portfolio Outcome

  This project demonstrates:

  End-to-end data analysis workflow

  Translating raw data into actionable business insights

  Ability to communicate results clearly with visualizations and recommendations

  Readiness to showcase a professional data-driven project in a portfolio
