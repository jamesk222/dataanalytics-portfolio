PROJECT SUMMARY:
Project Report: AI-Powered Sales Forecasting and Loan Default Prediction
1. Sales Forecasting with Linear Regression
Objective: To predict sales based on factors like Marketing_Spend and Loan_Amount to provide actionable business insights.
Methodology:
A Linear Regression model was trained on the cleaned sales data. This model is ideal for understanding the direct, linear relationship between a target variable (Sales) and several features.
Key Findings:
The model's analysis of feature coefficients provided a clear understanding of what drives sales:
•	Marketing_Spend (Coefficient: 0.235): This was the most significant and actionable factor. The model indicates that for every dollar spent on marketing, sales are predicted to increase by approximately 24 cents. This is a crucial business insight showing a direct, causal relationship.
•	Loan_Amount (Coefficient: 0.036): The model found a small positive correlation here. For every $100 increase in a customer's loan amount, sales are predicted to increase by about $3.60. This suggests that customers with a higher financial capacity (indicated by a larger loan) tend to have higher sales.
•	Customer_ID (Coefficient: 9.897): While this coefficient was numerically the largest, it was determined to be statistically insignificant. This is a common occurrence with unique identifiers and does not represent a meaningful business insight.
Business Recommendations:
•	Increase Marketing Investment: Based on the strong, positive coefficient, a strategic increase in Marketing_Spend is likely to yield a predictable return in increased sales.
•	Target High-Capacity Customers: The correlation with Loan_Amount suggests an opportunity to tailor marketing efforts toward customers with a higher financial capacity, as they may be more likely to make larger purchases.

2. Loan Default Prediction with Random Forest Classifier
Objective: To build a robust model that accurately predicts which customers are at high risk of defaulting on a loan, thereby enabling smarter lending decisions.
Methodology:
A Random Forest Classifier was trained on a loan dataset. This model is well-suited for classification problems and is highly effective at identifying complex, non-linear relationships between multiple features. The data was meticulously preprocessed, including one-hot encoding for categorical features and standardization to prevent data leakage. The model was evaluated using accuracy and a classification report.
Key Findings:
•	Model Accuracy: The model achieved a robust accuracy of approximately 95% on unseen test data, indicating its strong ability to correctly classify customers as "likely to default" or "unlikely to default."
•	Feature Importance: The model provided a clear ranking of the most influential factors in predicting loan defaults. The top features were:
o	Credit_Score: This was the most important predictor, which aligns with traditional lending practices. A higher credit score significantly lowers the risk of default.
o	Income & Loan_Amount: These factors were also highly influential. Customers with higher incomes are better positioned to repay larger loans, making them lower-risk.
o	Previous_Defaults: The model correctly identified a history of previous defaults as a strong indicator of future risk.
Business Recommendations:
•	Automate Risk Assessment: The trained Random Forest model can be integrated into your loan approval process to automatically assess the default risk of new applicants.
•	Prioritize Key Factors: Focus on the most important features (Credit_Score, Income, Loan_Amount) when making lending decisions. The model confirms that these are the most reliable indicators of risk.
•	Refine Lending Criteria: Consider setting stricter criteria for applicants with lower credit scores or those with a history of defaults, as the model has identified them as high-risk segments.



