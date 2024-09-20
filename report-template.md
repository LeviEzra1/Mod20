# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

* The purpose of the analysis
    * To find high risk and healthy risks of financial loans
* Finacial information 
    * Was based on the creditworthiness of borrowers
* Basic info


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
        * Accuracy = .99
        * Precision = .87
        * Recall .89
    
* Machine Learning Model 0:
    * Description of Model 0 Accuracy, Precision, and Recall scores.
        * Accuracy = .99
        * precision = 1.00
        * Recall = 1.00
    


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The logistic regression model is performing exceptionally well in predicting healthy loans (class 0), with a precision of 1.00 and recall of 0.99. However, while the model also shows good performance in identifying risky loans (class 1), the precision is slightly lower at 0.87, and the recall is 0.89.

This reduced precision and recall for risky loans may be due to the imbalanced nature of the dataset. The support for class 1 in the test data is only 625, which is quite low compared to 18,759 for class 0. This imbalance indicates that the model has fewer examples of high-risk loans to learn from, which could hinder its ability to accurately predict them. Enhancing the dataset by including more high-risk loans for training might improve the model's performance.

In the context of loan classification, accurately identifying high-risk loans is crucial, as the financial loss from a loan defaulting can far outweigh the potential interest earned from a healthy loan. Although the overall accuracy of the model is high at 99%, there's still room for improvement in detecting high-risk loans, which could be critical in minimizing financial risk.
