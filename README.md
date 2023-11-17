# Module 12 Report Template

## Overview of the Analysis
The aim of this analysis is to assess the effectiveness of two logistic regression machine learning models in anticipating credit risk associated with loans. The evaluation was performed on financial data, with a particular emphasis on variables such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The primary goal was to forecast the loan status, categorizing it as either a healthy loan (0) or a high-risk loan (1).

The machine learning process in this analysis involved the following stages:

1. **Data Splitting:**
   Dividing the dataset into training and testing sets.

2. **Logistic Regression Model (Original Data):**
   Developing and training a logistic regression model using the original dataset.

3. **Model Evaluation (Original Model):**
   Assessing the performance of the original model using metrics such as accuracy, precision, and recall.

4. **Data Resampling (RandomOverSampler):**
   Addressing class imbalance by resampling the data using the RandomOverSampler technique.

5. **Logistic Regression Model (Resampled Data):**
   Constructing and training another logistic regression model using the resampled dataset.

6. **Model Evaluation (Resampled Model):**
   Evaluating the performance of the resampled model using the same metrics as before.

## Results

 ## Machine Learning Model 1:

 * Model 1, trained on the original data, demonstrates an impressive overall accuracy of 94.4% in classifying the two labels. It excels in predicting healthy loans, achieving perfect precision and recall scores of 1.00. However, there is room for improvement in predicting high-risk loans. The precision score for high-risk loans stands at 0.87, implying that only 87% of identified high-risk loans were accurate. Additionally, the recall score for high-risk loans is 0.89, indicating that the model captured only 89% of all high-risk loans in the dataset.

## Machine Learning Model 2:

  * Model 2, trained on the resampled data, attains an impressive accuracy of 99.6% in accurately classifying the two labels. The model excels in predicting healthy loans, achieving perfect precision and recall scores of 1.00. While the precision score for high-risk loans remains at 0.87, indicating 87% accuracy in identification, the recall score has notably improved to 1.00. This enhancement suggests that the model can now successfully identify all high-risk loans in the dataset.

## Summary

Based on the findings, the logistic regression model trained with resampled data (Model 2) performs better than the model trained with the original data (Model 1), particularly in the accurate prediction of high-risk loans. Model 2 exhibits superior precision and recall scores for high-risk loans, which is important in minimizing potential financial losses for the lending company.

I recommend the adoption of the logistic regression model trained with resampled data (Model 2) for credit risk analysis. Its substantial improvement in predicting high-risk loans compared to the original model positions it as a valuable tool for the company. Utilizing this model will enhance the company's ability to assess loan applications, enabling more informed decisions when approving or rejecting loans and thereby effectively mitigating credit risk.
