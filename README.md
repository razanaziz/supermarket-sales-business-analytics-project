# supermarket-sales-business-analytics-project
Supermarket Sales Optimization Using Business Analytics
Project Overview

This project analyzes supermarket sales performance using business analytics and machine learning techniques to identify key revenue drivers, improve customer segmentation, optimize inventory planning, and forecast future sales trends.

The objective was to provide actionable business recommendations that support better decision-making across sales strategy, customer retention, and operational efficiency.

The dataset contains 1,000 supermarket transactions across 3 branches and 3 cities over a 3-month period in 2019.

Business Problem

A supermarket chain needed to understand:

What factors drive total sales?
Which branches and product categories perform best?
How can customer segments be better targeted?
How can future sales be forecasted more accurately?
What strategies can improve profitability and customer retention?

This project uses predictive analytics to answer these questions and support data-driven business decisions.

Dataset

Source: Kaggle Supermarket Sales Dataset
https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales

Dataset Includes:

1,000 transaction records
3 branches (A, B, C)
3 cities (Yangon, Mandalay, Naypyitaw)
6 product lines
Customer demographics
Payment methods
Product pricing
Quantity sold
Gross income
Customer ratings
Historical daily sales data

Key Variables

Branch
City
Gender
Customer Type
Product Line
Unit Price
Quantity
Total Sales
Payment Method
Gross Income
Rating
Date and Time

Tools & Technologies Used

Python
AWS S3
Amazon SageMaker
Excel
Machine Learning Models
Time Series Forecasting
Data Visualization
Statistical Analysis

Analytical Methods

Exploratory Data Analysis (EDA)
Descriptive Statistics
Linear Regression
Regression Tree Analysis
K-Nearest Neighbors (KNN)
Customer Segmentation (Clustering)
Time Series Forecasting (ARIMA / SARIMA)
Project Workflow

1. Data Collection & Preprocessing
Imported dataset from Kaggle
Stored data using AWS S3
Processed analysis in Amazon SageMaker
Checked for missing values
Verified data quality and data types
Cleaned and prepared dataset for analysis

2. Exploratory Data Analysis

Analyzed:

Sales performance by branch
Product line profitability
Customer type distribution
Gender-based purchasing behavior
Revenue contribution by product category
Correlation between numerical variables

3. Predictive Modeling

Built multiple models to predict total sales:

Linear Regression

Used:

Unit Price
Quantity

To predict:

Total Sales

Result:

R² = 0.90

Key finding:
Quantity sold had a significantly stronger impact on total sales than unit price.

Regression Tree Analysis

Compared model performance against linear regression.

Result:

R² = 0.99
Lower RMSE than linear regression

Conclusion:
Regression tree provided a better fit for the dataset.

K-Nearest Neighbors (KNN)

Tested multiple values of K:

K = 3
K = 5
K = 7

Best Result:

K = 3 / K = 5
R² = 0.99

Conclusion:

KNN confirmed strong predictive relationships between quantity, unit price, and total sales.

Customer Segmentation (Clustering)

Used clustering to identify customer groups based on:

Unit Price
Quantity
Gender
Customer Type
Branch

Optimal Clusters:

K = 3–4

This helped identify different customer purchasing patterns across branches.

Time Series Forecasting

Used:

ARIMA
SARIMA

To forecast:

Future daily total sales

Result:

SARIMA captured seasonality better and provided stronger long-term forecasting value.

Forecast showed continued upward sales growth.

Key Insights

Sales Performance
Branch C generated the highest revenue despite having the fewest transactions
Food & Beverages was the most profitable product category
Fashion Accessories and Food & Beverage had the highest transaction volume

Revenue Drivers
Quantity sold had the strongest positive impact on total sales
Unit price had a smaller but positive effect on revenue

This suggests increasing basket size is more effective than relying on price increases.

Customer Behavior
Member and non-member transactions were almost evenly split
Female customers accounted for slightly more transactions
Distinct customer groups were identified across branches using clustering

Sales Forecasting
Future sales showed an upward trend
Sales patterns showed clear seasonality and stable demand behavior

This supports stronger inventory planning and promotional timing.

Business Recommendations
1. Increase Bulk-Buy Promotions

Since quantity sold had the strongest impact on revenue:

Recommended actions:

Buy One Get One Free offers
Bundle promotions
Loyalty rewards for high-volume purchases
2. Strengthen Membership Conversion

Normal customers contributed strongly to revenue.

Recommended actions:

Improve loyalty membership campaigns
Offer personalized member discounts
Promote exclusive member benefits

3. Optimize Branch-Level Inventory

Branch C performed strongly with fewer transactions.

Recommended actions:

Improve stock allocation by branch
Match inventory to local purchasing behavior
Reduce overstock and understock risks

4. Improve Product-Level Promotions

Focus marketing efforts on:

Food & Beverages
Sports & Travel
High-performing product lines

This supports stronger ROI on promotions.

5. Use Forecasting for Operational Planning

Use SARIMA forecasting to:

Improve inventory planning
Support staffing decisions
Prepare for demand fluctuations
Project Visuals
Included Visuals
Sales by Branch Dashboard
Product Line Profitability Analysis
Linear Regression Results
Customer Clustering Profiles
Sales Forecasting Dashboard

(Visual files available in the /visuals folder)

Repository Structure
supermarket-sales-business-analytics-project/

├── README.md
├── data/
├── visuals/
├── report/
├── code/
└── presentation/
Final Conclusion

This project demonstrates how business analytics can transform raw sales data into strategic business decisions.

By combining predictive modeling, customer segmentation, and time series forecasting, the supermarket can improve profitability, strengthen customer retention, and optimize operations using data-driven decision-making.

The project highlights the practical value of analytics in solving real business problems and supporting long-term business growth.

Author

Business Analytics Graduate
Focused on Data Analytics, Business Intelligence, and Decision-Making through Data

Skills:

SQL
Power BI
Python
Excel
Tableau
Machine Learning
Forecasting
Dashboard Development
Business Strategy
