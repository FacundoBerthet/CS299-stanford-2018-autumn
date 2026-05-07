# CS229 — Machine Learning (Stanford, Autumn 2018)

Python implementations following the CS229 course by Stanford University.
Each algorithm is implemented from scratch with numpy, then replicated with scikit-learn.

- [Lecture videos (YouTube)](https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU)

## Datasets

**ZonaProp CABA** — 32,585 properties scraped and cleaned. Used for regression (predict property prices).

**E-commerce customers** — 8,000 customers with purchase history and engagement metrics ([Kaggle](https://www.kaggle.com/datasets/meruvakodandasuraj/e-commerce-customer-behavior-and-sales-20202026)). Used for classification (predict churn).

## Structure

```
models/
  data/
    zonaprop_clean.csv              # ZonaProp CABA dataset
    customers.csv                   # E-commerce customer dataset
  01_linear_regression.ipynb
  02_linear_regression_scikit.ipynb
  03_logistic_regression.ipynb
  04_logistic_regression_scikit.ipynb
  utils.py
```

## Models

**`01_linear_regression.ipynb`**
Linear regression from scratch, three ways:
- Normal Equations — closed-form solution
- Batch Gradient Descent
- Stochastic Gradient Descent

Includes univariate (metros → price) and multivariate regression (metros, rooms, bathrooms → price).

**`02_linear_regression_scikit.ipynb`**
Replicates the same models using scikit-learn (`LinearRegression`, `SGDRegressor`).
Results are directly comparable to the from-scratch notebook.

**`03_logistic_regression.ipynb`**
Logistic regression from scratch: sigmoid, binary cross-entropy loss, gradient descent.
Applied to customer churn prediction on the e-commerce dataset.

**`04_logistic_regression_scikit.ipynb`**
Replicates the same model using scikit-learn (`LogisticRegression`).
Includes coefficient plot and direct comparison with the from-scratch results.
