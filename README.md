
AutoML Pipeline
Automated machine learning pipeline for regression and classification tasks. It performs end-to-end processing, from data cleaning to model evaluation, and provides clear insights into feature importance.
Features
Supports regression and classification tasks automatically
Data preprocessing: handles missing values, duplicates, and outliers
Categorical encoding with LabelEncoder
Feature selection based on correlation thresholds
Train-test split with optional SMOTE oversampling for imbalanced classification
Model training and evaluation: RandomForest, GradientBoost, AdaBoost, GradientBoostingRegressor
Generates plots for feature importance and confusion matrix
Saves evaluation reports in CSV format
Usage
Python
Copy code
from automl_pipeline import AutoMLPipeline  # adjust import based on your file

csv_path = "path/to/your/dataset.csv"
target_col = "target"  # replace with your target column

pipeline = AutoMLPipeline(csv_path, target_col)
pipeline.run()
