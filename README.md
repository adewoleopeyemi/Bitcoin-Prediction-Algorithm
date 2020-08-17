### Bitcoin-Prediction-Algorithm
In this notebook i plan on predicting the price of bitcoin by using the value  of the past 60 days as an input. This is done with stacked Bidrectional LSTM layers,  the features taken into account are

- txVolume
- Adjusted txVolume(USD)
- Exchange Volume(USD)
- Active Addresses 
- Generated Coins
- Fees
- Average Difficulty
- Median TxValue
- Median Fee
- Block Size
- Block Count



To judge the result of the model we evaluate the following
* The rate at which the model predicts the prices change versus the real rate at which the prices actually change
* A binary price which defalts to a value of 1, if the difference between the predicted price and the actual price is > 0, else the value is 0
* We calculate the mean squared error 
* We also calculate the precision of the model

