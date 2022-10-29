## Brief: 
Estimating annual temperature changes of countries using the ARIMA model, making temperature-related analyzes

__*Before the data preparation phase*__, I made an analysis that could answer the question "Is there global warming?" since I have a large amount of temperature-related data. Result: yes there is...

### In the data preparation phase: 
I cleaned the ready csv data set from NaN and null data because I did time series analysis. The dataset I had had the average temperature of the cities and the uncertainty of the average temperature. I made it suitable for the moving average model using these two columns. Then I tested whether the dataset is stationary or not with the adfuller method. I used the shift() method to make the dataset stationary. I came to this conclusion by observing that the pi-value was less than 0.05 as a result of this method. 

### In the phase of building the model: 
I prepared the data set for the model by using the rolling method by taking advantage of the temperature differences. I manually entered the p,d,q values according to partial and normal correlations, that is, dependencies. 
### In the analysis part: 
I looked at the metrics and forecasts and tested the accuracy of the model. I could not perform the cross-validation because of an error in the module or library of the ARIMA method.
