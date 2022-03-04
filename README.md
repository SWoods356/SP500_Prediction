# SP500_Prediction


# Overview
This repository features EDA and prediction on the SP500 index. Adjusted closing prices were pulled from yahoo finance for ticker ^GSPC for the prior five years (March 2017 to March 2022)

# EDA and Preparation for Modeling

Historical close prices are plotted for the prior five years along with bollinger bands.

For LSTM model prep, 80% of data was split for training and 20% for testing. Adjusted close prices were min max transformed. Training data was formatted with a look back period of 60 days.

# Modeling - LSTM Recurrent Neural Networks

Two LSTM RNN models were used to fit and predict SP500 closing prices for the next 30 days. Both models had similar performance. The higher performing model achieved an RMSE of 66.58 on training data and 122.35 on testing data. 

30 day predictions for both models did not 

Predictions vs Actual:

![image](https://user-images.githubusercontent.com/85903905/156837602-c8c0150d-4746-412d-a363-2e0d3d68f89f.png)

Predictions for next 30 days:

![image](https://user-images.githubusercontent.com/85903905/156838092-50f072cf-ff4f-4161-96c5-e21e3a59041a.png)

