# Credit-card-fraud-detection💳
Credit card fraud is one of the most common online scams. Credit card numbers, PINs, and security codes can be easily stolen and used to make fraudulent transactions. This can cause huge financial losses for traders and consumers. However, credit card companies are ultimately obligated to reimburse their customers for any losses. Therefore, it is extremely important that credit card companies and other financial institutions can detect fraud before it occurs.

![ccd](https://github.com/ishagoel840/Credit-card-fraud-detection/assets/163164421/f66f76e4-15b3-4cc2-8aee-991923e1bed6)


## Problem Statement:
A credit card 💳 is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
**We have to build a classification model to predict whether a transaction is fraudulent or not.**

The dataset is taken from kaggle [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## Content:
It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. **Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.**

## Model Pipeline:
### - Exploratory Data Analysis (EDA):

Conduct comprehensive exploratory data analysis to understand the distribution of fraudulent and non-fraudulent transactions.

Visualized transaction features such as amount, time, and transaction type to identify patterns and anomalies.

### - Dealing with Imbalanced data: 
This data set is highly imbalanced. Addressed class imbalance using techniques such as oversampling, undersampling, or synthetic data generation.

### - Data Preprocessing:

Handled missing or erroneous values in the dataset.

Outlier treatment.

### - Feature Engineering:

Extracted relevant features from the dataset, including transaction amount, time of transaction, and frequency of transactions.

Normalized or scaled features to enhance model performance.

### - Model Selection and Training:

Experiment with various classification algorithms suitable for imbalanced datasets, such as Logistic Regression, XgBoost and K Nearest Neighbour (KNN).

Utilized  hyperparameter tuning to optimize model performance.

Evaluate models based on metrics like precision, recall, F1-score, and area under the ROC curve (AUC-ROC).
### - Model Evaluation and Validation:

Validate trained models using a separate test dataset .

Assess model performance in terms of its ability to accurately classify fraudulent and non-fraudulent transactions while minimizing false positives and false negatives.

### - Deployment and Monitoring:

Deployment plan to the trained model into production systems for real-time fraud detection.

Implement monitoring mechanisms plan to track model performance over time and update the model as needed to adapt to evolving fraud patterns.

# Conclusion:
|S.no.|Model|	Accuracy|	Precision|	Recall|	F1 Score|
|---|---|---|---|---|---|
|0	|Logistic Regression|	0.981614|	0.988101|	0.975042|	0.975042|
|---|---|---|---|---|---|
|1	|KNN	|0.999165|	0.998335	|1.0	|1.0|
|---|---|---|---|---|---|
|2	|XGBoost|	0.990064|	0.993775|	0.986345|	0.986345|
|---|---|---|---|---|---|






### KNN Model shows the highest accuracy score with an accuracy of 99.99%.


