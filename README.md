# crypto_pairs_trading

This repository contains a pairs trading strategy on crypto currencies. 

The strategy works by finding the most cointegrated pairs of a selection of tokens traded on binance. The notebook contains plots to demonstrate the intuition. 
Optimal entry and exit points for a pair one pair are found via grid search and cross validation, resulting in a fairly robust result, where the training result does not deviate too much from the test result.

From an initial optimization, I find average monthly returns of around 8% in the training set, and 5% in the test set.
This is without taking trading costs into consideration and will still be prone to overfit as the most cointegrated pair is almost guaranteed to work very well for pairs trading.  

