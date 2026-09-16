# Linear Regression From Scratch

This project implements Linear Regression from scratch using NumPy and compares the results with the Linear Regression implementation provided by Scikit-learn.

## 📌 Project Overview

The main goal of this project is to understand how Linear Regression works internally instead of directly relying on a machine learning library.

The implementation includes:

- Linear Regression from scratch
- Multiple Linear Regression
- Model training using the pseudoinverse
- Prediction using learned coefficients
- Comparison with Scikit-learn
- R² score comparison
- Comparison of coefficients and intercept

## 📊 Dataset

The project uses the **Diabetes dataset** available through Scikit-learn.

Dataset shape:

- Features: 442 samples × 10 features
- Target: 442 values

The dataset is divided into training and testing sets using an 80/20 split.

## 🧮 Linear Regression From Scratch

The custom model is implemented using NumPy.

The model calculates the parameters using the pseudoinverse:

β = X⁺y

where:

- `X` = feature matrix
- `X⁺` = pseudoinverse of X
- `y` = target values
- `β` = model parameters

The first parameter represents the intercept and the remaining parameters represent the coefficients.

## 🛠️ Technologies Used

- Python
- NumPy
- Scikit-learn
- Jupyter Notebook

## 📈 Model Evaluation

The custom implementation is compared with Scikit-learn's `LinearRegression`.

The models are evaluated using the **R² (R-squared) score**.

### Results

| Model | R² Score |
|-------|----------|
| Scikit-learn Linear Regression | 0.4399 |
| Custom Linear Regression | 0.4399 |

The project also compares the learned intercept and coefficients between the two implementations.

## 📁 Project Structure

```text
linear-regression-from-scratch/
│
├── regrresion.ipynb
└── README.md
