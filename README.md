# Predict-Customer-Purchase-Behaviour-Project
Background

Understanding customer purchase behavior is crucial for businesses to tailor their marketing strategies and improve sales. This project aims to predict whether a customer will make a purchase based on various demographic and behavioral attributes. By leveraging machine learning techniques, we can gain insights into the factors influencing purchase decisions and help businesses target their efforts more effectively.
Dataset Description

The dataset used in this project is sourced from Kaggle and contains information on customer purchase behavior across various attributes. The dataset includes demographic information, purchasing habits, and other relevant features.

Features:

  Age: Customer's age
  Gender: Customer's gender (0: Male, 1: Female)
  Annual Income: Annual income of the customer in dollars
  Number of Purchases: Total number of purchases made by the customer
  Product Category: Category of the purchased product (0: Electronics, 1: Clothing, 2: Home Goods, 3: Beauty, 4: Sports)
  Time Spent on Website: Time spent by the customer on the website in minutes
  Loyalty Program: Whether the customer is a member of the loyalty program (0: No, 1: Yes)
  Discounts Availed: Number of discounts availed by the customer (range: 0-5)
  PurchaseStatus (Target Variable): Likelihood of the customer making a purchase (0: No, 1: Yes)

Target Variable Distribution:

  0 (No Purchase): 48%
  1 (Purchase): 52%

The dataset can be found at this https://www.kaggle.com/datasets/rabieelkharoua/predict-customer-purchase-behavior-dataset?resource=download.

# Aim and Objectives
# Aim

The primary aim of this project is to develop and evaluate machine learning models to predict customer purchase behavior. The project seeks to identify the most effective model in terms of accuracy, precision, recall, and F1-score.
Objectives

    
Develop and define the architecture for various machine learning models.
Train the models using the training dataset and validate their performance.
Evaluate the models using various metrics, including accuracy, precision, recall, and F1-score.
Compare the performance of the models to identify the best one for deployment.
# Data Exploration

During the data exploration phase, we analyzed the relationships between various attributes and the target variable, PurchaseStatus. Here are the key findings:

Positively Correlated Variables:
  AnnualIncome: Higher annual income is associated with a higher likelihood of making a purchase.
  NumberOfPurchases: Customers with a higher number of past purchases are more likely to make a purchase.
  TimeSpentOnWebsite: Increased time spent on the website correlates with a higher likelihood of purchase.
  LoyaltyProgram: Customers enrolled in the loyalty program are more likely to make a purchase.
  DiscountsAvailed: Customers who availed more discounts are more likely to make a purchase.

Negatively Correlated Variable:
Age: Older customers are less likely to make a purchase compared to younger customers.

Histograms:
NumberOfPurchases: The histogram shows that customers with fewer past purchases are less likely to make a purchase.
Age: Younger customers, particularly those aged 20 to 40 years, are more likely to make a purchase than those aged 40 and older.
Product Category and Gender: The ratios of customers likely to make a purchase are consistent across different product categories and genders.


# Model Development and Evaluation
## Models

We will develop and evaluate multiple models, including:

Logistic Regression,
Random Forest,
K-Nearest Neighbors (KNN),
Support Vector Machine (SVM), and
Deep Learning Model (using TensorFlow/Keras)

## Evaluation Metrics

The models will be evaluated using the following metrics:

Accuracy: The proportion of correctly predicted instances out of the total instances.
Precision: The proportion of true positive predictions out of the total positive predictions.
Recall: The proportion of true positive predictions out of the total actual positive instances.
F1-Score: The harmonic mean of precision and recall.

## Results

### Model Performance
We evaluated several machine learning models to predict customer purchase behavior. The following table summarizes the accuracy of each model:

| Model                    | Accuracy |
|--------------------------|----------|
| Logistic Regression      | 70%      |
| Random Forest            | 94%      |
| K-Nearest Neighbors (KNN)| 59%      |
| Support Vector Machine   | 62%      |
| Deep Learning Model      | 61%      |

### Key Findings
- The **Random Forest** model outperformed all other models with an accuracy of **94%**.
- The deep learning model and KNN model had the lowest accuracy, suggesting that simpler models might be more effective for this dataset.
- Factors such as **Annual Income**, **Time Spent on Website**, and **Number of Purchases** were significant in influencing the likelihood of a purchase.



## Conclusion
The results indicate that the Random Forest model is the most effective in predicting customer purchase behavior. These insights can help businesses tailor their marketing strategies and improve sales targeting.


