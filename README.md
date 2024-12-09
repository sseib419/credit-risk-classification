# credit-risk-classification

To train a model to predict loan risk, first the credit card csv was imported and it was divided into training and testing sets, with the loan status being the label and the rest of the columns being the features. The testing and training data for both the label and the features were then split using the module train_test_split, and a logistic regression model was created using the training data. A confusion matrix was generated as well as a classification report. 

The purpose of the analysis is to be able to see how accurate our logistic regression model is at predicting whether a loan will be a healthy loan or a high-risk loan given the data, and hopefully if the model is good enough, we can input new data and we can trust that the model will give us accurate results in predicting whether a loan is healthy or high risk.

Healthy loans:
• 100% precision
• 99% recall
• 99% accuracy

High Risk loans:
• 84% precision
• 95% recall
• 99% accuracy 

From the classification report, it can be seen that when predicting the healthy loans the results are a lot more precise, which could be due to the fact that there are a lot more healthy loans in the data set compared to high risk loans, so the model may have a harder time predicting the high risk loans. Another reason could be that high risk loans may have more  variability in their features, which would make them harder to predict. 

With the high risk loans, the model may incorrectly flag some healthy loans as high risk ones. This model would be good if situations where missing a high risk loan is far worse than labeling a healthy loan as high risk. In my opinion, I would rather flag healthy loans as high risk loans more often than missing more high risk loans, so I would recommend this model to be used by the company.
