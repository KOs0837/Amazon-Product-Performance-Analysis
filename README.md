# Amazon product performance analysis

## Poject Overview
This project explores Amazon product data to evaluate product performance using customer ratings, review volume, pricing, and discount patterns. Since the dataset does not include actual sales or transaction-level information, performance is assessed through proxy indicators such as rating count, average rating, and discount strategy.


## Business Objectives
The main goals of this project are to:
- identify the most reviewed products
- compare average ratings across product categories
- analyze price and discount distributions
- evaluate how discounts relate to customer ratings and review counts
- highlight strong and weak performing products using proxy performance indicators

## Dataset
The dataset contains Amazon product information, including:
- product name
- category
- discounted price
- actual price
- discount percentage
- rating
- rating count
- review title and review content

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning
The data cleaning process included:
- removing currency symbols from price columns
- converting `actual_price` and `discounted_price` into numeric format
- cleaning and converting `discount_percentage`
- converting `rating` and `rating_count` into numeric values
- handling missing values in `rating_count`
- splitting the hierarchical `category` column into `main_category`, `sub_category1`, and `sub_category2`

## Feature Engineering
To support the analysis, additional variables were created:
- `savings_amount`: difference between actual price and discounted price
- `discount_percentage_display`: discount percentage in readable format
- `performance_score`: simple proxy indicator based on rating and rating count

## Exploratory Data Analysis
The EDA focused on:
- rating distribution
- discounted price distribution
- top categories by product count
- top reviewed products
- average rating by category
- relationship between discount percentage and rating
- relationship between discounted price and rating

## Key Insights
- Some categories show consistently high average ratings, indicating stronger customer satisfaction.
- A limited number of products concentrate a very large share of total reviews.
- Categories such as Computers & Accessories dominate the dataset in product volume.
- Higher discounts do not automatically lead to better ratings.
- Review count appears to be a strong proxy for product visibility and customer engagement.

## Business Recommendations
- Prioritize highly rated and highly reviewed products in promotional campaigns.
- Reassess discount strategies for products with large discounts but only average ratings.
- Use top-performing categories as benchmarks for weaker categories.
- Investigate products with low ratings despite strong visibility to identify quality or positioning issues.

## Limitations
This dataset does not contain actual sales volume, revenue, or time-based transaction data. As a result, product performance cannot be measured through direct business KPIs such as sales growth or profitability. Instead, proxy indicators such as ratings, review counts, and discount patterns were used.
