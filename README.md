📊 E-Commerce Product Analysis Dashboard (Power BI)
📌 Project Overview
This project is an interactive Power BI dashboard for analyzing e-commerce product performance, pricing, discounts, and customer feedback.
It uses a dataset of products, prices, discounts, ratings, reviews, and image/product links to provide insights for data-driven decision-making.

📂 Dataset
The dataset includes the following columns:

product_id: Unique identifier for each product
product_name: Name of the product
category: Product category (multi-level)
discounted_price: Price after discount
actual_price: Original product price
discount_percentage: Discount applied (%)
rating: Average product rating
rating_count: Total number of ratings
about_product: Product description
user_id: Reviewer IDs
user_name: Reviewer names
review_id: Unique review identifiers
review_title: Title of the review
review_content: Full review text
img_link: Product image URL
product_link: Clickable product page link
🎯 Objectives
Track total products, discounts, and customer satisfaction
Compare actual vs discounted prices
Analyze the relationship between price, discount, and rating
Explore customer review insights
Build a visual product catalog with images and clickable links
📊 Dashboard Pages
1️⃣ Executive Overview
KPI cards: Total Products, Avg Discount %, Avg Rating, Total Ratings
Donut chart: Products by Category
Bar chart: Top 10 Products by Rating Count
Table with product images and clickable links
2️⃣ Pricing & Discounts Analysis
Clustered Column Chart: Actual vs Discounted Price
Scatter Plot: Discounted Price vs Rating
Box Plot: Distribution of Discounts by Category
3️⃣ Customer Reviews & Catalog
Word Cloud: Most common review terms
Reviews Table: Reviewer, Rating, and Comments
Product Catalog with images and links
📌 Key DAX Measures
Total Products = DISTINCTCOUNT(Products[product_id])

Average Discount % = AVERAGE(Products[discount_percentage])

Average Rating = AVERAGE(Products[rating])

Total Ratings = SUM(Products[rating_count])

Total Discounted Sales = SUM(Products[discounted_price])

Total Savings = SUMX(Products, Products[actual_price] - Products[discounted_price])

Weighted Discount % =
DIVIDE(
    SUMX(Products, Products[actual_price] - Products[discounted_price]),
    SUM(Products[actual_price])
) * 100
About
This project is an **interactive Power BI dashboard** for analyzing e-commerce product performance, pricing, discounts, and customer feedback. It uses a dataset of products, prices, discounts, ratings, reviews, and image/product links to provide insights for data-driven decision-making.

Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Footer
