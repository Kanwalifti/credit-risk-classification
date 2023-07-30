## Overview of the Analysis
The objective of this analysis is to develop a model capable of determining the creditworthiness of borrowers.

The dataset used for this analysis comprises historical lending data obtained from a peer-to-peer lending services company.

The dependent variable (y value) in this analysis is the "loan status," indicating whether a loan is considered healthy or at risk.

The independent variables (x values) include loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and derogatory marks.

To conduct the analysis, the data is first split into training and test sets. Next, the dependent and independent variables are defined. A logistic regression model is then created and trained using the original data. The trained model is used to make predictions, and its performance is evaluated.

To account for data imbalances, two different logistic regression models are created: one using the original dataset and another using a randomly oversampled dataset. The oversampling technique helps to address any class imbalances in the "loan status" variable. The results of both models are compared using the scikit-learn library.

Overall, the goal is to develop a reliable model that can accurately predict the creditworthiness of borrowers, and this analysis explores different approaches to achieve that.

# Results
Machine Learning Model 1: Logistic Regression Model with Original Data Original Data
![Original_Data]()

Machine Learning Model 2: Logistic Regression Model with StandardScale() Data Scaled Data
![Scaled_Data]()

Machine Learning Model 3: RandomForest Calssifier with Original Data RandomForest Data
![RandomForestClassifier_Data]()


# Summary
The analysis indicates that the collected data is suitable for training and testing the Machine Learning Classification Model effectively. However, to improve the model's predictions, it is essential to address the issue of class imbalance in the dataset.

By randomforest classifier the data, the class imbalance problem is mitigated, leading to higher balanced accuracy and recall scores. The increased recall value allows the model to make more accurate predictions for risky loans.

The consequences of incorrect predictions involve two issues: false positives and false negatives. False positives occur when users are incorrectly flagged as risky despite being healthy borrowers, while false negatives occur when risky borrowers are not identified as such.

Both cases have associated costs, making it vital to predict both positive (risky) and negative (healthy) instances accurately. As a result, the model should strive for good accuracy in terms of both classes to minimize the impact of misclassification.
