# S&P 500 Prediction using DeepAR

The objective of this project is to to extend the classic DL time series modeling into a probabilistic framework and overcome the limitations of classic deep learning time series architecture which give deterministic result without quantifying the uncertainty.

Statistical methods of time series prediction rely heavily on data pre-processing and are not very robust when it comes to prediction accuracy. Neural networks have been helpful in terms of better prediction accuracy but they are still limited in application. This project is to extend their usability by adding probabilistic understanding to the deep learning time series prediction frameworks. 

In addition to providing better forecast accuracy than previous methods, the DeepAR approach has a number of key advantages compared to classical approaches and other global methods:


 1. As the model learns seasonal behavior and dependencies on given covariates across time series, minimal manual feature engineering is needed to capture complex, group-dependent behavior;

2. DeepAR makes probabilistic forecasts in the form of Monte Carlo samples that can be used to compute consistent quantile estimates for all sub-ranges in the prediction horizon;

3. By learning from similar items, their method is able to provide forecasts for items with little or no history at all, a case where traditional single-item forecasting methods fail

4. Their approach does not assume Gaussian noise, but can incorporate a wide range of likelihood functions, allowing the user to choose one that is appropriate for the statistical properties of the data.

## Why DeepAR 

DeepAR model integrates LSTM successfully with Autoregressive recurrent network and enables to predict multiple time-series at once. This approach has been quite successfully applied to natural language processing but has remained rather unexplored in the context of time-series prediction. 

Other methods of time-series prediction like AR, MA, ARIMA, etc. are unable to learn simultaneously from multiple time-series. DeepAR provides better accuracy without overfitting during training. As mentioned previosuly, the classical prediction methods also rely on pre-processing methods for giving better results but the standard techniques sometimes fail to apply generally over data and that's where DeepAR has an advantage. 

## Experimental Results

SP500 Dataset being market data has been quite volatile over the years. The volatility makes it difficult to predict the stock index and the models used in our project also show instability when it comes to predicting stock market prices. DeepAR model tends to perform well with other, rather stable data set  like electricity or car parts sales data. When it comes to predicting stocks value, the RMSE remains unstable and fluctuates between 40-200.

When trying to predict stock prices of individual companies, the model performs well for companies whose stocks tend to move together like Apple, Facebook, Amazon, etc. For a random set of companies, the model gives very high RMSE values, to the magnitude of 1000. 

After normalizing the data and removing the trend, the model improves a lot and the RMSE drops to **0.269** (mean). For individual companies, adjusted close price prediction, similar improvement is noticed. However, when similar companies are clubbed together, the RMSE is much lower. When all the companies are taken together, the RMSE is around 300 with normalized data. 


