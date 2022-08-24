# LSTM-and-GRU

Classification prediction with LSTM and GRU neural networks as a support to investment and risk management strategies.

******************************* Abstract *******************************

Randomness dynamics in financial markets can be captured by the volatility, which directly links to the risk aversion of investors. As a consequence, a successful volatility prediction can be highly profitable from many aspects: For the investment manager, it can be a signal to hedge his investment portfolio in response to high upcoming volatility. For the option trader, it can be a signal for a volatility arbitrage. For the risk manager, it can be a support to forward-looking risk measures which depict the portfolio risk better.

This paper is about a classification prediction exercise in order to support investment and risk management strategies using neural networks. Two variations of Recurrent Neural Networks (RNN), the Long-Short Term Memory (LSTM) and the Gated Recurrent Units (GRU) models are employed to predict whether the volatility spread between the realized and implied volatility (RV-IV spread) ends up positive or negative on the next trading day. In particular, LSTM and GRU models adopt the same structure design - prior tuning of hyperparameters, such that their prediction performances can be compared. SP500 Index and the Eurostoxx 50 Index are used as support for the classification prediction exercise and design of investment and risk management strategies. For both indices, the GRU model outperforms the LSTM model. 

Both investment and risk management strategies are built around the interpretation that a positive RV-IV spread prediction is indicative of a bear market to come as a result of higher upcoming volatility. The investment strategy, derived from SP500 GRU predictions, highlights that the GRU model does well in identifying a bear market and avoiding losses, albeit initially struggling to identify a bull market. The risk management strategy incorporates Eurostoxx 50 GRU predictions and machine learning techniques applied to volatilities and correlations to derive forward-looking risk measures in the case of an investment portfolio.

******************************* Main paper *******************************

---> "Long-Short Term Memory and Gated Recurrent Units as a support to investment and risk management strategies"

******************************* Supporting note *******************************

---> "Deep learning toolbox for classification prediction models"

Supporting theory to the main paper. Theory around deep learning in a separate document for main paper readability reasons

******************************* Model 1: SP500 Index *******************************

Code: Model 1_SP500 Index.ipynb

Source files: SPX.xlsx, 10Y_yield.xlsx, VIX.xlsx

******************************* Model 2: SP500 Index *******************************

Code: Model 2_Eurostoxx 50 Index.ipynb

Source files: ES50_Bloomberg.xlsx, GICS - ES.csv, ES50_ohlc.npy

******************************* POPSOM py package *******************************

.py file with popsom package for feature importance using SOM
