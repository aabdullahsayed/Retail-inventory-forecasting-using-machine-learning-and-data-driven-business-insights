# Retail Store Inventory Forecasting Analysis

## Project Overview
This project focuses on the application of data science and machine learning techniques to optimize retail inventory management. By analyzing historical sales data, pricing strategies, and environmental factors, the project aims to build a robust forecasting model capable of predicting daily `Units Sold`. The ultimate goal is to provide actionable insights that help retailers reduce stockouts and minimize overstocking costs.

## Dataset
The dataset utilized for this analysis is sourced from Kaggle. It contains daily records of store sales, including variables such as price, discounts, weather conditions, and holiday flags.

* **Dataset Name:** Retail Store Inventory Forecasting Dataset
* **Source:** [Kaggle Link](https://www.kaggle.com/datasets/anirudhchauhan/retail-store-inventory-forecasting-dataset)

## Project Workflow
The analysis follows a structured data science lifecycle:

1.  **Data Acquisition & Cleaning:** Handling missing values, converting temporal data types, and removing outliers.
2.  **Exploratory Data Analysis (EDA):** Visualizing weekly sales trends, seasonality, and the impact of promotions.
3.  **Feature Engineering:**
    * Creation of rolling statistics (7-day moving averages and standard deviations).
    * Lag features to capture autoregressive properties.
    * Categorical encoding of weather and holiday data.
4.  **Model Development:** Training and evaluating multiple regression algorithms.
5.  **Business Insights:** extracting feature importance to identify key drivers of sales.

## Technologies Used
* **Language:** Python 3.10+
* **Development Environment:** Google Colab / Jupyter Notebook
* **Libraries:**
    * Data Manipulation: Pandas, NumPy
    * Visualization: Matplotlib, Seaborn
    * Machine Learning: Scikit-Learn

## Model Performance
Four machine learning models were trained and evaluated using Root Mean Squared Error (RMSE) and R-Squared (R2) metrics. The Random Forest Regressor demonstrated the superior performance, effectively capturing non-linear relationships in the data.


## Strategic Insights
The analysis identified the following factors as the primary drivers of sales:
1.  **Demand Forecast:** The baseline forecast provided the strongest signal.
2.  **Pricing & Discounts:** Sales volume showed high elasticity regarding price changes and promotional discounts.
3.  **Seasonality:** Distinct sales spikes were observed during specific holiday periods, necessitating dynamic inventory buffering.

## Usage Instructions
To reproduce the analysis:

1.  Clone this repository to your local machine.
2.  Download the dataset from the link provided above and place `retail_store_inventory.csv` in the root directory.
3.  Open the notebook file in Jupyter or Google Colab.
4.  Run all cells sequentially to execute the data pipeline and model training.
