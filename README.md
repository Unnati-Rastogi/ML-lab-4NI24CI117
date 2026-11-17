# Machine Learning Lab

This repository contains Jupyter notebooks for introductory machine learning exercises. The notebooks cover polynomial and linear regression, regularization, cross-validation, and binary classification.

## Repository contents

| File | Description |
| --- | --- |
| `activity 1.ipynb` | Compares ordinary least squares, Ridge regression, and a manually calculated Lasso-style solution using a small synthetic dataset. Reports training, validation, and test predictions and mean squared errors. |
| `activity 2.ipynb` | Explores the UCI Banknote Authentication dataset, trains a scaled logistic regression classifier, and reviews classification metrics, threshold choices, cross-validation, and a decision tree comparison. Saves diagnostic figures when run. |
| `2 degree polynomial.ipynb` | Fits a quadratic polynomial by constructing the design matrix and solving the normal equations, then reports predictions and metrics and plots the fit. |
| `3 degree polynomial.ipynb` | Builds a small in-memory dataset, fits a cubic polynomial with scikit-learn, evaluates it, and plots the fitted curve. |
| `kfold.ipynb` | Demonstrates five-fold cross-validation for linear regression and reports fold-level predictions and metrics. |
| `linear-regression.ipynb` | Fits a linear regression model to study hours and marks, evaluates the fit, plots it, and predicts a mark for 10 study hours. |
| `regularization.ipynb` | Compares OLS, Ridge, and a manually calculated Lasso-style solution on a synthetic dataset, including split-level predictions and mean squared errors. |

## Requirements

Use Python 3 with Jupyter Notebook or JupyterLab. The notebooks use NumPy, pandas, Matplotlib, and scikit-learn. Install the libraries with:

```bash
python -m pip install numpy pandas matplotlib scikit-learn jupyter
```

## Data files

Three notebooks read datasets from the current working directory. These data files are not included in this repository, so provide them before running the corresponding notebook:

- `2 degree polynomial.ipynb` expects `Degree 2 Polynomial.csv` with `X` and `Y` columns.
- `kfold.ipynb` expects `k_fold_linear_regression (2).csv` with `Hours_Studied` and `Marks` columns.
- `linear-regression.ipynb` expects `linear_regression.csv` with `Hours_Studied` and `Marks` columns.
- `activity 2.ipynb` expects the headerless `data_banknote_authentication.txt` dataset in the UCI Banknote Authentication format: four feature columns followed by the class label. The notebook assigns the feature and label column names when loading it.

`activity 1.ipynb`, `regularization.ipynb`, and `3 degree polynomial.ipynb` create their example data within the notebook and do not require external data files.

## Run a notebook

1. Clone or download this repository.
2. Install the requirements above.
3. Place any required dataset files beside the notebooks.
4. Start Jupyter from the repository directory and open the notebook you want to run.

The notebooks are independent exercises and can be run separately. Some include saved cell outputs from earlier runs; output figures from `activity 2.ipynb` are generated when that notebook is executed.
