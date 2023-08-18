Credit Risk Analysis
-------------------------------------------------
Overview of the Analysis
-------------------------------------------------
The purpose of this was to assess the effiency of the two logistic regression machine learning models to forsee the credit risk linked to loans. The evauluation centers on financial data, concentrating on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective was to predict the loan status, either as a healthy loan (0) or high-risk loan (1).

The stages of the machine learning process in this analysis included:

    - Splitting the data into training and testing datasets
    - Creating and fitting a logistic regression model with the original data
    - Evaluating the model's performance using accuracy, precision, and  recall scores
    - Resampling the data using RandomOverSampler to address class imbalance
    - Creating and fitting another logistic regression model with the resampled data
    - Evaluating the performance of the resampled model using the same metrics

Methods used in this analysis include LogisticRegression and RandomOverSampler for resampling.

-------------------------------------------------
Results
-------------------------------------------------
    Model 1: Logistic Regression with Original Data


    - Accuracy : The overall accuracy of the model is .944, indicating it can correctly classify 94.4% of the instances


    - Precision Score : The model was 100% precise with healthy loans, though the model was only 87% precise in predicting high-risk loans 

    - Recall : The model had 100% recall in predicting healthy loans, but 89% recall in predicting high-risk loans


    Model 2 : Logistic Regression with Resampled Data

    - Accuracy : The overall accuracy of the model is .994, indicating it can correctly classify 99.4% of the instances


    - Precision Score : The model was 99% precise in prediciting both healthy loans and high-risk loans 

    - Recall : The model was 99% recall in prediciting both healthy loans and high-risk loans 

-------------------------------------------------
Summary
-------------------------------------------------
Based on the findings, the logistic regression model developed with resampled data (Model 2) outperforms the model created using the original data (Model 1), particularly in its ability to predict high-risk loans. Model 2 showcases notably elevated precision and recall scores for high-risk loans, a pivotal factor in minimizing potential financial losses for the lending institution.

It is strongly advised to leverage the logistic regression model trained with resampled data (Model 2) for the purpose of credit risk analysis. This choice is justified by its substantial enhancement in accurately predicting high-risk loans when compared to the original model. By employing this model, the company can effectively evaluate loan applications and make well-informed choices during the loan approval process, thereby effectively mitigating credit risk.