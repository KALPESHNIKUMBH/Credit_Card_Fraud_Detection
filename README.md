# Credit_Card_Fraud_Detection

## Problem Statement 
* For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.
* In the banking industry, credit card fraud detection using machine learning and deep learning is not only a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees as well as denials of legitimate transactions.
* In this project we will detect fraudulent credit card transactions with the help of Machine learning and deep learnig models.
* We will analyse customer-level data that has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group. 

## Theory about Credit Card Fraud
# **What is Credit Card Fraud Detection?**
  * Credit card fraud is a term that has been coined for unauthorized access of payment cards like credit cards or debit cards to pay for using services or goods
  *  Hackers or fraudsters may obtain the confidential details of the card from unsecured websites. When a fraudster compromises an individual's credit/debit card, everyone involved in the process suffers, right from the individual whose confidential data has been leaked to the businesses (generally banks) who issue the credit card and the merchant who is finalizing the transaction with purchase
  * This makes it extremely essential to identify the fraudulent transactions at the onset. Financial institutions and businesses like e-commerce are taking firm steps to flag the fraudsters entering the system.  Various advanced machine learning technologies are at play, assessing every transaction and stemming the fraud users in its nip using behavioral data and transaction patterns
  * The process of automatically differentiating between fraudulent and genuine users is known as “credit card fraud detection” 


## How does Credit Card Fraud work?
  * A credit card is one of the most used financial products to make online purchases and payments  such as gas, groceries, TVs, traveling, shopping bills, and so on because of the non-availability of funds at that instance. Credit cards are of most value that provide various benefits in the form of points while using them for different transactions. There are several categories of credit card fraud that are prevalent in today’s time:

    1. Lost/Stolen cards: People steal credit cards from the mail and use them illegally on behalf of the owner. The process of blocking credit cards that have been stolen and re-issuing them is a hassle for both customers and credit card companies. Some financial institutions keep the credit cards blocked until it is verified that the rightful owner has received the card. 

    2. Card Abuse: The customer buys goods and items on the credit card but has no intention to pay back the amount charged by the bank for the same. These customers stop answering the calls as the deadline to settle the dues approaches. Sometimes they even declare bankruptcy—this type of fraud results in losses of millions every year. 

    3. Identity Theft: The customers apply illegitimate information, and they might even steal the details of a genuine customer to apply for a credit card and then misuse it. In such cases, even card blocking can not stop the credit card from falling into the wrong hands.

    4. Merchant Abuse: Some merchants show illegal transactions (that never occurred) for money laundering. For performing these illicit transactions, legal information of genuine credit card users is stolen to generate replicas of the cards and use it for illegal work.

  * Many traditional old-school techniques have been used since time in-memorial for credit card fraud detection like CVV verification, geolocation tracking, IP Address verification, etc. But over time, the criminals are using more advanced techniques to commit crimes, and it is impossible to prevent them all using only traditional methods. Millions of transactions are processed every second in today’s world, which takes it beyond human intelligence to process all the data to identify the behavioral patterns of the fraudsters. This is where credit card fraud detection using machine learning plays a vital role. 

  * Financial institutions increasingly depend upon automated machine learning systems to make intelligent decisions and protect businesses against substantial losses. These measures play a significant role in reducing the risk while doing online transactions. Like humans, machine learning algorithms learn from past transaction data and use that information to analyze future transactions with the same lens. While machines might not be as intelligent as humans are and might need some supervision on top of it, the advantage lies in the speed of data processing and computation. Also, machines can identify and remember more patterns in vast volumes of data compared to humans. Generally, these algorithms are known as anomaly detection. Let us delve into details in the next section.


# **Credit Card Fraud Detection using Machine Learning can be done using**

  1. **Unsupervised Learning** - 
    * Machine Learning Algorithms such as Isolation Forest, One-class SVM, LOF, etc., do not require labeled data for training the model. They identify patterns in the data and try to group the data points based on observed similarities in patterns. 

  2. **Supervised Learning**  
    * Machine Learning and Deep Learning Algorithms such as Ensemble Models (RandomForest, XGBoost, LightGBM, etc.), KNN, Neural Networks, Autoencoders, etc. These algorithms are trained on labeled data, and the model learns to predict the labels for the unseen data. Labeled data can be expensive to gather. 


# **Challenges in Credit Card Fraud Detection** 
  * The challenges involved in credit card fraud detection project is primarily the data itself. The data is heavily imbalanced, i.e., the count of data labeled as fraudulent is way less than the data labeled as non-fraudulent data. This makes it extremely tricky to train the model as it tends to overfit for the majority class and underfit for the minority class. Techniques like oversampling, undersampling, cost-sensitive learning, etc. can be used to deal with this. The metrics used for the final model are different from standard evaluation metrics of accuracy, AUC-ROC, etc.

  * Another prevalent faced challenge is the quality and quantity of the data. The startups in the early stage do not have much user history data to train extensive models, which makes it difficult to train a robust fraud detection model. A temporary solution to this problem can be sourcing data from an external third party, like scores from credit bureaus. 


## **DATASET DESCRIPTION**
* The dataset contains 284,807 transactions among which there are 492 i.e., 0.172% transactions are fraudulent transactions
* It also contains transactions made by a cardholder in 2 days in month of september 2013 
* This dataset is highly unbalanced. Due to security reasons, most of the features in the dataset are transformed using principal component analysis (PCA). V1, V2, V3,…, V28 are PCA applied features and rest features include ‘time’, ‘amount’ and ‘class’ are non-PCA applied features

## **Table of Contents**
1. Importing dependencies
2. Exploratory data analysis
3. Splitting the data into train & test data
4. Model Building
   * Perform cross validation with RepeatedKFold
   * Perform cross validation with StratifiedKFold
   * RandomOverSampler with StratifiedKFold Cross Validation
   * Oversampling with SMOTE Oversampling
   * Oversampling with ADASYN Oversampling
5. Hyperparameter Tuning
6. Conclusion