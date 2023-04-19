# crypto_pairs_trading

This repository contains a pairs trading strategy on crypto currencies. 

## Overview
The strategy works by finding the most significantly cointegrated pairs of a selection of tokens traded on binance. The notebook contains plots to demonstrate the intuition. 
Optimal entry and exit points for a pair one pair are found via grid search and cross validation, resulting in a fairly robust result, where the training result does not deviate too much from the test result.

## Results and considerations
After optimizating, I find average monthly returns of around 8% in the training set, and 5% in the test set.
This is without taking trading costs into consideration and potential margin calls from short positions moving against you. 

However, overfit is largely avoided as well as look ahead bias. Pairs are constructed only from the train set as well as the optimal entry and exit points. The test set contains new data that had not been seen before for any calculations and calibrations.
