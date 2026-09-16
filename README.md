# SmartKart Customer Churn Prediction

## Description

An AI/ML project for SmartKart, an online retail company, that predicts which customers have a higher possibility of leaving the company. The project uses customer-related data to classify customers into **High, Medium, or Low churn risk** and can also provide a churn probability.

## Business Scenario

SmartKart is an online retail company experiencing several customer-related problems:

* Some customers are no longer purchasing.
* Marketing campaigns receive a low response.
* Customer complaints are increasing.
* Management does not know which customers require immediate attention.

To address these challenges, SmartKart wants to use AI to identify customers who may stop purchasing.

## Business Question

**Which customers have a higher possibility of leaving SmartKart?**

## Proposed AI Use Case

### Customer Churn Prediction

The proposed system uses machine learning to analyze customer information and predict the likelihood that a customer may stop purchasing from SmartKart.

The prediction can help the business identify customers who may require additional attention or retention activities.

## Expected AI Output

For each customer, the system can produce a churn-risk category:

| Risk Level        | Meaning                                               |
| ----------------- | ----------------------------------------------------- |
| High Churn Risk   | Customer has a relatively high probability of leaving |
| Medium Churn Risk | Customer shows a moderate possibility of leaving      |
| Low Churn Risk    | Customer has a relatively low possibility of leaving  |

The system may also present the result as a probability.

Example:

```text
Customer C102: 78% probability of churn
Risk Level: High
```

> **Note:** The 78% value above is only an example of the expected output format. It is not an actual model result.

## Machine Learning Approach

A classification-based machine learning model can be used for customer churn prediction.

The general workflow is:

1. Collect customer data.
2. Clean and prepare the data.
3. Select relevant customer features.
4. Split the data into training and testing sets.
5. Train a classification model.
6. Evaluate model performance.
7. Generate churn probabilities.
8. Convert probabilities into risk categories.
9. Use the results to support customer-retention decisions.

## Possible Customer Features

Depending on the available SmartKart dataset, useful features may include:

* Customer purchase frequency
* Recency of last purchase
* Total purchase value
* Number of orders
* Average order value
* Customer complaints
* Marketing campaign response
* Customer tenure
* Website/app activity
* Payment-related issues

## Example Output

```text
Customer ID    Churn Probability    Risk Level
C101           0.18                 Low
C102           0.78                 High
C103           0.46                 Medium
C104           0.12                 Low
```

## Business Benefits

Customer churn prediction could help SmartKart:

* Identify customers who may leave.
* Prioritize customers requiring attention.
* Improve customer-retention activities.
* Create more targeted marketing campaigns.
* Investigate customers with increasing complaints.
* Reduce unnecessary marketing spending.
* Support data-driven customer-management decisions.

## Project Structure

```text
smartkart-customer-churn-prediction/
│
├── data/
│   └── customer_data.csv
│
├── notebooks/
│   └── smartkart_churn_prediction.ipynb
│
├── src/
│   └── churn_prediction.py
│
├── README.md
└── requirements.txt
```

## Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

## Model Evaluation

The model should be evaluated using appropriate classification metrics such as:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC-AUC, where appropriate

For churn prediction, **precision and recall should also be considered**, because identifying customers who may leave is generally more useful than relying on accuracy alone.

## Important Note

The example churn probability in this README is illustrative only. Actual probabilities and risk classifications should be generated from the trained SmartKart model and evaluated using the project's test data.

The model's predictions should be treated as decision-support information rather than certainty that a customer will leave.

## Future Improvements

Possible future improvements include:

* Testing multiple machine learning algorithms.
* Hyperparameter tuning.
* Using customer purchase-history data.
* Adding customer complaint information.
* Adding marketing-response data.
* Creating a customer-risk dashboard.
* Monitoring model performance over time.
* Retraining the model with new customer data.
* Developing automated retention recommendations.

## Conclusion

The SmartKart Customer Churn Prediction project demonstrates how AI and machine learning can be used to identify customers who may be at risk of leaving. By converting customer data into churn probabilities and risk categories, SmartKart can better prioritize customer-retention efforts and support data-driven decision-making.
