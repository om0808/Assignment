# Assignment 

Assumptions made in the code -

1. Technical indicators are calculated using the actual monthly closing price (close) rather than adjclose because close price represents the real market-traded value whereas adjusted close is for company's evaluation criteria.
2. All technical indicators (SMA and EMA) are calculated after resampling the data to monthly frequency, using the monthly closing price (last trading day of each month).
3. SMA 10 / EMA 10 represent 10-month moving averages
   SMA 20 / EMA 20 represent 20-month moving averages
   Since indicators are computed on monthly data, the window sizes correspond to months, not days
4. The first EMA value is initialized using the corresponding Simple Moving Average (SMA) [As mentioned]
   
Note - The first 9 rows for 10-month indicators and first 19 rows for 20-month indicators are left empty (NaN).
This is because sufficient historical data does not exist to compute first 10-month and first 20-month moving averages.
