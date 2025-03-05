# SyriaTel Customer Churn Prediction

## Business Problem
SyriaTel is experiencing customer churn, which negatively impacts revenue and profitability. The goal of this project is to develop a predictive model that identifies customers likely to leave, enabling targeted retention strategies such as personalized offers and service improvements to enhance customer loyalty.

## Dataset Overview
The dataset consists of various features such as call minutes, customer service calls, charge amounts, and service plan details. The target variable is **churn**, which indicates whether a customer leaves the service.

## Models Used & Performance Comparison
We tested multiple machine learning models to predict customer churn:

| Model              | Accuracy  | Precision (Churn) | Recall (Churn) | F1-score (Churn) |
|--------------------|----------|------------------|---------------|----------------|
| Logistic Regression | 87.5%    | 0.61             | 0.39          | 0.48           |
| Random Forest      | 95.6%    | 1.00             | 0.70          | 0.82           |
| Gradient Boosting  | 96.4%    | 0.94             | 0.80          | 0.87           |

From the above results, **Gradient Boosting** performed the best, with **96.4% accuracy** and the highest recall for predicting churned customers.

## **Key Findings & Feature Importance**
Feature importance analysis from the Gradient Boosting model revealed that the following features had the most impact on churn prediction:

- **Total charge**: The most important factor affecting churn.
- **Customer service calls**: More complaints correlate with higher churn likelihood.
- **International plan**: Customers with an international plan are more prone to churn.
- **Voice mail plan**: Affects churn probability.
- **Total minutes & messages**: Usage patterns impact customer retention.

## **Customer Segmentation**
To better understand churn risk, we segmented customers into three risk levels:

| Churn Risk | Number of Customers |
|------------|---------------------|
| High Risk  | 1,932               |
| Medium Risk | 1,081               |
| Low Risk   | 320                 |

This segmentation allows SyriaTel to focus retention efforts on **High Risk** customers by offering incentives, improved customer support, and personalized offers.

## **Conclusion & Recommendations**
- **Monitor High-Risk Customers**: Implement proactive retention strategies for high-risk segments.
- **Improve Customer Service**: Since service complaints correlate with churn, enhancing customer support may improve retention.
- **Incentives for Loyal Customers**: Provide offers and discounts to customers showing churn behavior.
- **Data-Driven Marketing**: Use predictive insights to create personalized retention campaigns.


This project provides a valuable framework for predicting and reducing customer churn at SyriaTel. 

