# Insurance Cost Prediction

## Overview
This project predicts individual medical insurance costs based on demographic and lifestyle factors using regression techniques.  
The goal is not only to build a predictive model, but also to understand which factors most influence insurance charges and where simple models succeed or fail.

This project demonstrates an end-to-end machine learning workflow including data exploration, feature analysis, model training, evaluation, and interpretation.

---

## Problem Statement
Medical insurance costs vary significantly depending on factors such as age, BMI, smoking habits, and region.  
Accurately predicting these costs can help insurance providers with pricing strategies and risk assessment.

This project aims to:
- Predict insurance charges using regression models
- Analyze the impact of key features
- Evaluate model performance and limitations

---

## Dataset
- **Source:** Publicly available insurance dataset
- **Records:** 1,338
- **Features:**
  - `age`: Age of the individual
  - `sex`: Gender
  - `bmi`: Body Mass Index
  - `children`: Number of dependents
  - `smoker`: Smoking status
  - `region`: Residential region
  - `charges`: Medical insurance cost (target variable)

Dataset is stored in:
data/insurance.csv

---

## Project Structure
nsurance-cost-prediction/
├── data/
│ └── insurance.csv
├── notebooks/
│ └── insurance_cost_prediction.ipynb
├── README.md


---

## Methodology
1. **Exploratory Data Analysis (EDA)**
   - Distribution analysis of numerical features
   - Relationship between features and insurance charges
   - Identification of high-impact variables (e.g., smoking status)

2. **Data Preprocessing**
   - Encoding categorical variables
   - Feature selection
   - Train-test split

3. **Modeling**
   - Linear Regression used as a baseline regression model
   - Model trained on processed features to predict insurance costs

4. **Evaluation**
   - Performance evaluated using regression metrics
   - Interpretation of coefficients to understand feature influence

---

## Key Observations
- Smoking status is the strongest predictor of insurance cost
- Age and BMI have a positive correlation with charges
- Linear regression struggles with non-linear cost patterns for smokers, highlighting model limitations

---

## Results
The linear regression model provides a reasonable baseline but shows higher prediction errors for individuals with extreme medical costs.  
This suggests the presence of non-linear relationships that could be better captured by more advanced models.

---

## Future Improvements
- Compare Linear Regression with Ridge, Lasso, or tree-based models
- Perform detailed error analysis for high-cost outliers
- Add feature engineering (e.g., interaction terms, polynomial features)
- Improve model generalization and robustness

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Author
**Sandesh Duduskar**

This project is part of my machine learning portfolio and reflects my interest in applied ML, data-driven decision making, and continuous learning.
