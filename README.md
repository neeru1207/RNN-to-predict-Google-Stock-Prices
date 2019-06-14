# RNN-to-predict-Google-Stock-Prices
A RNN coded in python using the Keras deep learning library to predict Google Stock prices.
## Dataset
The dataset contains high, low and open values of Google stock prices.
I chose the open values for the prediction instead of the high and low values.
## Architecture
The architecture of the RNN is 4 sets of LSTM (Long short term memory) layers and Dropout regularization layers.
The number of time steps chosen for the RNN is 60.
The model is trained on 100 epochs with a batch size of 32. The optimizer used is adam and the loss function is mean squared error.
## Results
After successful prediction, the results were visualized using the matplotlib library.
