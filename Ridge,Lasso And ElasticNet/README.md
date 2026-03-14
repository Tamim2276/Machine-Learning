# Algerian Forest Fires Analysis and Prediction

This project analyzes the Algerian Forest Fires dataset to predict the occurrence of fires based on meteorological data. The analysis includes data cleaning, exploratory data analysis (EDA), and feature engineering. The final goal is to build a regression model to predict the Fire Weather Index (FWI).

## Dataset

The dataset used in this project is `Algerian_forest_fires_dataset_UPDATE.csv`. It contains meteorological data for two regions in Algeria: Bejaia and Sidi-Bel Abbes.

## Notebook

The Jupyter notebook `RidgeLassoAndElasticNet.ipynb` contains the complete analysis. The notebook is structured as follows:

1.  **Data Loading and Initial Exploration:** Loading the dataset and getting a first overview.
2.  **Data Cleaning:** Handling missing values, correcting data types, and cleaning column names.
3.  **Exploratory Data Analysis (EDA):** Visualizing the data to find patterns and correlations. This includes histograms, pie charts, correlation heatmaps, and box plots.
4.  **Feature Engineering:** Creating new features and preparing the data for modeling.
5.  **Model Training:** (This part is not yet implemented in the notebook but is the intended next step) Training Ridge, Lasso, and ElasticNet regression models to predict FWI.

## How to Run

1.  Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
2.  Open and run the `RidgeLassoAndElasticNet.ipynb` notebook in a Jupyter environment.
