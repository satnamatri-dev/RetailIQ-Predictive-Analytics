
# RetailIQ – Retail Analytics and Customer Behaviour Prediction System

![Python](https://img.shields.io/badge/Python-3.13-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Course](https://img.shields.io/badge/Course-INT234-purple)

## Project Overview

RetailIQ is a Predictive Analytics project developed to analyse retail transaction data, identify customer purchasing patterns, understand sales behaviour, and apply machine learning techniques to support data-driven business decisions.

The project uses the **UCI Online Retail Dataset** and Python-based data science libraries to perform exploratory data analysis, data preprocessing, feature engineering, regression modelling, and customer repeat-purchase classification.

## Project Objectives

- Analyse retail transaction data and identify sales patterns.
- Clean and preprocess raw transactional data.
- Perform exploratory data analysis using statistical and visual techniques.
- Calculate revenue and customer-level business metrics.
- Apply RFM (Recency, Frequency, Monetary) analysis.
- Develop regression models for invoice revenue analysis.
- Build classification models to predict customer repeat purchases.
- Evaluate machine learning models using appropriate performance metrics.

## Dataset

**Dataset:** Online Retail Dataset  
**Source:** UCI Machine Learning Repository  
**Original Records:** 541,909  
**Time Period:** December 2010 – December 2011  
**Features:** 8 original columns

The dataset contains transactional records from a UK-based online retail business.

Dataset source:  
https://archive.ics.uci.edu/dataset/352/online+retail

The original dataset is not included in this repository. Download it from the official source and place `Online Retail.xlsx` in the project directory before running the notebook.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels (for OLS, if used)
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Exploratory Data Analysis

- Dataset inspection and statistical summaries.
- Missing value and duplicate analysis.
- Distribution analysis of numerical variables.
- Correlation analysis.
- Country-wise transaction analysis.

### 2. Data Cleaning and Preprocessing

- Removal of duplicate records.
- Handling missing CustomerID and Description values.
- Filtering invalid and non-positive quantities and prices.
- Conversion of data types.
- IQR-based outlier detection.
- Feature scaling using MinMaxScaler and StandardScaler.

### 3. Feature Engineering

- Total revenue calculation.
- Extraction of year, month, day, hour, and weekday.
- Customer-level aggregation.
- Invoice-level business metrics.
- RFM feature generation.

### 4. Regression Modelling

The following regression techniques were implemented:

- Simple Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Ordinary Least Squares (OLS)

**Evaluation Metrics:**
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

### 5. Customer Repeat-Purchase Classification

Classification models were developed to estimate whether a customer would make another purchase during the final three-month evaluation period, using earlier transaction history.

Models implemented:

- Logistic Regression
- K-Nearest Neighbours (KNN)
- Gaussian Naive Bayes
- Decision Tree Classifier
- Support Vector Machine (SVM)

**Evaluation Metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Log Loss
- Confusion Matrix

## Repository Structure

```text
RetailIQ-Predictive-Analytics/
│
├── README.md
├── RetailIQ_Predictive_Analytics.ipynb
├── requirements.txt
│
├── data/
│   └── README.md
│
├── reports/
│   └── RetailIQ_Project_Report.pdf
│
├── results/
│   ├── RetailIQ_Regression_Results.csv
│   └── RetailIQ_Classification_Results.csv
│
└── visualizations/
    └── project_charts/
```

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/RetailIQ-Predictive-Analytics.git
```

2. Open the project directory:

```bash
cd RetailIQ-Predictive-Analytics
```

3. Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl statsmodels jupyter
```

4. Download the Online Retail dataset from the UCI repository.

5. Place `Online Retail.xlsx` in the project directory.

6. Launch Jupyter Notebook:

```bash
jupyter notebook
```

7. Open `RetailIQ_Predictive_Analytics.ipynb` and execute the cells sequentially.

## Results and Business Applications

RetailIQ demonstrates how retail transaction data can be used to:

- Understand customer purchasing behaviour.
- Identify revenue patterns and high-value customers.
- Examine relationships between invoice characteristics and revenue.
- Estimate customer repeat-purchase behaviour.
- Support customer retention and business planning.

Actual model performance results are available in the exported results files after successful execution of the notebook.

## Limitations

- The analysis is based on historical transaction data.
- The dataset covers a limited period.
- Revenue has a direct mathematical relationship with quantity and unit price.
- Repeat-purchase predictions are limited to the defined historical evaluation period.
- Model performance depends on data quality and class distribution.

## Future Scope

- Customer segmentation using K-Means clustering.
- Market basket analysis using association rules.
- Dimensionality reduction using PCA.
- Neural network-based prediction.
- Ensemble learning using Random Forest and boosting.
- Interactive retail analytics dashboard.

## Author

**Satnam Singh**  
Registration Number: 12418878  
Course Code: INT234  
Lovely Professional University  
Phagwara, Punjab, India

## Academic Project

Developed as part of the Predictive Analytics coursework (INT234).

---

**If you find this project useful, feel free to explore the repository and its implementation.**
