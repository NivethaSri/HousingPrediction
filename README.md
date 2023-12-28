# House Price Prediction

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
Which variables are significant in predicting the price of a house, and
How well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression.




## General Information
BUSINESS GOALS
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Conclusions
    Features    Linear    Ridge    Lasso
0    r2_train    9.089000e-01    0.9075    0.9039
1    r2_test    -3.157214e+23    0.8800    0.8839
2    rss_train    1.546900e+00    1.5709    1.6318
3    rss_test    2.417095e+24    0.9186    0.8885
4    mse_train    1.500000e-03    0.0015    0.0016
5    mse_test    5.505911e+21    0.0021    0.0020
6    rmse_train    3.890000e-02    0.0392    0.0400
7    rmse_test    7.420182e+10    0.0457    0.0450

By considering the matrices we come to the conclution that Lasso and Ridge is better compered to Linear.

Thr r-sq is also good in both Lasso and RIdge. But the coeff are near to 0 in Lasso . So we are considering Lasso regression for this model.


The list of top 5 features are

    GrLivArea    
    OverallQual    
    OverallCond    
    GarageCars    
    MSZoning_RH




## Technologies Used
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.preprocessing import MinMaxScaler
from sklearn.model_selection import train_test_split, GridSearchCV
from sklearn.feature_selection import RFE
from sklearn.metrics import mean_squared_error, r2_score
from sklearn.linear_model import LinearRegression , Ridge, Lasso






## Contact
Created by niviinfotechs@gmail.com - feel free to contact me!

