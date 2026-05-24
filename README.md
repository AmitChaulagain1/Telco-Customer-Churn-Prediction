# Telco Customer Churn Prediction Using Machine Learning

## Project Overview

This project focuses on predicting customer churn in a telecommunications company using machine learning techniques in Python. Customer churn prediction is an important business problem because retaining existing customers is often less expensive than acquiring new customers.

The project applies a complete end-to-end machine learning workflow including:
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Data preprocessing
- Model building
- Hyperparameter tuning
- Cross-validation
- PCA and clustering analysis
- Model comparison and interpretation

The goal of the project is to identify customers who are likely to leave the company and understand the factors influencing churn behavior.

---

## Business Problem

Telecommunication companies face customer loss due to competition, pricing, service quality, and customer dissatisfaction. By predicting churn early, companies can:
- Improve customer retention
- Reduce revenue loss
- Offer personalized retention strategies
- Improve customer satisfaction

This project builds predictive classification models to identify high-risk churn customers.

---

## Dataset

Dataset Used:
- Telco Customer Churn Dataset (Kaggle)

Dataset Characteristics:
- 7,043 customer records
- 21 original features
- Binary target variable: `Churn`

Target Variable:
- `0` = Customer did not churn
- `1` = Customer churned

Features include:
- Customer demographics
- Account information
- Contract type
- Billing information
- Internet services
- Support services

---

## Technologies and Libraries Used

### Programming Language
- Python

### Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

### Machine Learning Techniques
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- HistGradientBoosting
- KNN
- Naive Bayes
- LDA / QDA
- Neural Networks
- PCA
- K-Means Clustering

---

## Project Workflow

### 1. Data Cleaning
- Converted `TotalCharges` to numeric format
- Removed duplicate rows
- Dropped customer identifier column
- Handled missing values using imputation pipelines

### 2. Feature Engineering
Created additional features including:
- Tenure groups
- Average charges per tenure
- Internet service flag
- Multiple service count

### 3. Exploratory Data Analysis (EDA)
Performed:
- Target distribution analysis
- Numeric feature distributions
- Categorical variable analysis
- Correlation heatmaps
- Outlier analysis

### 4. Data Preprocessing
Applied:
- Median imputation
- Standard scaling
- One-hot encoding
- ColumnTransformer pipelines

### 5. Machine Learning Modeling
Developed and compared multiple baseline and improved classification models.

### 6. Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Cross-validation

### 7. Additional Analysis
- PCA dimensionality reduction
- K-Means clustering
- Learning curves
- Feature importance analysis

---

## Best Model Performance

### Best Model
**Logistic Regression Baseline**

### Performance Metrics

| Metric | Score |
|---|---|
| Test Accuracy | 0.807 |
| Precision | 0.681 |
| Recall | 0.511 |
| F1 Score | 0.584 |
| Test ROC-AUC | 0.842 |

The Logistic Regression model achieved the best balance between predictive performance, generalization, and stability.

---

## Key Findings

The analysis revealed several important churn patterns:

- Customers with month-to-month contracts had significantly higher churn rates.
- Customers with shorter tenure were more likely to churn.
- Higher monthly charges increased churn probability.
- Customers without online security and tech support services showed higher churn risk.
- Fiber optic internet customers experienced higher churn compared to DSL customers.

These findings can help businesses create targeted retention strategies and improve customer satisfaction.

---

## Cross-Validation Results

Cross-validation confirmed the stability and consistency of the top-performing models.

| Model | Mean CV ROC-AUC |
|---|---|
| Improved Logistic Regression | 0.848 |
| Improved Gradient Boosting | 0.847 |
| Improved Random Forest | 0.846 |

---

## PCA and Clustering Insights

PCA and K-Means clustering showed that natural customer groups exist within the dataset. However, supervised machine learning models performed better for churn prediction because the target variable was clearly defined.

---

## Files Included

- `Telco_Churn_Project_Notebook.ipynb` → Full Jupyter Notebook
- `Telco_Churn_Project_Notebook.pdf` → Exported project report
- `README.md` → Project documentation

---

## Skills Demonstrated

- Machine Learning
- Predictive Analytics
- Classification Modeling
- Feature Engineering
- Data Cleaning
- Exploratory Data Analysis
- Hyperparameter Tuning
- Cross-Validation
- PCA and Clustering
- Business Analytics
- Python Programming

---

## Future Improvements

Possible future improvements include:
- Advanced ensemble methods
- SMOTE or advanced imbalance handling
- Deep learning approaches
- Deployment using Streamlit or Flask
- Real-time churn prediction systems

---

## Author

**Amit Chaulagain**  
MS in Data Analytics – Oklahoma City University  
Aspiring Data Analyst | SQL | Power BI | Python | Machine Learning
