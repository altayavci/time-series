## Brief :
Time series analysis based on estimating the "volume-weighted average price", that is, the VWAP metric, from the data obtained from the csv file where the stock market data is ready. VWAP is a metric that shows the average price of a stock adjusted for its volume.

### In the data preparation part: 
I took care not to have NaN or null data in the dataset, as I was doing time series analysis. Since the model works with the moving average principle, I prepared the data according to the model by applying the rolling windows methods.

### In the process of creating the model: 
I preferred the Auto-ARIMA model. This model is a model that works on the moving average principle and is designed to make predictions based on partial and normal correlations. If it is different from ARIMA, instead of manually entering the p, d, q values by reading the graphs, this model automatically makes the p, d, q values by cross-validation method.

### In the analysis part: 
I tested the accuracy of the model with plots and metric values.
