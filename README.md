# RNN to predict Google Stock Prices
A Recurrent Neural Network coded in Python using Tensorflow's Keras to try to predict Google Stock prices.
## Installation
* Download and install Python3 from [here](https://www.python.org/downloads/)
* I recommend using [virtualenv](https://virtualenv.pypa.io/en/latest/) to create a Python environment. It's good practise to create and use different environments for different projects. Open a terminal and type:
    ```bash
    pip install virtualenv
    ```
* Create a Virtual environment with some name say rnnenv.

   * Windows
   ```bash
   virtualenv rnnenv
   cd rnnenv/Scripts
   activate
   ```
   * Linux:
   ```bash
   source rnnenv/bin/activate
    ```
* Clone this repository, extract it if you downloaded a .zip or .tar file and cd into the cloned repository.

    * For Example:
    ```bash
    cd A:\RNN-to-predict-Google-Stock-Prices-master
    ```
* Install the required packages by typing:
   ```bash
   pip install tensorflow==1.15
   pip install pandas
   pip install matplotlib
   pip install numpy
   pip install scipy
   pip install -U scikit-learn
   ```
## Running
```bash
python rnn.py
```
## Dataset
The dataset contains high, low, close and open values of Google's stock prices, date and the volume.
I tried to predict the open values based on past open values
## Architecture
The architecture of the RNN is 4 sets of LSTM (Long short term memory) layers and Dropout regularization layers with the LSTM and Dropout layers sandwitched between each other.
The number of time steps chosen for the RNN is 60.
The model is trained on 100 epochs with a batch size of 32.
The optimizer used is adam and the loss function is mean squared error.
## Results
After successful prediction, the results were visualized using the matplotlib library.

