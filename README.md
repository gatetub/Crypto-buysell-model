# Crypto-buysell-model
We have developed an algorithmic trading model which utilizes a machine learning algorithm, long short-term memory network (LSTM), to predict closing prices, and then utilizes the technique of mean reversion to algorithmically trade and generate returns of 143 percent.

LSTM Model

Long short term memory network was used to predict the closing prices of the time series of BTC/USDT using the dataset at 5 minute intervals. 

The dataset was transformed into a range of (0,1) using MinMaxScaler from Sci-Kit Learn library. Then, training and testing sets were formed by splitting the dataset into a ratio of 80:20. 
The LSTM model is composed of three layers: the first layer, a dense layer and an activation layer. The lookback period (backcandles was set to be 30) and the scaled input was transformed into the shape of (30,4) and fed into the LSTM. Additionally, the model was optimized with Adam optimizer.
Finally, the testing and prediction results are plotted in a line chart.
