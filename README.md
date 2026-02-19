# Customer-Churn-Prediction

## Customer Churn Prediction with Logistic Regression

## Executive Summary

Predicting who’s leaving before they leave. This project turns raw customer data into actionable insights, helping businesses retain high-value customers by flagging churn risk early. Simple, interpretable, and tuned for real-world impact.

## Business Problem

Customer churn directly impacts revenue and growth. Businesses need an early-warning system to flag customers likely to churn so retention efforts can be deployed effectively.

## Objective

Build a binary classification model using logistic regression to predict churn.

Tune the decision threshold to balance recall (catching churners) and precision (avoiding unnecessary retention actions).

## Approach

Data Preparation – Cleaned, processed, and encoded customer behavioral and demographic data.

Modeling – Logistic regression was chosen for its interpretability and efficiency.

Threshold Tuning – Adjusted decision threshold to maximize recall while keeping precision reasonable.

## Key Decisions

Chosen Threshold: 0.4

Reasoning: Captures ~79% of churners while maintaining a practical balance between coverage and operational cost.

## Trade-Offs

Lowering the threshold → higher recall, more false positives.

Increasing the threshold → higher precision, more missed churners.

Business priority: Minimize lost customers, even at the cost of some false alarms.

## Recommendation

Treat the model as a churn-risk flagging system, not a final decision-maker.

Customers flagged with a churn probability ≥ 0.4 should be prioritized for retention actions such as:

Targeted offers

Service quality checks

Proactive customer support

## Results

Logistic regression effectively predicts churn while remaining interpretable.

Decision threshold tuning aligns predictions with business priorities, emphasizing recall over precision to reduce revenue loss.

## Takeaways

Early identification of churners allows proactive retention.

Threshold tuning is critical: recall is more valuable than precision in customer retention contexts.

Logistic regression remains a strong baseline for churn prediction thanks to its transparency and actionable insights.

## Tech Stack

Python: Pandas, NumPy, Scikit-learn

Visualization: Seaborn, Matplotlib
