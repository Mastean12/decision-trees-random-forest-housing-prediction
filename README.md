# Decision Trees and Random Forest Housing Price Prediction

## Project Overview

This project explores tree-based machine learning algorithms for predicting housing prices using the California Housing Dataset from Scikit-Learn.

The objective is to understand how Decision Trees and Random Forests improve prediction performance compared to traditional regression models while providing insights into feature importance and model interpretability.

---

## Problem Statement

Accurately predicting housing prices is an important problem in real estate, finance, and urban planning.

This project investigates:

- How Decision Trees learn decision rules from data.
- How Random Forests improve predictive performance through ensemble learning.
- Which housing features have the greatest influence on house prices.

---

## Dataset

The project uses the California Housing Dataset provided by Scikit-Learn.

### Features

| Feature | Description |
|----------|------------|
| MedInc | Median Income |
| HouseAge | Median House Age |
| AveRooms | Average Rooms |
| AveBedrms | Average Bedrooms |
| Population | Population |
| AveOccup | Average Occupancy |
| Latitude | Latitude |
| Longitude | Longitude |

### Target Variable

**Price** – Median House Value

---

## Project Workflow

### 1. Data Loading

- Loaded California Housing Dataset
- Converted data into a Pandas DataFrame

### 2. Exploratory Data Analysis

- Dataset inspection
- Statistical summaries
- Missing value analysis
- Correlation analysis

### 3. Feature Understanding

- Correlation heatmap
- Feature relationship analysis
- Identification of influential variables

### 4. Data Splitting

- 80% Training Data
- 20% Testing Data

### 5. Decision Tree Regression

Implemented:

```python
DecisionTreeRegressor()
```

Evaluated using:

- MAE
- RMSE
- R² Score

Visualized the learned decision tree structure.

### 6. Random Forest Regression

Implemented:

```python
RandomForestRegressor()
```

Evaluated using:

- MAE
- RMSE
- R² Score

### 7. Feature Importance Analysis

Used Random Forest feature importance scores to identify the most influential variables driving housing prices.

---

## Results

### Decision Tree Regressor

| Metric | Score |
|----------|----------|
| MAE | 0.4547 |
| RMSE | 0.7037 |
| R² | 0.6221 |

### Random Forest Regressor

| Metric | Score |
|----------|----------|
| MAE | 0.3275 |
| RMSE | 0.5053 |
| R² | 0.8051 |

---

## Feature Importance Ranking

| Feature | Importance |
|----------|----------|
| MedInc | 0.5249 |
| AveOccup | 0.1384 |
| Latitude | 0.0889 |
| Longitude | 0.0886 |
| HouseAge | 0.0546 |
| AveRooms | 0.0443 |
| Population | 0.0307 |
| AveBedrms | 0.0296 |

### Key Insight

Median Income (MedInc) was identified as the most influential predictor of housing prices, accounting for more than 50% of the model's predictive importance.

---

## Key Findings

- Random Forest significantly outperformed Decision Tree Regression.
- Ensemble learning improved prediction accuracy.
- Median Income was the strongest predictor of housing prices.
- Tree-based models captured non-linear relationships that traditional regression models may miss.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## Machine Learning Concepts Demonstrated

- Supervised Learning
- Regression
- Decision Trees
- Random Forests
- Ensemble Learning
- Feature Importance Analysis
- Model Evaluation
- Train-Test Split
- Exploratory Data Analysis

---

## Future Improvements

Potential enhancements include:

- Hyperparameter tuning using GridSearchCV
- Gradient Boosting Models
- XGBoost
- LightGBM
- Cross-validation optimization
- Advanced feature engineering

---

## Author

Stephen

AI Engineering & Machine Learning Portfolio Project

Focused on Machine Learning, AI Systems Development, Data Science, and Applied Artificial Intelligence.
