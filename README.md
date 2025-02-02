# Retail Price Optimization using Machine Learning

## Overview
Pricing a product is a crucial aspect of any business. Various strategies are used to estimate prices based on product demand and sensitivity to price changes. Some products have highly elastic demand, meaning a small price change can significantly impact sales, while others (luxury items or necessities) exhibit inelastic demand.

Price elasticity of demand (EPD) quantifies how demand changes concerning price fluctuations. Understanding this concept allows businesses to optimize pricing strategies, improving profitability while maintaining customer satisfaction.

This project focuses on optimizing prices for a cafe's menu items using machine learning techniques. By analyzing past sales data stored in a PostgreSQL database hosted on Amazon RDS, we calculate price elasticity and determine optimal pricing. The methods and concepts discussed here can be extended to other industries for price optimization.

---

## Aim
To determine optimal prices for cafe menu items using machine learning-based price optimization techniques.

---

## Data Description
The dataset consists of three CSV files:

1. **Cafe - Sell MetaData.csv**: Contains details of sales transactions.
   - Columns: Sell ID, Sell Category, Item ID, Item Name

2. **Cafe - Transaction - Store.csv**: Contains transaction and sales receipt data.
   - Columns: Calendar Date, Price, Quantity, Sell ID, Sell Category

3. **Cafe - DateInfo.csv**: Contains date-related information.
   - Columns: Date, Year, Holiday, Weekend, School Break, Temperature, Outdoor

Additionally, the project includes data fetching from a PostgreSQL database using the `psycopg2` library.

---

## Tech Stack
- **Language:** Python
- **Libraries:** pandas, numpy, scipy, matplotlib, seaborn, sklearn, statsmodels, psycopg2
- **Database:** PostgreSQL (Amazon RDS)

---

## Approach
### 1. Price Optimization Algorithms
- Understanding customer behavior through sales data
- Estimating cost of food items using historical sales data
- Exploring pricing methods:
  - Cost-less pricing
  - Competition-based pricing
  - Perceived value pricing
  - Demand-based pricing
- Introduction to price elasticity and its role in price optimization

### 2. Exploratory Data Analysis (EDA)
- Handling missing values and redundant data
- Merging datasets using pandas
- Visualizing trends using matplotlib and seaborn
- Preparing data for machine learning models

### 3. Machine Learning Algorithms
- Regression trees and ordinary least squares (OLS) method for price estimation
- Evaluating model accuracy using statistical metrics (R-squared, etc.)
- Feature selection and elimination to improve model performance
- Maximizing profits using price elasticity calculations

---

## Application of Machine Learning in Pricing Optimization
This project primarily focuses on optimizing prices for a burger cafe. However, its applications extend across various industries like healthcare, hospitality, and insurance. For example, hotel analysts can use similar techniques to adjust service prices based on guest feedback and past bookings.

---

## Results & Discussion
The model evaluates price elasticity and suggests optimal pricing strategies. It compares different pricing models and their effectiveness in maximizing revenue.

---

## Contributing
Contributions are welcome! Feel free to submit pull requests or open issues to improve this project.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
