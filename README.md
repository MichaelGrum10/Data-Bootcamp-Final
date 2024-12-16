# Data-Bootcamp-Final
### Introduction:
  Stocks are quite unpredictable. Their price and volume change every second, having the possibility to rise and fall by a momentous percentage in the blink of an eye. They also don't often follow set or clear patterns which is why they are incredibly difficult to trade for the average person. However, there are metrics such as the Dow Jones Industrial Average (DJI) and the SMP500 which depict the overall movement and sentiment of the stock market. Throughout this project, I will be comparing the top 500 publicly traded companies to the DJI in order to analyze if there is a cooperation between how these highly traded stocks behave compared to the overall market. The reason I chose the reason the DJI to represent the overall market in my project is because it focuses on 30 large, well-established companies, making it easier to explain trends and movements to a general audience, it is widely reported in the media and is often used as a shorthand for the market's overall health, and it is price-weighted, meaning higher-priced stocks have more influence on the index's movements which can illustrate the impact of specific high-profile and commonly traded companies on market sentiment. Through this project, I hope to find how strong the correlation is between these prominent stocks and the overall market, and to what extent these individual stocks follow the trend of the market overall. 
Furthemore, these predictions will help people decide whether to invest in a stock based on the trends and predictions of DJI, making investing much easier for the average person. Due to the mass amounts of descriptive and often updating news about the DJI (due to the fact often used as a shorthand for the market's overall health in the media), it will be much easier for an average person to read headlines and determine if they would like to invest into certain stocks. 

### Data Description:
  In my search to find a data set or api which would be able to provide me with the stock information I needed for this project, I realized that there weren’t many widely available for my use. Instead, I decided to develop my own data set using yfinance. Firstly, I took a wikipedia url which listed the top 500 companies on the stock market and transformed it into a list. This list was then used to create a data set containing the open price, daily high, daily low, close price, adjusted close price and volume for all of the stocks in the list from the past 5 years. Additionally, I added the DJI and SMP500 to this data set. 
  
  For my preliminary research, I initially believed I could find a correlation between volume and price (high) so I graphed it on a scatter plot. My results were inconclusive as the data was heavily clustered around two points which made it evident that there was not much, if any correlation between price and volume. Furthermore, I then plotted the cumulative percent change in DJI, the index which I chose to represent the whole market, against the percent change of the SMP500, the index which represents the 500 companies in my data set as a whole. Through this, I discovered that both indexes have an incredibly similar, almost identical, percent change based on the shape of the graphs. To further solidify my hypothesis, I plotted the normalized prices (the stock price divided by the moving average which removes short term fluctuations, therefore smoothing out the data) of both and the shapes of the graphs were identical to the shapes of the previously plotted percent change graphs. This research proved that there in fact is a cooperation between the 500 stocks in my data swt and the DJI. To further my observations, I decided to plot the percent change of individual stocks against the percent change of the DJI and SMP500. I wrote code which allowed me to input a ticker of any of the stocks in my data frame and plot its percent change. I tested a few tickers such as TSLA, AAPL, AMZN and observed that they do relatively follow the same trend as the graphs of the DJI and SMP500 with varying fluctuations which allowed me to solidify my hypothesis that there is a substantial amount of correlation between the stocks in my data set and DJI. 
