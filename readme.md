# California Housing Regression Analysis

## Overview
This project delivers a customized regression pipeline for the California housing dataset, uniquely combining per-capita feature engineering (rooms and bedrooms normalized by population), ocean-proximity encoding, and thorough distribution diagnostics. By blending novel ratio features with standard predictors and assessing skewness/kurtosis, I built models that explain ~60% of block-level home value variance—while flagging collinearity and non-normality for future improvements.

## Features
Data Cleaning & Standardization,  Analysis, Single-Predictor Regression, Multiple Regression Model, Collinearity Assessment, and Distribution Diagnostics.

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
