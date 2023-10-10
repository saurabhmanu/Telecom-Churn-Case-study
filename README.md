# Telecom-Churn-Case-studyWe can take the following suggestive steps to build the model:
Preprocess data (convert columns to appropriate formats, handle missing values, etc.)
Conduct appropriate exploratory analysis to extract useful insights (whether directly useful for business or for eventual modelling/feature engineering).
Derive new features.
Reduce the number of variables using PCA.
Train a variety of models, tune model hyperparameters, etc. (handle class imbalance using appropriate techniques).
Evaluate the models using appropriate evaluation metrics. Note that it is more important to identify churners than the non-churners accurately - choose an appropriate evaluation metric which reflects this business goal.
Finally, choose a model based on some evaluation metric.
The above model will only be able to achieve one of the two goals - to predict customers who will churn. We can’t use the above model to identify the important features for churn. That’s because PCA usually creates components which are not easy to interpret.
Therefore, we will build another model with the main objective of identifying important predictor attributes which help the business understand indicators of churn. A good choice to identify important variables is a logistic regression model or a model from the tree family. In case of logistic regression, we will make sure to handle multi-collinearity.
After identifying important predictors, display them visually - we can use plots, summary tables etc. - whatever we think best conveys the importance of features.
Finally, recommend strategies to manage customer churn based on our observations.
Note:
Note that the best parameters procuded the accuracy of 91% which is not significantly deterred than the accuracy of original random forest, which is pegged around 92%
Conclusion :
The best model to predict the churn is observed to be Random Forest based on the accuracy as performance measure.
The incoming calls (with local same operator mobile/other operator mobile/fixed lines, STD or Special) plays a vital role in understanding the possibility of churn. Hence, the operator should focus on incoming calls data and has to provide some kind of special offers to the customers whose incoming calls turning lower.
Details:
After cleaning the data, we broadly employed three models as mentioned below including some variations within these models in order to arrive at the best model in each of the cases.
Logistic Regression :
Logistic Regression with RFE Logistic regression with PCA Random Forest For each of these models, the summary of performance measures are as follows:

Logistic Regression
. Train Accuracy : ~79%
. Test Accuracy : ~80%

Logistic regression with PCA
. Train Accuracy : ~91%
. Test Accuracy : ~92%

Decision Tree with PCA:
. Train Accuracy : ~93%
. Test Accuracy : ~92%

Random Forest with PCA:
. Train Accuracy :~ 91%
. Test Accuracy :~ 92%
