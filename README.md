# Home Prices: Multiple Linear Regression

## Project Overview
This project demonstrates the end-to-end process of building a Multiple Linear Regression (MLR) model using Python and Scikit-Learn. It takes a raw dataset of housing features (area, bedrooms, and age) and predicts the final unit price. A significant portion of this exercise focuses on essential data cleaning and preprocessing before model training.

## Dataset
* **Source File:** `homeprices-MLR(homeprices).csv`
* **Features Used (X):** `area` (sq ft), `bedrooms` (count), `age` (years)
* **Target Variable (y):** `price`

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas
* **Machine Learning:** Scikit-Learn (`linear_model.LinearRegression`)
* **Visualization:** Matplotlib

## Workflow & Methodology
1. **Data Cleaning & Preprocessing:** * Handled inconsistent formatting (e.g., removing rogue underscores and decimal points from numeric strings).
   * Identified and removed records with missing values (`NaN` in the bedrooms column).
   * Dropped duplicate entries to ensure model accuracy.
2. **Model Training:** Fit a Multiple Linear Regression model using the cleaned features to predict the continuous target variable (Price).
3. **Evaluation & Visualization:** Mapped the predicted line of best fit against the actual data points.
4. **Interactive Prediction:** Built a simple input script within the notebook to allow users to input custom area, bedroom, and age values to generate a live price prediction.

## How to Run

### Option 1: Run in Cloud (Recommended)
You can view and run this notebook instantly in your browser using Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ronanpatrick/home-prices-mlr/blob/main/MULTILINEAR_REGRESSION_homeprices.ipynb)

*(Note: To run the interactive prediction cell, you must run the notebook in Colab. Ensure you upload the CSV dataset to the session storage or update the pandas read path to the raw GitHub URL).*

### Option 2: Run Locally
1. Clone this repository: `git clone https://github.com/ronanpatrick/home-prices-mlr.git`
2. Install the required libraries: `pip install pandas scikit-learn matplotlib`
3. Open the `.ipynb` file in Jupyter Notebook or VS Code and run all cells.
