# California Housing Regression Analysis

## Overview
This project analyzes the California housing dataset to predict median house values at the block level. I standardized room- and bedroom-count predictors, engineered per-capita features, and built both simple and multiple linear regression models—culminating in a full model that explains ~60% of value variance.

## Features
- **Data Cleaning & Standardization:**  
  - Handled missing values and scaled “rooms” and “bedrooms” by population for comparability.  
- **Exploratory Analysis:**  
  - Correlation matrices and scatter plots to assess predictor usefulness and detect collinearity.  
- **Single-Predictor Regression:**  
  - Identified **median_income** as most predictive (R² ≈ 0.46) and **ocean_proximity** as least predictive.  
- **Multiple Regression Model:**  
  - Combined all seven predictors to achieve R² ≈ 0.60, demonstrating improved explanatory power.  
- **Collinearity Assessment:**  
  - Found moderate multicollinearity between rooms & bedrooms and between population & households.  
- **Distribution Diagnostics (Extra Credit):**  
  - Used histograms, skewness, and kurtosis to reveal non-normal predictor and outcome distributions.

## Tech & Tools
- **Language:** Python 3  
- **Analysis & Modeling:** pandas, NumPy, scikit-learn (StandardScaler, LinearRegression)  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  
- **Version Control:** Git & GitHub  

## Results & Key Takeaways
- **Normalization Choice:** Per-capita features (rooms/population, bedrooms/population) produced more uniform distributions than per-household.  
- **Key Predictors:** Median income strongly drives house value; ocean proximity offers minimal linear signal.  
- **Model Performance:** Multiple regression (R²=0.597) outperforms single-predictor model (R²=0.459).  
- **Collinearity Warning:** Rooms vs. bedrooms and population vs. households show moderate correlation, suggesting careful feature selection.  
- **Non-Normal Distributions:** Skewed, heavy-tailed data may violate linear regression assumptions—consider transformations for future work.

## Skills Gained
Feature Engineering, Regression Modeling, Statistical Diagnostics, and Data Visualization.

## Quick Start

```bash
git clone https://github.com/yourusername/california-housing-regression.git
cd california-housing-regression
pip install -r requirements.txt
jupyter lab Homework\ 1.ipynb
