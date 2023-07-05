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


## Model Training


After preprocessing the data, various machine learning models can be applied to predict credit scores. Some of the models that can be explored include logistic regression, decision trees, random forests, and gradient boosting machines.

For each model, the preprocessed dataset is split into training and testing sets using techniques like cross-validation or a simple train-test split. The model is then trained on the training set and evaluated using appropriate metrics such as accuracy, precision, recall, or F1-score.
### Various Model and their performance

|      Model Name            | Accuracy Score | Precision Score | Recall Score | F1 Score  |
|----------------------------|----------------|-----------------|--------------|-----------|
| LogisticRegression         | 0.810289       | 0.179641        | 0.728477     | 0.288210  |
| DecisionTreeClassifier     | 0.880936       | 0.745781        | 0.711319     | 0.728142  |
| RandomForestClassifier     | 0.923766       | 0.689711        | 0.937130     | 0.794606  |
| GradientBoostingClassifier | 0.915619       | 0.657594        | 0.926380     | 0.769182  |
| KNeighborsClassifier       | 0.832984       | 0.485574        | 0.645441     | 0.554209  |
| GaussianNB                | 0.817155       | 0.242243        | 0.713141     | 0.361642  |
| LinearDiscriminantAnalysis | 0.847649       | 0.465433        | 0.723350     | 0.566413  |
| xgb_type1                  | 0.925047       | 0.681546        | 0.954996     | 0.795426  |
| xgb_type2                  | 0.932845       | 0.742515        | 0.929155     | 0.825416  |
| xgb_type3                  | 0.929702       | 0.744692        | 0.910180     | 0.819162  |
| xgb_type4                  | 0.929818       | 0.740338        | 0.915209     | 0.818537  |
| CatBoostClassifier         | 0.931681       | 0.707131        | 0.963650     | 0.815699  |
| AdaBoostClassifier         | 0.879655       | 0.597169        | 0.788641     | 0.679678  |
| RidgeClassifier            | 0.843925       | 0.375612        | 0.780543     | 0.507166  |


##  Conclusion

In this project, we have successfully built a credit score model using a dataset of credit-related information. By preprocessing the data, handling missing values, and applying one-hot encoding, we ensure that the dataset is ready for model training. By exploring various machine learning models, we aim to predict creditworthiness accurately and help make informed credit-related decisions.

Feel free to modify and adapt this README file according to your project requirements, providing more details about the dataset, model evaluation, or any additional steps involved in your credit score project.
