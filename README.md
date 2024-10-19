# Life-Expectancy-Prediction
Life Expectancy Prediction using Machine Learning Bagging

The dataset contains information about health, immunization, economics, demographic information, and life expectancy of lots of region and country.

The purpose of the code is to build a mode, that is able to predict life expectancy based on the information given from the dataset.

The dataset itself contains a lot of outlier, so that consideration has to be made when using methods, encoding, and scaling.

# Methods
Bagging will be the methods used inside the machine learning model, because it can help to reduce variance and improve overall performance of the model itself, it's also robust to outliers.

Then, for the categorical variable, will be encoded using 2 methods, Frequency Encoding and Target Encoding, and then will be putted inside the bagging model.

Then, seeing at the outlier and variance, a Robust Scaler will be used to help maximizing the model's performance.

# Evaluation
For the evaluation of the encoding, will be using MAE, MSE, and R Squared Test. The method that is able to result a smaller MAE and MSE, and the highest R Squared will be chosen as the final encoding method. A prediction graph will also be used to map and see how the model performance is.

# Conclusion
After trying 2 different encoding method, Target Encoding is better than Frequency Encoding, seeing from the evaluation of MSE, MAE, and R Squared.
Then, scaling is not really important for the model, because the MAE, MSE, and R Squared is not significantly increasing.

# Comparison
1. Bagging using Frequency Encoding
**Train**
-> MAE:0.179
-> MSE: 0.079
-> R Squared: 0.999
**Test**
-> MAE:0.484
-> MSE: 0.426
-> R Squared: 0.995

2. Bagging using Target Encoding
**Train**
-> MAE:0.156
-> MSE: 0.062
-> R Squared: 0.999
**Test**
-> MAE:0.36
-> MSE: 0.272
-> R Squared: 0.997

3. Bagging & Scaling using Robust Scaler
**Train**
-> MAE:0.152
-> MSE: 0.059
-> R Squared: 0.999
**Test**
-> MAE:0.339
-> MSE: 0.247
-> R Squared: 0.997
