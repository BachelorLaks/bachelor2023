# bachelor2023

## Abstract
The purpose of this thesis is to utilize analytical models to predict the price of salmon using similar commodities and macroeconomic factors. To make these predictions we have used the cod price, halibut price, CPI and TWI. We have developed four models; ARIMA, SARIMA, SARIMAX and LSTM. These are all trained on a dataset gathered from Norsk Råfisklag. The models are trained on the data from the timeperiod spring 2013 to winter 2021, and tested on data from 2022. 

Our research and testing has shown that the predictions improve when taking seasonality into account. The improvement from the ARIMA to the SARIMA model is very significant, whereas the improvement from SARIMA to the SARIMAX with one exogenous variable is very small. This is also clearly shown in the predictions from the three models, where the SARIMA and SARIMAX roughly follow the same trends, and the ARIMA simply predicts the same average price for all weeks. The best prediction from the LSTM model also comes close to the RMSE of the SARIMAX model, but the results from the LSTM model varies greatly depending on the lookback period. Lookbacks of 52 and 104 weeks are the best perfoming in terms of catching the trends, but the lookback periods of the models with the lowest RMSE is quite random. LSTM with short lookback periods predict the average quite well, meaning that the RMSE is low, however, when looking at the graphs its clear that this does not actually represent a good prediction. 

Even though the SARIMAX model performs the best, there are still areas of uncertainty. Tests on the SARIMAX model show that we can't conclude whether or not the residuals are white noise. We can only conclude that we can't reject the null hypothesis that the residuals are white noise.  

In conclusion the models taking seasonality into account can to some extent catch the trends in the price of salmon, but they are not able to predict the price of salmon with a high degree of accuracy. 

![alt text](https://seatrans.no/wp-content/uploads/2022/01/FIskestim-scaled.jpg)