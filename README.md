# CS229 — Machine Learning (Stanford, Autumn 2018)

Personal notes, problem set solutions and Python implementations
while following the CS229 course by Stanford University.

- [Lecture videos (YouTube)](https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU)
- [Course website](https://cs229.stanford.edu/syllabus-autumn2018.html)

## Datasets

ZonaProp CABA housing dataset — 32,585 properties scraped and cleaned.
Used across the models notebooks to predict property prices.

## Structure

```
models/                             # Models implementations, from scrath and using scikit-learn
  data/
    zonaprop_clean.csv              # ZonaProp CABA dataset
  01_linear_regression.ipynb        
  02_linear_regression_scikit.ipynb 
  utils.py

problem-sets/                       # Problems statements and solutions
  problem-set-0/
    ps0.pdf                         
    ps0-solutions.tex / .pdf        
```

## Models

**`01_linear_regression.ipynb`**
Linear regression implemented from scratch, three ways:
- Normal Equations — closed-form solution
- Batch Gradient Descent
- Stochastic Gradient Descent

Includes univariate (metros → price) and multivariate regression (metros, rooms, bathrooms → price).

**`02_linear_regression_scikit.ipynb`**
Replicates the same models using scikit-learn (`LinearRegression`, `SGDRegressor`).
Results are directly comparable to the from-scratch notebook.
