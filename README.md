# Credit Card Fraud Detection
## Introduction
Credit card is a high-yield and high-risk banking business. With the development of the credit card business, banks are 
using the Internet and mobile data to build customer credit rating systems. It is crucial for banks to assess whether 
the customer would default in the future based on customers' information. In this report, supervised learning methods 
including Logistic Regression, K-Nearest Neighbors (KNN), Random Forest, and Gradient Boosting Decision Tree (GBDT) 
algorithms were used to construct a prediction model. Confusion matrix, accuracy, recall, precision, Matthews Correlation 
Coefficient (MCC), and AUC-ROC curve were used for evaluating models. Also, GridSearchCV was used to find the optimal 
hyperparameter. This project purposes on helping businesses identify potential fraudulent customers to reduce credit risk.

## Built With
* Python 3.7


## Conclusion and Improvements 
During the whole project, Logistic Regression, KNN, Random Forest, and GBDT algorithms were applied. The performance of 
the model was mainly assessed through recall, precision, MCC, and learning curve. When companies use machine learning 
models to try to identify fraudulent users, they need to consider both the cost of missing detection and the cost of 
misclassification. When a model has a high recall but a low precision, excessive misjudgments would damage the company’s 
financial condition. Similarly, when the precision of a model is high, but the recall is not good enough, many actual 
fraudulent users would be missed, thus affecting the profits of the companies. 

Based on the above discussion, it finds that Logistic Regression performs better than others. However, it does not mean 
that the Logistic Regression model is always the best since the model performance is affected by hyperparameters. In our 
project, although we used GridSearchCV to tune hyperparameters and find the optimal hyperparameters, only a few 
combination hypermeters of models were tried. It means that the hyperparameter attained may be a locally optimal, not a 
global optimal hypermeter. Hence, the robustness of the model is highly recommended. Besides, GridSearchCV is 
time-consuming since it creates a model of every combination of the hyperparameter to find the best parameters. So, in 
the future, we may explore other methods to train the dataset and improve prediction accuracy. 


## Author 

Dai Luqiao 

Miao qinglang 

Yan Siyu

Zhang Zhongyi


## Reference 
[1] Henrique Aguiar. What Is Imbalanced Data and How to Handle It?. https://www.turintech.ai/what-is-imbalanced-data-and-how-to-handle-it/

[2] Chicco D, Jurman G. The advantages of the Matthews correlation coefficient (MCC) over F1 score and accuracy in binary 
classification evaluation. BMC Genomics. 2020 Jan 2;21(1):6. doi: 10.1186/s12864-019-6413-7. PMID: 31898477; PMCID: PMC6941312.

[3] The right way of using SMOTE with Cross-validation.The right way of using SMOTE with Cross-validation | by KSV Muralidhar | Towards Data Science

[4] StratifiedKFold vs KFold in scikit-learn.python - StratifiedKFold vs KFold in scikit-learn - Stack Overflow

[5] How to use Matthews Coefficient for scoring in GridSearchCV?.python 3.x - How to use Matthews Coefficient for scoring in GridSearchCV? - Stack Overflow

[6] Credit Card Fraud Detection.Credit Card Fraud Detection | Kaggle

[7] Learning Curve.Learning Curve — Yellowbrick v1.5 documentation (scikit-yb.org)