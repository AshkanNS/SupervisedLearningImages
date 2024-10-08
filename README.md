
# Bank Customer Churn Prediction

This project focuses on predicting bank customer churn using a dataset containing various customer attributes. The goal is to build a machine learning model that can identify which customers are likely to leave the bank, allowing the bank to take proactive actions to retain them.

## Project Overview

The project analyzes customer data to understand patterns that lead to churn, such as customer demographics, account balances, transaction behavior, and more. Using this data, a predictive model is built to forecast customer churn.

### Dataset

The dataset used for this project includes the following features:

- `customer_id`: Unique identifier for the customer.
- `vintage`: Number of days the customer has been with the bank.
- `age`: Age of the customer.
- `gender`: Gender of the customer.
- `dependents`: Number of dependents the customer has.
- `occupation`: Occupation type (e.g., salaried, self-employed).
- `city`: Customer’s city code.
- `customer_nw_category`: Customer's net worth category.
- `branch_code`: Code of the branch associated with the customer.
- `current_balance`: The customer's current account balance.
- Several transaction-related features including:
  - `current_month_credit`
  - `previous_month_credit`
  - `current_month_debit`
  - `previous_month_debit`
  - `current_month_balance`
  - `previous_month_balance`
- `churn`: The target variable indicating if the customer churned (1) or not (0).
- `last_transaction`: Date of the customer's last transaction.

### Analysis

The analysis includes the following steps:

1. **Data Preprocessing**: Cleaning missing data, handling outliers, and feature engineering.
2. **Exploratory Data Analysis**: Identifying patterns in customer behavior related to churn.
3. **Model Building**: Training machine learning models like Logistic Regression, Decision Trees, and Random Forest to predict churn.
4. **Model Evaluation**: Using accuracy, precision, recall, and other metrics to evaluate model performance.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required libraries: `pandas`, `numpy`, `matplotlib`, `scikit-learn`

### Running the Project

1. Clone the repository.
2. Install the required dependencies.
3. Open the `bankanalysis.ipynb` file in Jupyter Notebook.
4. Run all the cells to see the analysis and model predictions.

## Results

The models help identify customers with a high risk of churn, providing insights into factors like low account balance, high transaction frequency, or long periods of inactivity, which can influence customer churn.
