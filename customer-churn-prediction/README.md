# Customer Churn Prediction — Python & Machine Learning

## Project Overview

This project uses **Python and Machine Learning** to analyze customer churn and predict whether a customer is likely to leave a telecommunications service.

The project uses the **IBM Telco Customer Churn dataset** and follows an end-to-end Data Science workflow, from data cleaning and exploratory analysis to machine learning model development, evaluation, and interpretation.

## Objective

The main objectives of this project are to:

- Explore customer data and identify patterns related to churn
- Perform data cleaning and preprocessing
- Conduct Exploratory Data Analysis (EDA)
- Build classification models using Python
- Evaluate and compare different Machine Learning models
- Identify important features that contribute to model predictions

## Dataset

The project uses the **Telco Customer Churn** dataset.

The dataset contains information about:

- Customer demographics
- Customer tenure
- Phone and internet services
- Contract type
- Online services
- Payment methods
- Monthly charges
- Total charges
- Customer churn status

The target variable is:

- `0` — Customer stayed
- `1` — Customer churned

## Data Preparation

The dataset was prepared using the following steps:

- Checked the dataset structure and data types
- Checked for missing values
- Converted `TotalCharges` to a numerical data type
- Handled 11 previously blank `TotalCharges` values
- Checked for duplicate records
- Removed `customerID` from the modelling data
- Converted the `Churn` target into binary values
- Separated numerical and categorical features
- Applied feature scaling to numerical variables
- Applied one-hot encoding to categorical variables
- Split the data into training and testing sets

## Exploratory Data Analysis

Several analyses were performed to understand customer churn.

### Churn Distribution

Approximately 73.46% of customers stayed, while 26.54% churned.

### Contract Type

Churn was examined across month-to-month, one-year, and two-year contracts.

### Customer Tenure

Customers with shorter tenure showed higher observed churn rates than customers with longer tenure.

### Monthly Charges

Monthly charges were compared between customers who stayed and customers who churned.

These analyses helped identify variables that could be useful for Machine Learning.

## Machine Learning Models

Two classification models were developed:

### 1. Logistic Regression

Logistic Regression was used as the first classification model and baseline.

### 2. Random Forest

Random Forest was used as a second model to compare its performance with Logistic Regression.

Both models were trained using the preprocessed training data.

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve

### Results

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 73.88% | 51% | 78% | 61% | 0.8418 |
| Random Forest | 76.15% | 54% | 72% | 62% | 0.8410 |

The results show that the models have different strengths. Random Forest achieved higher accuracy and F1-score, while Logistic Regression achieved higher recall and a slightly higher ROC-AUC.

## Feature Importance

Feature importance was analyzed using the Random Forest model.

Important features included:

- Tenure
- Total Charges
- Monthly Charges
- Contract type
- Internet Service
- Payment Method
- Online Security
- Technical Support

Permutation importance was also used as a second feature-analysis method to examine the effect of individual features on model performance.

The strongest permutation-importance results included:

1. Tenure
2. Contract — Two year
3. Internet Service — Fiber optic
4. Contract — One year
5. Total Charges

These results describe how the model uses the available features and should not be interpreted as proof that a feature directly causes customer churn.

## Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Google Colab**
- **Jupyter Notebook**

## Skills Demonstrated

This project demonstrates practical experience in:

- Python programming
- Data cleaning
- Exploratory Data Analysis
- Data visualization
- Feature preprocessing
- One-hot encoding
- Feature scaling
- Classification
- Machine Learning model evaluation
- Model comparison
- ROC-AUC analysis
- Feature importance
- Permutation importance
- Data-driven problem solving

## Project Notebook

The complete implementation is available in:

`customer-churn-prediction-python-ml.ipynb`

## Future Improvements

Possible future improvements include:

- Hyperparameter tuning
- Cross-validation
- Testing additional classification algorithms
- Improving model performance
- Exploring different probability thresholds
- Testing the models on additional customer datasets
- Deploying the final model as a simple application

## Conclusion

This project demonstrates an end-to-end approach to solving a real-world-style business problem using **Python and Machine Learning**.

It helped strengthen my practical skills in working with data, performing EDA, preparing datasets, building classification models, evaluating model performance, and interpreting Machine Learning results.

---

**Data Science Student | Python | Machine Learning | Data Analysis | EDA**
