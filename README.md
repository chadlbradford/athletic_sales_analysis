
# Athletic Sales Analysis

This project analyzes sales data from 2020 and 2021 to extract meaningful insights into product sales performance, regional trends, retailer activity, and specific product category sales. The analysis focuses on identifying high-performing regions, retailers, and products while leveraging various Python data manipulation and aggregation techniques.

---

## Table of Contents
1. [Overview](#overview)
2. [Setup and Installation](#setup-and-installation)
3. [Data Overview](#data-overview)
4. [Key Analysis Steps](#key-analysis-steps)
    - [Combine and Clean the Data](#1-combine-and-clean-the-data)
    - [Region with the Most Product Sales](#2-determine-which-region-sold-the-most-products)
    - [Region with the Most Total Sales](#3-determine-which-region-had-the-most-sales)
    - [Top Retailers by Sales](#4-determine-which-retailer-had-the-most-sales)
    - [Women's Athletic Footwear Analysis](#5-determine-which-retailer-sold-the-most-womens-athletic-footwear)
    - [Day and Week with the Most Sales](#6-determine-the-day-with-the-most-womens-athletic-footwear-sales-and-7-week-with-the-most-sales)
5. [Results](#results)
6. [License](#license)

---

## Overview
This project analyzes historical sales data from multiple regions to understand patterns and provide actionable insights. Techniques like `groupby` and `pivot_table` are employed to aggregate data and derive insights. The analysis also focuses on a specific product category—Women's Athletic Footwear.

---

## Setup and Installation
1. **Prerequisites**:
   - Python 3.8 or higher
   - `pandas` library installed

2. **Installation**:
   ```bash
   pip install pandas
   ```

3. **Project Structure**:
   ```
   ├── Resources/
   │   ├── athletic_sales_2020.csv
   │   ├── athletic_sales_2021.csv
   ├── main.py  # Script containing the analysis
   ```

4. **Run the Analysis**:
   Execute the script:
   ```bash
   python main.py
   ```

---

## Data Overview
The data consists of two CSV files for 2020 and 2021 sales. Each file includes columns such as:
- `region`, `state`, `city`: Location details
- `retailer`: Retailer name
- `product`: Product category
- `units_sold`: Units sold
- `total_sales`: Total sales value
- `invoice_date`: Date of sale

---

## Key Analysis Steps

### 1. Combine and Clean the Data
- **Import CSV Files**: Load sales data from 2020 and 2021.
- **Combine Data**: Merge data row-wise and reset the index.
- **Clean Data**:
  - Check for null values.
  - Convert `invoice_date` to `datetime` format.

### 2. Determine Which Region Sold the Most Products
- Use `groupby` and `pivot_table` to calculate the total products sold by `region`, `state`, and `city`.
- Identify the top-performing regions based on product sales.

### 3. Determine Which Region Had the Most Sales
- Use `groupby` and `pivot_table` to calculate total sales by `region`, `state`, and `city`.
- Highlight the regions generating the highest revenue.

### 4. Determine Which Retailer Had the Most Sales
- Analyze total sales for each `retailer`, segmented by `region`, `state`, and `city`.
- Use `groupby` and `pivot_table` to determine top-performing retailers.

### 5. Determine Which Retailer Sold the Most Women's Athletic Footwear
- Filter the dataset for Women's Athletic Footwear.
- Aggregate sales data by `retailer` to identify high-performing retailers.

### 6. Determine the Day with the Most Women's Athletic Footwear Sales
- Resample sales data by day and sort in descending order to identify peak sales days.

### 7. Determine the Week with the Most Women's Athletic Footwear Sales
- Resample sales data by week and sort to find the week with the highest sales.

---

## Results
- **Region Performance**:
  - Identified regions contributing the most to sales volume and revenue.
- **Retailer Insights**:
  - Highlighted retailers dominating sales overall and in specific product categories.
- **Product Trends**:
  - Pinpointed top-performing product categories and seasonal trends.
- **Time-Based Trends**:
  - Identified peak sales days and weeks for targeted marketing campaigns.

---


## **References**
Chatgpt was used to troubleshoot self generated code.

---
