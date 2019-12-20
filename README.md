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

### EDA 

Plot of the Data from Power Generator A. 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20Month%20Data.png)

Power A average power based on the time of day.  Shows there is some daily seasonality within each cycle.  Can see the water treatment plant is using the least power around 4 A.M. and the around 8 P.M.. 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20Month%20Box%20Plot%20.png)

Power A daily cycle.  Shows the daily seasonality 
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/ETS%204%20hour%20Cycle%20.png)

Power A overall trend
![](https://github.com/Landstein/Water-Treatment-Plant-Power-Predictions/blob/master/images/Power%20A%204%20month%20trend.png)


**Movie revenue by month**

From the data it is hard to determine if there is a best month to release a movie as April had the Avengers which was a big outlier.  Though it is safe to say that August was the worst performing month.  

![](https://github.com/Landstein/TopMovies/blob/master/images/Movie_release_month.png)

**Profitability**

For this category we looked at which movies had the best return on their investment.  

![](https://github.com/Landstein/TopMovies/blob/master/images/top_profit.png)

The Movies in Red are

- Bohemian Rhapsody
- A Star is born 
- A Quiet Place
- The Nun 
- Peter Rabbit
- Fifty Shades Freed 
- Green Book

**Genre**

Compared Genres that showed up in the movies that had the best revenue per budget against the other top 100 movies 

![](https://github.com/Landstein/TopMovies/blob/master/images/genre.png)

**Home Sales**

Lastly we looked at DVD and Blu Ray sales to see if there was any indicator of what type of movie has the best after theater sales.  Overall it was pretty consistant. 

![](https://github.com/Landstein/TopMovies/blob/master/images/homesales.png)

![](https://github.com/Landstein/TopMovies/blob/master/images/revenueandhomesales.png)

### Conclusions 

- The best performing genres were Drama, Horror, Music and Romance 
- Best Months to release a movie: April, June, July December 
- Worst Month to release a movie: August 
- If a movie is in the top 100 grossing for the year.  It will likely have good DVD / Blu Ray sales 
