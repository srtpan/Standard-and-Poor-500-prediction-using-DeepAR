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

