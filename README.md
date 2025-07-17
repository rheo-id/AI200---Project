# AI200---Project
AI200: Applied Machine Learning,

In my capstone project, I successfully developed a machine learning model to predict loan defaults for LendingClub. My goal was to identify high-risk applicants to help the company minimize credit loss. I'm proud to say that my final model achieved a strong performance, and I've outlined the key results of my work below.

- **I performed thorough data cleaning and feature engineering**. To prepare the data for modeling, I handled missing values in key columns like <revol_util> and <mort_acc> by filling them with the median and mean, respectively. I also engineered several new features, such as extracting numerical values for employment length, parsing dates to get month and year components, and even creating a custom <risk_lvl> category based on income and bankruptcy records to better segment applicants.

- **I successfully encoded all categorical data for machine learning**. I converted all non-numeric features, like <grade>, <home_ownership>, and my new <risk_lvl> feature, into a numerical format using both label encoding and custom mapping. This made the data fully compatible with the machine learning models I planned to use.

- **I built and evaluated multiple advanced models**. I didn't just stick to a baseline; I experimented with powerful ensemble methods. I built a <VotingClassifier> that combined LightGBM and CatBoost, and I also implemented a standalone XGBoost model. I used the AUC (Area Under Curve) score to evaluate their performance.

- **My final XGBoost model achieved an excellent AUC score of 0.933**. After comparing my models, the tuned XGBoost classifier proved to be the top performer on my validation set. This high AUC score indicates that the model is very effective at distinguishing between applicants who are likely to default and those who are not.

- **I generated final predictions for submission. Using my best-performing model**, I processed the official test dataset, applied all the same cleaning and feature engineering steps, and generated the final prediction files (<javier_chandra_predictions_2.csv> and <javier_chandra_predictions_xgboost_2.csv>) required for the competition.
