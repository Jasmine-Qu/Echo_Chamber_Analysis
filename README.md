# Echo Chamber Analysis

## Introduction
With the recent saga1 about a subreddit community (‘WallStreet bets’) being able to influence greatly the price of a risky stock (‘GameStop – GME’), any abuse of the platform to influence markets can result in severe ramifications on the economy, both locally and globally. Our study seeks to study the various features of subreddit communities that contribute to echo chambers on stocks and determine their level of importance towards stock indexes. As Reddit has a large database, our study adopted the use of PySpark and other big data techniques to process the large dataset.

## Steps
![image](https://user-images.githubusercontent.com/68145995/116177809-10b8df80-a747-11eb-8691-a8b3af168db8.png)

These steps were taken to build our model:
- (i) Reddit data extraction & preprocessing
- (ii) extraction and analysis of network features
- (iii) sentiment analysis of Reddit contents
- (iv) machine learning model training and validation
- (v) feature importance analysis and insights. 
Several machine learning models of different types and complexity were explored, including a time series method SARIMAX, and tree-based methods XGBoost and RandomForest. In terms of performance, XGBoost yielded the best results, with the MAPE = 2.01% for the best index. The top 5 most important features are retention rates, the daily average number of subscribers, daily average author count, the daily average count of posts, and sentiment score, which shows more importance of network metrics than sentiment metrics. These
features were able to predict better on a market index than a stock index.

## Conclusion
We were able to measure the level of importance of features extracted, and our study concludes that network analysis features are highly relevant and impactful in determining 
stock index accurately, with the best being the retention rate of authors in any subreddit group. This narrows the metricsused to track and monitor to detect high levels of activities that can potentially impact the market to a large degree. The model can also be leveraged to estimate the level of impact on the stock market, so that governments and economic agencies can be prepared, ensuring it does not negatively impact the economy. Further development on the application can help to extend this to other social platforms and turn it into a monitoring device to pre-empt such scenarios.
