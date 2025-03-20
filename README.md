# Iris Flower Classification

## Project Overview
This project implements a machine learning model to classify Iris flowers into three species based on their sepal and petal measurements. The classification is done using a Random Forest Classifier, which achieves high accuracy in species identification.

## Objectives
- Develop a classification model to identify Iris flowers into three species
- Identify the most significant features influencing flower species classification
- Evaluate model performance using appropriate metrics

## Dataset
The Iris dataset is a classic dataset in machine learning and contains measurements for 150 iris flowers from three species:
- Setosa
- Versicolor
- Virginica

Each flower has four features measured:
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

## Implementation Details

### Data Preprocessing
- Extracted dataset from ZIP file
- Removed unnecessary spaces in column names
- Encoded categorical target variable (species) using LabelEncoder
- Standardized features using StandardScaler
- Split data into training (80%) and testing (20%) sets

### Model Training
- Implemented Random Forest Classifier with 100 estimators
- Trained model on the preprocessed dataset

### Model Evaluation
- Calculated accuracy score (>95% achieved)
- Generated detailed classification report with precision, recall, and F1-score
- Created confusion matrix to visualize classification performance

### Feature Importance Analysis
Identified the most significant features for classifying Iris flowers:
1. Petal measurements (length and width) are most influential
2. Sepal measurements contribute less to the classification

### Visualizations
The notebook includes several visualizations:
- Pairplots showing relationships between features for different species
- Boxplots identifying potential outliers in the dataset
- Feature importance bar chart displaying the relative importance of each feature
- Confusion matrix heatmap showing classification performance

## How to View This Project
This repository contains a Jupyter notebook with all code, visualizations, and results. You can:

1. View the notebook directly on GitHub to see all code and outputs
2. Download and run the notebook locally:

   ```
   git clone https://github.com/passionateaman/iris-classification-project.git
   cd iris-classification-project
   jupyter notebook iris_classification.ipynb
   ```

## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- joblib

## Conclusions
The Random Forest Classifier successfully classifies Iris flowers with high accuracy. The analysis confirms that petal dimensions are more significant than sepal dimensions for species identification, which aligns with botanical knowledge of Iris flowers.