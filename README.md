# Dogecoin price prediction with Gaussian Process

Dogecoin price prediction based on the past 6 months data using non-parametric gaussian process (GP). GPy library is used for the implementation and optimisation. Choosing the right kernel is the main crux of using GPs. I tried a combination of linear, exponential and periodic kernels to get the best result[Lot more to improve!!]. Due to stochastic nature of the the time series, I though may be brownian kernel would be better but didn't work out well. Predicting the missing values in the data seems to work better than predicting future after a certain time point. Regardless, I learnt a bit more about Gaussian Processes which had been elusive to me for many years. 

* Dogecoin price data is extracted using `CoinGeckoAPI`


![alt text](https://github.com/LamaNIkesh/GaussianProcess/Plots/prediction.png)
