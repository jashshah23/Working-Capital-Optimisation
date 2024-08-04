# Working Capital Optimization Project

## Overview

This project aims to optimize working capital by leveraging historical financial and operational data to develop predictive models that forecast key metrics such as Days Sales Outstanding (DSO), Days Payables Outstanding (DPO), Inventory Turnover, and Cash Flow. The project involves data integration, cleaning, transformation, predictive modeling, and visualization.

### Table of Contents

-Project Structure

-Setup Instructions

-Data Sources

-Data Processing

-Predictive Modeling

-Visualization

# Project Structure

├── data

    ├── sales_dummy_data.csv

    ├── inventory_dummy_data.csv

    ├── accounts_receivable_dummy_data.csv
 
    ├── cash_flow_dummy_data.csv

    ├── accounts_payable_dummy_data.csv

    ├── aggregated_data.csv

├── notebooks

    ├── WCO analysis.ipynb

    ├── predictive_modeling.ipynb

   ├── visualization.ipynb

├── README.md

├── requirements.txt


## Setup Instructions

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/working-capital-optimization.git
    cd working-capital-optimization
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up the database:**
    - Create the necessary tables by running the SQL scripts provided in the `scripts` directory.
    - Load the dummy data from the `data` directory into the respective tables.

## Data Sources

- **Sales Data**: Contains information on sales transactions including sale amount, quantity sold, and customer details.
- **Inventory Data**: Contains inventory details such as item names, categories, and quantities.
- **Accounts Receivable Data**: Contains details on receivables including invoice dates, amounts, and payment statuses.
- **Cash Flow Data**: Contains cash flow transaction details.
- **Accounts Payable Data**: Contains details on payables including invoice dates, amounts, and payment statuses.

## Data Processing

Data processing involves cleaning, transforming, and merging the datasets to create a comprehensive aggregated dataset. This step includes:
- Removing duplicates and handling missing values.
- Calculating additional metrics such as `DaysToCollect` and `DaysToPay`.
- Merging datasets using common keys like `CustomerID` and `SaleID`.

## Predictive Modeling

Predictive models are developed to forecast key metrics using regression techniques. The modeling process includes:
- Splitting data into training and testing sets.
- Training models such as Linear Regression and Random Forest.
- Evaluating models using metrics like Mean Absolute Error (MAE) and R-squared (R²).

## Visualization

Interactive dashboards and visualizations are created using Looker Studio to present key metrics and insights. Visualizations include:
- Bar charts and line charts for DSO, DPO, Inventory Turnover, and Cash Flow trends.
- Heatmaps for identifying patterns and outliers.

---


Feel free to contact the project maintainer at jash.letsconnect@gmail.com for any questions or further information.
