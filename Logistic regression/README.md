# Logistic Regression tuning with GridSearchCV

This project is a detailed walk-through demonstrating Logistic Regression using `scikit-learn`. It starts with generating synthetic classification data, splitting it, and then applying a baseline logistic regression model. Afterwards, it dives into hyperparameter tuning using `GridSearchCV`.

## Project Structure

- `logisticRegression.ipynb` : The main notebook containing the data generation, training, hyperparameter search, and evaluation logic.

## Key Concepts Covered

- **Data Generation:** Using `make_classification` to build a simple synthetic dataset.
- **Baseline Modeling:** Training a default `LogisticRegression` to establish baseline metrics.
- **Evaluation:** Using accuracy score, confusion matrix, and a classification report to check the general performance of our model against test data.
- **Hyperparameter Tuning:** Searching for optimal combinations of `solver`, `penalty`, and `C` algorithms utilizing a grid mapped to dictionaries (to avoid incompatible parameter pairings). We apply `StratifiedKFold` for solid cross-validation splits.
- **Training Validation vs. Test Score:** Noticing the slight variations between internally-validated training accuracy (`grid.best_score_`) vs the unseen hold-out accuracy.

## Instructions

1. Install requirements (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`).
2. Run `logisticRegression.ipynb` to see the models in action.
