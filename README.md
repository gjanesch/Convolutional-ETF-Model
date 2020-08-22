This is a Jupyter notebook that is designed to do the following:
1. Acquire data on sector exchange traded funds (ETFs) and an ETF that tracks the Dow Jones Industrial Average from the API of [Tiingo](https://www.tiingo.com/).
2. Calculate daily returns for the sector ETFs and longer-term returns for the DJIA ETF (length of time can be configured in the code).
3. Feed a window of daily returns into a few different neural network models (focusing on convolutional networks) and use them to try to predict the direction of the DJIA ETF.

A blog post writing up the reasoning behing this code is [here](https://data-and-the-world.onrender.com/posts/convolutional-sector-etf-prediction/).

Note: the code assumes that the string containing the Tiingo API key is in a file names "api_key.py"; you'll need to supply your own key in order to get this to work.

Requires pandas, pandas_datareader, numpy, scikit-learn, tensorflow, keras.
