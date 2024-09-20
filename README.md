# Sales Data Analysis

This repository contains an analysis of sales data with data transformation, modeling, and visualization to address specific business needs. The goal is to extract key insights related to sales, profit, and quantity sold, and to model the data for optimal performance using a star schema design.

## Table of Contents
- [Data Transformation](#data-transformation)
- [Data Merging](#data-merging)
- [Data Modeling](#data-modeling)
- [Business Insights](#business-insights)
- [Visualizations](#visualizations)

## Data Transformation

The first step involved cleaning and transforming the data for analysis:
- **Renaming Sheets**: Renamed `Sheet3` to `Fact Table` to ensure consistent and clear naming conventions.
- **Header Renaming**: Changed the header of the `Dim Promotion` table for clarity.
- **Conditional Formatting**: Applied conditional formatting to the `Promotion Code` column, converting it to a percentage format for easy interpretation.

## Data Merging

We merged multiple tables to create a comprehensive dataset:
- **Fact Table and Dim Product Merge**: Merged the `Fact Table` with the `Dim Product` table using the `Product_ID` key, enabling us to pull in the price per product.
- **Custom Columns**: Created custom columns to calculate:
  - `Discount Value`
  - `Total Sales`
  - `Profit`
  - `Net Sales`

## Data Modeling

We structured the data using a **Star Schema** to optimize query performance:
- **Relationships**: Defined relationships between the `Fact Table` and dimensional tables (such as products, customers, and promotions) to ensure a clean and efficient model for data analysis.

## Business Insights

This analysis addresses several key business questions:

1. **Top/Bottom 5 Products**: Ranked the top and bottom 5 products by:
   - Sales
   - Profit
   - Quantity Sold
2. **Sales Trends Over Time**: Evaluated how sales trends vary over time, examining:
   - Daily
   - Monthly
   - Quarterly
   - Annually
3. **Sales & Profit Relationship**: Visualized the relationship between sales and profit to uncover correlations.
4. **Period Comparison**: Compared sales, profit, and quantity sold between any two user-selected periods.
5. **Discount Analysis**: Calculated the average discount offered in each discount category.
6. **Total Orders**: Displayed the total number of orders.
7. **Filterable Sales Details**: Displayed detailed sales metrics (e.g., Sales, Profit, Discount, Net Sales) for each order, which could be filtered using visual filters like:
   - Product
   - Date
   - Customer ID
   - Promotion Category
8. **City-Wise Sales**: Showed the total sales breakdown by different cities.

## Visualizations

The following visualizations were created to facilitate the business insights:
- **Bar Charts**: To show the top/bottom 5 products by sales, profit, and quantity sold.
- **Line Charts**: To analyze sales trends over time (daily, monthly, quarterly, and annually).
- **Scatter Plots**: To depict the relationship between sales and profit.
- **Slicers**: Allow users to filter by period, product, date, customer ID, and promotion category.
- **City Map**: Displaying sales distribution across different cities.

---

## How to Use

Clone the repository and run the analysis using the following steps:
1. Clone the repository: 
   ```bash
   git clone https://github.com/yourusername/sales-data-analysis.git
