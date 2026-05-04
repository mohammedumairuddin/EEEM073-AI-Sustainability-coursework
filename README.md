# EEEM073-AI-Sustainability-coursework
# Crop Yield Prediction — EEEM073 AI and Sustainability

## Introduction
Machine learning workflow to predict the crop yield from Indian agricultural
statistics dataset, alongside model compression for sustainable use.

## Prerequisites
To install all required modules execute command:
    pip install pandas numpy scikit-learn matplotlib seaborn shap joblib
    
Minimum Python version: 3.8

## Datasets
Make sure that `crop_production.csv` is present in the same directory as notebooks.
Dataset source: Indian Crop Production Statistics (Kaggle)

## Running Instructions – Notebooks sequence execution:
1. data_loading_preprocessing.ipynb
   → Loads raw CSV, creates Yield variable, pre-processes and encodes dataset 
   → Saves: processed_dataset.csv

2. exploratory_analysis.ipynb
   → Produces all figures for exploratory analysis (Figures 1-8 report)
   → Saves: PNG images to results/plots/

3. model_training_evaluation.ipynb
   → Train Linear Regression and Random Forest
   → Perform hyper-parameter search for models using GridSearchCV
   → Produce SHAP summary plots and model evaluation plots
   → Saves: rf_model.pkl, best_model.pkl to models/

4. model_compression.ipynb
   → Perform feature selection + model pruning model compression
   → Evaluates all model versions and makes a comparison by metrics
   → Saves: model_comparison_results.csv to results/metrics/

## Hardware Requirements
No GPU required. Experiments are performed using only CPU resources.
Expec
