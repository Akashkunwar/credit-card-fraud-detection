<center><img src="https://raw.githubusercontent.com/Akashkunwar/credit-card-fraud-detection/main/images/credit%20card.png"></center><br>

# Credit Card Frauds Detection by using Machine Learning
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

In this project, I'll use **scikit-learn**, **XG-Boost** and many more library to prediction model that can tell or detect when transaction is deriving from fraud or a genuine purchase. Here i will compare between some of the most famous machone learning algorithem which are uses in classification.

<center><img src="https://raw.githubusercontent.com/Akashkunwar/credit-card-fraud-detection/main/images/download.png"></center><br>
Interpretation:- 

Here as we can see the distribution of data in all the columns are mixed some columns are normally distributed and some are not in most of the cases and in very few column seems normally distributed data and most column has skewed data. Means data is imbalanced.

<center><img src="https://github.com/Akashkunwar/credit-card-fraud-detection/blob/main/images/download%20(1).png"></center><br>
**75%** of transactions in the analyzed period were **up to €77.16**.<br><br>
The **maximum amount** identified during this period was **€25,691.16**, way higher than the **average amount of €88.35**.

<center><img src="https://raw.githubusercontent.com/Akashkunwar/credit-card-fraud-detection/main/images/download%20(2).png"></center><br>
It looks like most transactions are genuine, represented by the **blue** dots on the chart above. We can also see that all high value transactions were genuine, with apparently **no fraudulent** transaction made being **above €5,000.00**<br><br>
However, it seems hard to identify the fraudulent transactions, painted **yelow**, looking at the distribution of **amount values**. This leaves us with a question: **How many transactions were in fact fraud?**

<center><img src="https://raw.githubusercontent.com/Akashkunwar/credit-card-fraud-detection/main/images/download%20(3).png"></center><br>
So it seems **only 492** transactions in the dataset were **fraudulent** which represents **only 0.173%** of data, there is a **huge class imbalance** that we have to work on here!


Considering we have **155 fraudulent transactions** in our testing set, and the **goal of our model is predicting these fraudulent transactions**, we can realize that the model which **best performed such task** was the **xgboost** model which predicted **145 fraudulent transactions out of 155**, with a **96.17% of AUROC Score**, the highest one of all the models tested, which indicates **how well our model detects fradulent transactions from our testing set**.

## Conclusion

In this project, my goal is to **detect all the fraudulent transactions**, best suited model for this task is **xgboost** with a **AUROC score of 96.172%**, which is considered as most supperior matric for classification problem. That correctly detect 145 fraudulent transactions out of 155. When we work with a **machine learning model** we must always know for a fact what it is that we're trying to get from that model.<br><br> Considering we have **155 fraudulent transactions** in our testing set, and the **goal of our model is predicting these fraudulent transactions**, we can realize that the model which **best performed such task** was the **xgboost** model which predicted **145 fraudulent transactions out of 155**, with a **96.17% of AUROC Score**, the highest one of all the models tested, which indicates **how well our model detects fradulent transactions from our testing set**.<br> 
This model can firther be improved by testing all the parameters and trying to find more suitable splittion, imbalanced learning and machine learning technique if available in public domain.
<br><br>
See notebook on:<br>
Kaggle : https://www.kaggle.com/code/kunwarakash/eda-and-model-training-with-auroc-score-of-96-1 <br><br>
Deepnote : https://deepnote.com/@akashkunwar/https://deepnote.com/workspace/akashkunwar-24eb70be-4d95-4113-b8f0-3fa2332b09c7/project/Credit-card-fraud-detection-ba0c37d8-ec4c-4988-adfb-1c7e2a18e87b/notebook/Credit_Card_Fraud_Detection-20220830-021227-3b55e273b6d64e72a68f386bc2980f8b <br><br>
My Github reposatory of this project : https://github.com/Akashkunwar/credit-card-fraud-detection

Thanks...

