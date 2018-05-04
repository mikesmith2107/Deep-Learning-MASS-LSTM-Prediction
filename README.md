# Deep-Learning-MASS-LSTM-Prediction
This project is to create a model, that is completely automated(setting buy/sell Flags, prediction of the next day) 

First and foremost: This programs NueroNet is was retro fitted for my Computer system.
My System Setup:
Ubuntu 16.04 LTS
Dual Xeon #5520 2.27Ghz (Each cpu containing 8 cores)(total core count = 16 cores)
16GB dual channel pc3 1333Mhz
Nvidia 1050 GTX OverClocked to 1607Mhz
Tesla Card with 1200 Cuda Cores

Though my Program do not use the gpu's as of this moment. At some point it will, thus hopefully rendering predictions every 10-15 Seconds
As of right now Average Time for Prediction is around 10-25 seconds depending on DataSet.

My Code is as Followed:


IMPORTING MODULES:

`import numpy as np`

`import matplotlib.pyplot as plt`

`import matplotlib.pyplot as plt2`

`import pandas as pd`

`from pandas import datetime`

`import math, time`

`import itertools`

`from sklearn import preprocessing`

`import datetime`

`from sklearn.metrics import mean_squared_error`

`from math import sqrt`

`from keras.models import Sequential`

`from keras.layers.core import Dense, Dropout, Activation`

`from keras.layers.recurrent import LSTM`

`from keras.models import load_model`

`import keras`

`import pandas_datareader.data as web`

`import h5py`

# Load In the Data Set with your File Locations to the Adjusted Folder to pull Main_DF which contains the Ticker,Path to file Desired

`DF1_path = 'C:\\Users\\SkullCrusher\\Desktop\\StockPrediction\\Adjusted\\Main_DF'`

`Main_DF = pd.read_csv(DF1_path,index_col=0)`


# Next I will begin Defining Definitions to be called upon request:

## To Be Coninued Taking a rest for a moment while I Test additional Information into NueroNet
## Brother mentioned adding 3 Day MPA and 6 Day MPA. So I am Adjusting DataBase For Additional 2 Columns inside Each Ticker DataSet
