# Basel-III-Credit-Risk

This project focuses on building a credit risk scorecard to estimate the Probability of Default (PD) using customer data. It follows a complete end-to-end modeling pipeline from preprocessing to validation and monitoring.

 1. Data Preprocessing
Cleaned the raw dataset and handled missing values using appropriate imputation methods.

Applied normalization to scale continuous features for model stability.


2. Exploratory Data Analysis & Feature Engineering
Classified variables into categorical and numerical types.

Performed Fine Classing and calculated Weight of Evidence (WoE) and Information Value (IV) to evaluate variable predictive power.

3. Model Development

Built a Logistic Regression model to estimate the Probability of Default (PD) for each customer.

Selected variables based on IV, business logic, and multicollinearity checks.


4. Scorecard Development
Transformed the logistic regression output into a credit scorecard using binning and score scaling techniques.

Designed scorecard to assist in credit decisioning and risk-based pricing.

5. Model Validation
Evaluated model performance using:

- ROC Curve / AUC

- KS Statistic

- Gini Coefficient

- Assessed overfitting and model stability across training and validation sets.

6. Population Monitoring
Monitored Population Stability Index (PSI) to track changes in data distribution over time.

Flagged significant shifts in customer behavior for early warning and model recalibration.


