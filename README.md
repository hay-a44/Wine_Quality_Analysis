## 🍷  Wine Quality Data Analysis & Prediction
### Overview

This project analyzes the Portuguese “Vinho Verde” wine quality dataset from the UCI Machine Learning Repository. The goal is to explore how chemical attributes influence wine quality and to build predictive models that classify wine quality levels using Logistic Regression and K-Nearest Neighbors (KNN).

Both red and white wine datasets are combined into a single dataset for comprehensive analysis.

### Data Source

UCI Machine Learning Repository – Wine Quality Dataset
https://archive.ics.uci.edu/ml/datasets/Wine+Quality

### Raw Data Files

White wine:
http://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-white.csv

Red wine:
http://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv

### Tools & Technologies

**Python**

**pandas, numpy**

**matplotlib, seaborn**

**scikit-learn**

**Jupyter Notebook**

### Project Structure
```
Wine-Quality-Data-Analysis/
│
├── data/
│   ├── raw/
│   │   ├── winequality-red.csv
│   │   └── winequality-white.csv
│   └── processed/
│       └── wine_data_all.csv
│
├── notebooks/
│   └── wine_quality_analysis.ipynb
│
├── outputs/
│   ├── figures/
│   │   ├── quality_distribution.png
│   │   ├── correlation_matrix.png
│   │   └── chemical_vs_quality.png
│   └── models/
│       ├── logistic_regression_results.txt
│       └── knn_results.txt
│
├── README.md
└── requirements.txt
```
### Data Preparation

Imported red and white wine datasets from UCI.

Combined both datasets by appending rows into a single dataframe:

wine_data_all


All analyses and models are based on this combined dataset.

### Analysis Objectives

- Import and Combine Data

- Check Data Types

- Missing Value Analysis

- Correlation Analysis (Excluding Quality)

- Identify strong positive and negative relationships.

- Assess potential multicollinearity.

- Wine Quality Distribution

- Visualize the frequency of wines across different quality ratings.

- Impact of Chemical Attributes on Wine Quality

- Identify the most impactful chemical components.

- Recoding Wine Quality

- Normalization of Numeric Attributes

- Predicting Wine Quality – **Logistic Regression**

- Predicting Wine Quality – **K-Nearest Neighbors (KNN)**

- Classify wines based on nearest neighbors.

- Confusion Matrices.

- Visualize correct and incorrect classifications.

- Model Performance Evaluation

- Compare Logistic Regression and KNN performance.

### Key Insights

Alcohol content shows a strong positive relationship with wine quality.

Several chemical attributes exhibit meaningful correlations.

Model performance varies by algorithm, with trade-offs between precision and recall.

Normalization significantly improves KNN performance.

### How to Run the Project
```
Clone the repository:

git clone <repository-url>


Install dependencies:

pip install -r requirements.txt


Open the notebook:

jupyter notebook notebooks/wine_quality_analysis.ipynb
```

Run all cells sequentially.
