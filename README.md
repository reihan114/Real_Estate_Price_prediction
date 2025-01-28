# Real Estate Price Prediction

This project aims to predict real estate prices in Bangalore, India, using a dataset of property features such as location, size, number of bathrooms, and total square footage. The goal is to build a machine learning model that can accurately predict property prices.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Key Steps](#key-steps)
- [Technologies Used](#technologies-used)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [How to Run the Project](#how-to-run-the-project)
- [Future Improvements](#future-improvements)
  

---

## Overview

This project is an end-to-end machine learning pipeline for predicting housing prices. The dataset contains information on property location, size, number of bathrooms, total area, and the selling price. Using these features, we preprocess the data, train a regression model, and evaluate its performance.

---

## Dataset

The dataset contains the following columns:
- **Location**: The area or neighborhood where the property is located.
- **Size**: Number of bedrooms (e.g., "2 BHK").
- **Total Sqft**: Total area of the property in square feet.
- **Bath**: Number of bathrooms.
- **Price**: Price of the property in lakhs (1 lakh = 100,000 INR).

### Data Source
The dataset is sourced from an open dataset containing Bangalore real estate information.

---

## Key Steps

1. **Data Cleaning**:
   - Removed rows with missing or invalid data.
   - Standardized the `size` and `total_sqft` columns.
2. **Feature Engineering**:
   - Created a `price_per_sqft` column.
   - Grouped rare locations under a single "other" category.
   - Removed outliers based on domain-specific rules.
3. **Exploratory Data Analysis (EDA)**:
   - Visualized price trends and distributions.
   - Analyzed relationships between features and property prices.
4. **Model Building**:
   - Used a **Linear Regression** model for prediction.
5. **Evaluation**:
   - Evaluated the model using metrics like R-squared and Mean Absolute Error (MAE).

---

## Technologies Used

- **Python**: Programming language for data analysis and modeling.
- **Libraries**:
  - `pandas`: For data manipulation.
  - `numpy`: For numerical operations.
  - `matplotlib` and `seaborn`: For data visualization.
  - `scikit-learn`: For machine learning model building and evaluation.

---

## Project Workflow

1. Load the dataset and explore its structure.
2. Clean and preprocess the data:
   - Handle missing values and irregular entries.
   - Standardize columns like `size` and `total_sqft`.
3. Perform exploratory data analysis:
   - Identify trends and outliers.
   - Visualize important relationships.
4. Engineer features and remove outliers.
5. Train a **Linear Regression** model to predict prices.
6. Evaluate the model's performance using:
   - R-squared: Indicates how well the model explains the variance in the data.
   - Mean Absolute Error (MAE): Measures the average error in price prediction.

---

## Results

- **Best Model**: Linear Regression
- **Performance**:
  - R-squared: ~0.8
  - Mean Absolute Error (MAE): ~5 lakhs

Key factors influencing the property price:
1. **Location**: Prime locations significantly increase property value.
2. **Size (Total Sqft)**: Larger properties generally cost more.
3. **Number of Bedrooms and Bathrooms**: Higher configuration properties are priced higher.
4. **Price Per Sqft**: A key determinant of property value.

---

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/reihan114/Real_Estate_Price_prediction.git
   cd Real_Estate_Price_prediction
2. Install the required Python libraries:
   pip install -r requirements.txt
3. Open the Jupyter Notebook:
   jupyter notebook jupyter notebook banglore_home_prices_final.ipynb
4. Run the notebook cells to process the data, train the model and view the results.
## Future Improvements
1. Use advanced machine learning models like Random Forest, Gradient Boosting 
   (XGBoost/LightGBM), or Neural Networks for improved predictions.
2. Incorporate additional features such as Distance to key landmarks



