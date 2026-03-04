# Austin Animal Center Analytics – Code Sample

## Overview

This repository contains the modeling components of a data science project designed to support operational planning for animal shelters.

The primary objectives were:

1. Predict animal stay time (regression)
2. Predict outcome type (classification)

The implementation is organized within a structured Jupyter notebook to reflect the full analytical workflow from data preparation to modeling and simulation.


The notebook is organized into clearly defined sections:

1. Data Cleaning & Preprocessing  
2. Feature Engineering  
3. Stay Time Modeling  
4. Outcome Classification  
5. Simulation Framework  
6. Scenario Analysis  

---

## How to Reproduce

1. Clone repository
2. Install dependencies: `pip install -r requirements.txt`
3. Activate notebook: `jupyter notebook`
4. Run notebook from top to bottom

The notebook is fully executable end-to-end. In case the download link for the data does not work, I have uploaded a copy of the cleaned dataset we used, feel free to replace the file path if needed. 

---

## Modeling Approach

### Stay Time Prediction
- Random Forest Regressor
- GridSearchCV for hyperparameter tuning
- MAE and MSE as evaluation metrics
- Stay time capped at 35 days to reduce skew impact

### Outcome Classification
- Random Forest Classifier
- F1-score used as primary evaluation metric
- Comparison with decision tree and gradient boosting

---

## Design Decisions & Trade-offs

- Notebook format retained to preserve analytical workflow transparency
- Tree-based models selected to capture non-linear relationships
- Distribution-based simulation chosen for interpretability
- Outlier capping applied to improve model stability

---

## Attribution

All preprocessing, feature engineering, modeling code in this repository was written by me and Nina Jiang, who wrote the code for predicting outcome types.

The dataset is merged and cleaned from publicly available tables from Austin Animal Center.
