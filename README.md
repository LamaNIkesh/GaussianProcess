# Dogecoin price prediction with Gaussian Process

Dogecoin price prediction based on the past 6 months data using non-parametric gaussian process (GP). GPy library is used for the implementation and optimisation. 

Choosing the right kernel is the main crux of using GPs. I tried a combination of linear, exponential and periodic kernels to get the best result[Lot more to improve!!]. Due to the stochastic nature of the time series, I though may be brownian kernel would be better but didn't work out well. Predicting the missing values in the data seems to work better than predicting future after a certain time point. Regardless, I learnt a bit more about Gaussian Processes which had been elusive to me for many years. 

* Dogecoin price data is extracted using `CoinGeckoAPI`
* Standard matplotlib library for visualisation. 

> The script always pulls out the latest dogecoin price or you can change to any other coin, so everytime you run it you get the latest data. 

![alt text](https://github.com/LamaNIkesh/GaussianProcess/blob/main/Plots/missing.png?raw=True)

![alt text](https://github.com/LamaNIkesh/GaussianProcess/blob/main/Plots/prediction.png?raw=True)


