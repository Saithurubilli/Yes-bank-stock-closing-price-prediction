# Yes-bank-stock-closing-price-prediction
# Yes-bank-stock-closing-price-prediction
![image](https://user-images.githubusercontent.com/107321295/196026341-df6f6b0f-b15f-43fe-a9ae-08015bb79350.png)

Problem Statement
--------------------------------------------------
Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock’s closing price of the month.

Project Approach
--------------------------------------------------
Aim is to Perform regression analysis using multiple models and predict the closing price of the stock and in the end will compare the evaluation metrics for all different models to find the best model.
Below steps has followed.

* Initiate with data overview, to understand the dataset and in order to inspect how the dataset is for working.
* Visualizations makes things easier so, performed exploratory data analysis in order to understand data distribution and relation with dependent variable.
* Used log transformation as our variavles are positively skewd in nature .
* Checked for multicollinearity to check if the features are depedent or independent of each other.
* Splitted the dataset into training and testing data (80% of the data is used for training & 20% of the data is being used for testing).
* Model optimization using the following algorithms:
  1. Linear Regression
  2. Ridge Regession
  3. Lasso Regression
  4. K Nearest Neighbours (KNN)
  5. XG-Boost
  
Compared model performance using different evaluation metrics in order to get the best performing model.

Model Evaluation
--------------------------------------------------
All the models are evaluated on the basis of following evaluation metrics

![image](https://user-images.githubusercontent.com/107321295/196026495-6a280810-6cda-414c-82f6-217841344313.png)

Conclusion
--------------------------------------------------
* All the input variables are highly contributing for output prediction.
* The accuracy score for each model is more than 95%.
* Linear Regression has given the best results with lowest MSE and RMSE and highest R-square value scores out of other three algorithms beacause of linear relation of   dataset.
* KNN and XG Boost not performed well with high MSE and RMSE score.
* We see lasso with low performance beacause it penalizes the coefficient and thus shrinks them to zero. whereas in this case all the features were important for prediction purpose so, it ended up with poor results.
