# Sales-Revenue-Prediction

LSTM model to estimate the sales income of any company or organisation. The purpose of this project is to be able to forecast future sales for any corporation, which will have a substantial impact on the company's profit. Second, it can be used to create plans. Forecasts help us organise our demand and supply activities. It helps to determine where extra investment should be placed. The most difficult task in this project was determining which model to employ for training and testing. We initially used CNN, but it created a lot of inaccuracies. Next, we attempted to forecast the model using a standard feed forward neural network, however the model's accuracy was significantly worse.
We then tested the LSTM (Long Short-Term Memory) model instead of CNN/ANN, and it addressed our difficulties. The implementation of our concept will involve three essential phases.

Data wrangling is purifying or cleaning the data so that our model can readily access it.
Data transformation - To anticipate sales more precisely and simply (i.e. with no mistakes), we shall do: - Determine if the data is stationary (constant). If there is a rising or declining trend, create a new data frame to make it constant.
Finally, because our data is time series, the LSTM model will require our feature set to be supervised, necessitating the conversion of time series to supervised data. 3. Finally, we'll scale the data to normalise it for training and testing.

We employed supervised machine learning for this training. LSTM may be used as both a supervised (classification, sequence prediction) and unsupervised (autoencoder) method, depending on the loss function it optimises for. In this project, we use supervised learning to train our LSTM model. 
The primary reason for using the LSTM model is that it is difficult to use sequenced data as input to a supervised learning model like CNNs or other models. Our objective is to forecast monthly sales. We need to aggregate our data at the monthly level and then total the sales column to get the monthly sales. We next displayed the data to see if it showed an increasing or declining trend. After charting, it is clear that our data is not stationary. To make our data steady, we used several trial-and-error procedures.
The one that offered us the solution we required was to calculate the difference between current and prior sales, i.e. sales from the previous month.
