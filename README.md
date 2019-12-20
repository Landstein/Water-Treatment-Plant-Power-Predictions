# Water-Treatment-Plant-Power-Predictions
Water Treatment plant power prediction.  Two main power generators represented by power A and Power B.  Will use multiple Time Series models to predict the power usage.  


### Project Goals
1. Become familiar with Arima, Sarima and Facebook Prophet Models 
2. Determine the seasonality within the water treatment plant 
3. Predict the Power usage 1 week into the future 


### Data
Water Treatment plant in the Unite States.  

The original Dataset was on a 4 hour frequency from August - November 2019.  (550 Data Points)
The Final Dataset was 1 year of hourly data. (8731 Data Points)

Power is measured in kWh

### Initial EDA 

Plot of the Data from Power Generator A. 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20Month%20Data.png)

Power A average power based on the time of day.  Shows there is some daily seasonality within each cycle.  Can see the water treatment plant is using the least power around 4 A.M. and the around 8 P.M.. 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20Month%20Box%20Plot%20.png)

Power A daily cycle.  Shows the daily seasonality 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/ETS%204%20hour%20Cycle%20.png)

Power A overall trend
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20month%20trend.png)

### Initial Sarima Model 
Initial Sarima Model definitely got the overall trend, but was only able to hold the prediction two days into the future.  
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%20Sarima%20Model.png)


**To improve the model I used a second data set with 1 Year of hourly Data** 


### 1 Year hourly Dataset EDA 
Following EDA used the second dataset with 8731 data points over a year. 

Plot of the Power usage over 1 year
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Total%20Power%20data.png)


Power usage by hour average  This plot is a little more accurate then the above.  The low of the day is around 5 A.M. and the peak is around 9 - 11 P.M. 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Total%20Power%20Boxplot.png)


### Facebook Prophet Model 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Total%20Power%20Sarima.png)


### Final Sarimax Model 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Total%20Power%20Sarima.png)


### Conclusions 

- For time series it is necessary to have a lot of data. The improvement in the models from the first data set to the second is substantial
- The facebook prophet model had a RMSE of about 224,000 compared to the Sarimax model which had a RMSE of 159,000.  
- Overall the Sarimax Model was predicting with a high enough accuracy for it to be useful. 

