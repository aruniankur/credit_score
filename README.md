# credit_score_Project

This project aims to build a credit score model using a dataset containing credit-related information. The goal is to predict creditworthiness based on various features such as age, income, and employment status.
## dataset 
The dataset used in this project is stored in a CSV file named credit_risk_dataset.csv. It contains the following columns:

| Feature Name                 | Description                      |
|------------------------------|----------------------------------|
| person_age                   | Age                              |
| person_income                | Annual Income                    |
| person_home_ownership        | Home ownership                   |
| person_emp_length            | Employment length (in years)     |
| loan_intent                  | Loan intent                      |
| loan_grade                   | Loan grade                       |
| loan_amnt                    | Loan amount                      |
| loan_int_rate                | Interest rate                    |
| loan_status                  | Loan status (0 is non-default, 1 is default) |
| loan_percent_income          | Percent income                   |
| cb_person_default_on_file    | Historical default               |
| cb_preson_cred_hist_length   | Credit history length            |


## Preprocessing

To prepare the dataset for modeling, the following steps are performed:

Loading the Dataset: The dataset is loaded into a pandas DataFrame using the read_csv() function.

Handling Missing Values: Any rows with missing values are removed from the dataset using the dropna() function. This ensures that the model is trained on complete data.

One-Hot Encoding: Categorical variables, such as person_home_ownership, loan_intent, are encoded using one-hot encoding. This converts each category into a binary column, making it suitable for training machine learning models.
