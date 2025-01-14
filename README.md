# Predicting_Telecom_Customer_Churn

Predicting customer churn: LogisticRegression, RandomForest

The Indian telecommunications (telecom) industry is undergoing significant transformation, with an increasing number of telecom companies entering the market and a growing trend of customers switching between service providers. Customer "churn" refers to the phenomenon where users discontinue a company's services or products. For telecom companies, understanding the factors that contribute to customer retention is vital for improving service quality and boosting customer satisfaction. For the data scientist, leading this project, the goal is to analyze the complex interplay of customer behavior and demographics in the Indian telecom landscape to predict churn. This analysis will leverage two extensive datasets from four leading telecom providers: Airtel, Reliance Jio, Vodafone, and BSNL.

## Project Instructions
Does Logistic Regression or Random Forest produce a higher accuracy score in predicting telecom churn in India?
- Load the two CSV files into separate DataFrames. Merge them into a DataFrame named `churn_df`. Calculate and print churn rate, and identify the categorical variables in `churn_df`.
- Convert categorical features in `churn_df` into `features_scaled`. Perform feature scaling separating the appropriate features and scale them. Define scaled features and target variable for the churn prediction model.
- Train Logistic Regression and Random Forest Classifier models, setting a random seed of 42. Store model predictions in `logreg_pred` and `rf_pred`.
- Assess the models on test data. Assign the model's name with higher accuracy (`"LogisticRegression"` or `"RandomForest"`) to `higher_accuracy`.

- `telecom_demographics.csv` contains information related to Indian customer demographics:

| Variable             | Description                                      |
|----------------------|--------------------------------------------------|
| `customer_id `         | Unique identifier for each customer.             |
| `telecom_partner `     | The telecom partner associated with the customer.|
| `gender `              | The gender of the customer.                      |
| `age `                 | The age of the customer.                         |
| `state`                | The Indian state in which the customer is located.|
| `city`                 | The city in which the customer is located.       |
| `pincode`              | The pincode of the customer's location.          |
| `registration_event` | When the customer registered with the telecom partner.|
| `num_dependents`      | The number of dependents (e.g., children) the customer has.|
| `estimated_salary`     | The customer's estimated salary.                 |

- `telecom_usage` contains information about the usage patterns of Indian customers:

| Variable   | Description                                                  |
|------------|--------------------------------------------------------------|
| `customer_id` | Unique identifier for each customer.                         |
| `calls_made` | The number of calls made by the customer.                    |
| `sms_sent`   | The number of SMS messages sent by the customer.             |
| `data_used`  | The amount of data used by the customer.                     |
| `churn`    | Binary variable indicating whether the customer has churned or not (1 = churned, 0 = not churned).|

