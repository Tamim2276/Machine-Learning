# Algerian Forest Fires Analysis and Prediction

This project analyzes the Algerian Forest Fires dataset to predict the occurrence of fires based on meteorological data. The analysis includes data cleaning, exploratory data analysis (EDA), and feature engineering. The final goal is to build a regression model to predict the Fire Weather Index (FWI).

## Dataset

The dataset used in this project is `Algerian_forest_fires_dataset_UPDATE.csv`. It contains meteorological data for two regions in Algeria: Bejaia and Sidi-Bel Abbes.

## Notebook

The Jupyter notebook `RidgeLassoAndElasticNet.ipynb` contains the complete analysis. The notebook is structured as follows:

1.  **Import Libraries:** Loading necessary Python libraries including pandas, numpy, matplotlib, and seaborn.
2.  **Data Loading and Initial Exploration:** Loading the dataset and getting a first overview of the structure and content.
3.  **Data Cleaning:**
    - Handling missing values and removing invalid rows
    - Adding a 'Region' column to distinguish between Bejaia (0) and Sidi-Bel Abbes (1)
    - Correcting data types and cleaning column names
    - Converting string columns to appropriate numeric types
4.  **Exploratory Data Analysis (EDA):**
    - **Distribution Analysis:** Histograms showing the distribution of all features
    - **Class Balance:** Pie chart displaying the proportion of fire vs. not fire instances
    - **Correlation Analysis:** Heatmap revealing relationships between features, with FWI showing high correlation (0.77) with FFMC
    - **Box Plot Analysis:** Visualizing FWI distribution and identifying outliers
    - **Temporal Analysis:** Monthly fire occurrence patterns by region, showing August and September as peak fire months
5.  **Feature Engineering and Model Preparation:** Creating new features and preparing the data for modeling.
6.  **Model Training:** (This part is not yet implemented in the notebook but is the intended next step) Training Ridge, Lasso, and ElasticNet regression models to predict FWI.

## Key Findings

- **High Correlation Features:** FFMC (0.77), ISI (0.74), and FWI (0.72) show the strongest correlation with fire occurrence
- **Seasonal Pattern:** August and September show the highest fire frequency in both regions
- **Temperature Impact:** Temperature shows moderate positive correlation (0.52) with fire occurrence
- **Humidity Effect:** Relative Humidity (RH) has negative correlation (-0.43) with fires

## Visualizations

The notebook includes several informative visualizations:

- **Density Plots:** Distribution histograms for all numerical features
- **Pie Chart:** Class distribution showing fire (56.4%) vs. not fire (43.6%) instances
- **Correlation Heatmap:** Complete correlation matrix with annotations showing feature relationships
- **Box Plot:** FWI distribution with optimized tick spacing to prevent label overlap
- **Bar Charts:** Monthly fire analysis for both Bejaia and Sidi-Bel Abbes regions

## How to Run

1.  Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
2.  Open and run the `RidgeLassoAndElasticNet.ipynb` notebook in a Jupyter environment.

## Dataset Features

- **Meteorological Variables:** Temperature, RH (Relative Humidity), Ws (Wind speed), Rain
- **Fire Weather Indices:** FFMC (Fine Fuel Moisture Code), DMC (Duff Moisture Code), DC (Drought Code), ISI (Initial Spread Index), BUI (Build Up Index), FWI (Fire Weather Index)
- **Target Variable:** Classes (fire/not fire)
- **Additional:** Region identifier for spatial analysis
