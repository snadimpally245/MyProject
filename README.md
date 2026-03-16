Bankruptcy Risk Prediction Using Machine Learning
Project Overview

This project focuses on predicting the likelihood of corporate bankruptcy using machine learning techniques. Financial ratios and company financial indicators are used as input features to classify companies as either bankrupt or non-bankrupt. Early bankruptcy prediction is valuable for investors, financial institutions, and business analysts to support better decision-making and risk management.

The project was implemented using Altair AI Studio (RapidMiner) and includes a complete machine learning pipeline consisting of data preprocessing, exploratory data analysis, model training, and performance evaluation.

Dataset

The dataset contains various financial indicators and ratios describing company financial health. These attributes capture profitability, liquidity, leverage, and operational efficiency metrics that are commonly used in financial risk assessment.

Target Variable

Bankrupt?

1 → Bankrupt

0 → Non-Bankrupt

Data Preprocessing

Several preprocessing steps were applied to prepare the dataset for machine learning:

Missing values were handled using the Replace Missing Values operator.

Financial ratios were standardized using Z-score normalization to ensure all features are on a comparable scale.

The target variable was converted to a binominal class label.

The dataset was divided into training (80%) and testing (20%) subsets to evaluate model performance on unseen data.

Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand the distribution and relationships of financial variables. Different visualizations were used including:

Histograms for feature distributions

Scatter plots for feature relationships

Boxplots for outlier detection

These analyses helped identify important financial indicators associated with bankruptcy risk.

Machine Learning Models

Three classification algorithms were implemented and compared:

Logistic Regression

Support Vector Machine (SVM)

Random Forest

Each model was trained on the training dataset and evaluated using the testing dataset.

Model Evaluation Metrics

The models were evaluated using several performance metrics:

Accuracy

Precision

Recall

F1 Score

Area Under the ROC Curve (AUC)

These metrics help assess how well each model distinguishes between bankrupt and non-bankrupt companies.

| Model                  | Accuracy | Precision | Recall | AUC   |
| ---------------------- | -------- | --------- | ------ | ----- |
| Logistic Regression    | 95.97%   | 44.19%    | 38%    | 0.906 |
| Support Vector Machine | 96.63%   | 70%       | 14%    | 0.808 |
| Random Forest          | 96.70%   | 85.71%    | 12%    | 0.906 |

Final Model
Based on overall performance comparison, the Random Forest model achieved the highest accuracy and strong predictive capability. Therefore, Random Forest was selected as the final model for bankruptcy prediction.
