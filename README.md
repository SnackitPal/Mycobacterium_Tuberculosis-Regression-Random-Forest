# Mycobacterium_Tuberculosis-Regression-Random-Forest
This project focuses on predicting the bioactivity of Mycobacterium tuberculosis compounds using a Random Forest Regression model. 

## Project Overview
This project focuses on predicting the bioactivity of Mycobacterium tuberculosis compounds using a Random Forest Regression model. The dataset used contains molecular descriptors and the corresponding pIC50 values. The primary objective of this project is to train a Random Forest model to predict pIC50 values and visualize the results in a scatter plot, comparing the predicted values to the experimental ones.

## Dataset
The dataset used in this project is based on molecular fingerprints and bioactivity data for Mycobacterium tuberculosis. Specifically, it contains:

- Features: Molecular descriptors/fingerprints generated from compound structures.
- Target Variable: Experimental pIC50 values (bioactivity).

The dataset is stored as:
- mycobacterium_tuberculosis_bioactivity_data_3class_pIC50_pubchem_fp.csv

## Code Explanation
## Steps:
- Data Loading:
The dataset is loaded using pandas and split into features (X) and target (Y).
- Feature Selection:
A VarianceThreshold is applied to remove low-variance features, reducing the dataset's dimensionality.
- Data Splitting:
The dataset is split into training and test sets using an 80-20 split.
- Random Forest Model:
A Random Forest Regressor model with 100 estimators is trained on the training data.
The model’s performance is evaluated on the test data using R-squared (R²).
- Predictions:
The model predicts the pIC50 values for the test data.
- Visualization:
A scatter plot is created using seaborn's regplot to compare the predicted and experimental pIC50 values. This visual representation gives an indication of how well the model's predictions align with the true values.

## Results
The plot below shows the correlation between the predicted and experimental pIC50 values. Ideally, the points should be aligned along the diagonal line, indicating a strong predictive power of the model.

![image](https://github.com/user-attachments/assets/ed701b63-ba65-42c4-b5eb-742f9ffe25fd)
