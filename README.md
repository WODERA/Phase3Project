# Loan Approval Prediction Project
This project aims to predict loan approval statuses using machine learning models. It involves data preprocessing, exploratory data analysis (EDA), model building, and evaluation.
## Objective
The goal of this project is to automate loan approval decisions for a financial institution. By analyzing applicants' demographic and financial details, the models predict whether a loan application will be approved or rejected.
## Data Set
The project used a dataset with the following features:
Target Variable: Loan_Status (Y: Approved, N: Rejected)
Features:
Gender: Applicant's gender.
Married: Marital status.
Dependents: Number of dependents.
Education: Education level (Graduate/Not Graduate).
Self_Employed: Employment type.
ApplicantIncome: Applicant's income.
CoapplicantIncome: Coapplicant's income.
LoanAmount: Loan amount requested.
Loan_Amount_Term: Loan repayment term (in months).
Credit_History: Applicant's credit history (1: Good, 0: Poor).
Property_Area: Urban, Semi-Urban, or Rural area.
The dataset was split into training and test sets for model evaluation.
## Exploratory Data Analysis (EDA)
EDA was performed to understand the data:
Missing Values were identified and imputed.
Outliers were detected and handled using the Interquartile Range (IQR) and log transformations.
Categorical Features: Distributions were visualized using count plots.
Correlation: Numerical features were analyzed using a heatmap.
## Model Development
The following models were built and evaluated:

### Logistic Regression:

Accuracy: ~82.2%
Strong recall for approved loans but low recall for rejected loans.

### Decision Tree Classifier:
Accuracy: ~78%
High precision for approved loans but struggled with rejected loans (low recall).

### Random Forest Classifier:
Accuracy: 82.7% (Best-performing model)
High recall for approved loans and improved performance for rejected loans.

## Key Findings
Credit_History and LoanAmount were significant predictors of loan approval.
Class imbalance (fewer rejected loans) impacted model performance, especially for rejected loan predictions.
Random Forest performed best, achieving a balanced trade-off between precision and recall.

## Future Improvements
Address class imbalance
Optimize Random Forest hyperparameters for even better performance.

#### Files in This Repository
Notebook.ipynb: Jupyter Notebook with full project code and analysis.
train.csv / test.csv: Input datasets.
README.md: Project documentation.



