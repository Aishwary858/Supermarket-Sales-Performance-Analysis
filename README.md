# Supermarket Sales Performance Analysis

A comprehensive Power BI report analyzing supermarket sales performance, customer behavior, and profitability across multiple branches and product lines.

![Report Screenshot](<img width="1030" height="491" alt="Image" src="https://github.com/user-attachments/assets/9b9b0361-8cc2-4e5d-87bb-aa2ee8a66739" />)

## 📊 Project Overview

This project provides stakeholders with actionable insights into sales trends, customer preferences, and profitability metrics to support data-driven business decisions including inventory management, pricing strategies, and customer retention initiatives.

## 🎯 Objectives

- Analyze supermarket sales performance focusing on revenue and profitability
- Perform customer segmentation analysis
- Evaluate customer satisfaction ratings across branches and product lines
- Identify top-performing branches and product categories
- Track purchasing trends by demographics and payment methods

## 📈 Key Metrics & KPIs

- **Total Sales**: 323K
- **Total Transactions**: 1,000
- **Average Quantity**: 5.51 units per transaction
- **Average Unit Price**: $55.67
- **Average Customer Rating**: 6.97/10

*Source: Live dashboard data as of latest refresh*

## 🏢 Stakeholders

- **Store Managers**: Track branch-level performance and sales trends
- **Product Managers**: Gain insights into high-demand product lines
- **Finance Teams**: Assess profitability and revenue across branches
- **Marketing Teams**: Create targeted campaigns based on customer behavior
- **Customer Experience Teams**: Understand satisfaction levels and improve service

## 📊 Dashboard Features

### Visual Analytics
- **Sales by Product Line and Gender**: Horizontal bar chart showing gender-based purchasing patterns
- **Rating by Gender and Product Line**: Bubble chart visualization showing satisfaction levels
- **Gross Income by Gender and Payment Method**: Donut chart displaying payment preferences
- **Interactive Filters**: City and Payment method slicers for dynamic analysis
- **KPI Cards**: Key performance indicators prominently displayed

### Interactive Elements
- **City Filter**: Select between Mandalay, Naypyitaw, and Yangon
- **Payment Method Filter**: Filter by Cash, Credit Card, and E-wallet
- **Cross-filtering**: Click on any visual to filter related charts
- **Clear All Slicers**: Reset all filters to view complete dataset

## 🔍 Key Insights

### Product Performance by Gender
- **Food and Beverages**: Strong female preference (Female: 33K, Male: 23K)
- **Health and Beauty**: Male-dominated category (Male: 31K, Female: 19K)
- **Sports and Travel**: Slight female preference (Female: 29K, Male: 27K)
- **Fashion Accessories**: Female preference (Female: 30K, Male: 24K)
- **Home and Lifestyle**: Female preference (Female: 30K, Male: 24K)
- **Electronic Accessories**: Balanced distribution (Female: 27K, Male: 27K)

### Customer Satisfaction
- Consistent ratings across all product categories (around 6.97 average)
- Gender-neutral satisfaction levels
- Stable customer experience across different product lines

### Payment Methods
- **Balanced Distribution**: Even split between Cash, Credit Card, and E-wallet
- **E-wallet**: 12% of gross income
- **Credit Card**: Multiple segments showing 10-13% each
- **Cash**: Consistent usage across customer segments

### Geographic Performance
- **Multi-city Operations**: Presence in Mandalay, Naypyitaw, and Yangon
- **Branch Performance**: Varies by location with specific city preferences
- **Regional Insights**: Different customer behaviors across cities

## 📋 Dataset Features

| Feature | Description |
|---------|-------------|
| Invoice ID | Unique identifier for each transaction |
| Branch | Supermarket branch location |
| City | City where the branch is located |
| Customer Type | Member or Non-member classification |
| Gender | Customer gender |
| Product Line | Product category (Health & Beauty, Sports, etc.) |
| Unit Price | Price per unit of product |
| Quantity | Number of units purchased |
| Tax 5% | Tax amount on transaction |
| Total | Total transaction amount (including tax) |
| Date | Transaction date |
| Time | Transaction time |
| Payment | Payment method (Cash, Credit Card, E-wallet) |
| COGS | Cost of Goods Sold |
| Gross Margin % | Predefined margin percentage |
| Gross Income | Income earned from transaction |
| Rating | Customer satisfaction rating |

## 🔧 Technical Implementation

### Data Preparation
- **Storage Mode**: Import
- **Data Source**: CSV file imported into Power BI
- **Data Cleaning**: Removed duplicates, formatted date/time columns, ensured proper numeric data types

### Data Transformation
- Created calculated columns for time-based analysis (Month, Day, Hour)
- Implemented measures for sales aggregation and profitability analysis

### Key Calculated Measures
```DAX
Total Sales = SUM(Total)
Average Rating = AVERAGE(Rating)
Total Gross Income = SUM('Gross Income')
Gross Income Percentage = [Total Gross Income] / [Total Sales]
```

## 📱 Interactive Features

- **Slicers**: Dynamic filtering by Branch, Product Line, Customer Type, and Date
- **Drill-through**: Detailed views by branch or product line
- **Cross-filtering**: Interactive visualizations for comprehensive analysis
