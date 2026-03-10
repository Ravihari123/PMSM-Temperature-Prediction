# PMSM-Temperature-Prediction

This repository contains the code and report for predicting temperatures in Permanent Magnet Synchronous Motors (PMSMs) using machine learning and deep learning models. The project focuses on data-driven approaches to estimate motor temperatures, addressing challenges in traditional thermal monitoring methods.

## Overview

PMSMs are widely used in electric vehicles due to their efficiency and torque capabilities. However, accurate temperature monitoring is crucial to prevent failures. This study implements and evaluates models to predict four key temperatures (permanent magnet surface, stator yoke, stator tooth, and stator winding) based on inputs like motor speed, ambient temperature, torque, currents (d/q-axis), voltages (d/q-axis), and coolant temperature.

The models include:
- Ordinary Least Squares (OLS)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Convolutional Neural Network (CNN)

Key findings: CNN achieved the lowest MSE (0.0264), while Random Forest had the highest R² (0.9999) on test data.

Dataset: Sourced from [Kaggle](https://www.kaggle.com/datasets/wkirgsn/electric-motor-temperature) (1.3M records, 13 features).

## Requirements

- Python 3.x
- Libraries: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras

- 
## Usage

Run the notebooks:
- `DL_project_Group2_EDA_and_oldModels.ipynb`: Exploratory Data Analysis (EDA) and initial models.
- `DL_project_Group2_MLModels_final.ipynb`: Machine Learning models (OLS, KNN, Decision Tree, Random Forest).
- `DL_project_Group2_DLModels_final.ipynb`: Deep Learning model (CNN).


## Results

- Evaluated using R², MSE, and MAE.
- Best performers: CNN (min MSE) and Random Forest (max R²).
- Detailed results and visualizations in the notebooks and report.

## Files

- `Group2_Report_final submitted.pdf`: Full project report with methodology, literature review, and results.
- `DL_project_Group2_DLModels_final.ipynb`: Deep learning implementation.
- `DL_project_Group2_MLModels_final.ipynb`: Machine learning implementation.
- `DL_project_Group2_EDA_and_oldModels.ipynb`: EDA and preliminary models.
