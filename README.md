# Boston-House-Price-Prediction
This project focuses on predicting the median value of owner-occupied homes (`MEDV`) in the Boston area using various features such as crime rate, number of rooms, and accessibility to highways. The solution involves data preprocessing, exploratory data analysis (EDA), feature engineering, and model building using regression algorithms.

---

## Dataset

The dataset contains features including:
- `CRIM`: Per capita crime rate by town
- `ZN`: Proportion of residential land zoned for large lots
- `INDUS`: Proportion of non-retail business acres
- `CHAS`: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- `NOX`: Nitric oxides concentration (ppm)
- `RM`: Average number of rooms per dwelling
- `AGE`: Proportion of owner-occupied units built before 1940
- `DIS`: Weighted distances to five Boston employment centers
- `RAD`: Index of accessibility to radial highways
- `TAX`: Full-value property tax rate
- `PTRATIO`: Pupil-teacher ratio
- `B`: 1000(Bk - 0.63)^2 where Bk is the proportion of Black residents
- `LSTAT`: % lower status of the population
- `MEDV`: Median value of owner-occupied homes (Target)

---

## Problem Statement

Build a regression model to accurately predict `MEDV` based on the other features in the dataset.

---

## 🔧 Tech Stack

- **Pandas**, **NumPy** – Data manipulation
- **Seaborn**, **Matplotlib** – Data visualization
- **Scikit-learn** – Machine Learning models
- Jupyter Notebook / Python 3.x

---

## Project Workflow

1. **Data Preprocessing**
   - Handling missing and malformed data
   - Converting string entries to numeric where needed

2. **Exploratory Data Analysis (EDA)**
   - Heatmap of feature correlations
   - Distribution plots and outlier detection

3. **Modeling**
   - Train/Test split
   - Multiple Regression Models tested:
     - Linear Regression
     - Ridge/Lasso Regression
     - Decision Tree / Random Forest Regressor

4. **Evaluation**
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - R² Score

---

## Results

- Best performing model: `Random Forest Regressor`
- R² Score: ~0.87 (depending on parameters)
- Feature importance analysis showed `LSTAT` and `RM` as most predictive

---

## How to Run

```bash
git clone https://github.com/Manviya-Sahni/Boston-House-Price-Prediction.git
cd Boston-House-Price-Prediction
pip install -r requirements.txt
jupyter notebook  # or open the .ipynb file in VS Code
