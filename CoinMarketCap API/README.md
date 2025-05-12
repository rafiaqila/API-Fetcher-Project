# CoinMarketCap API Project

## Project Overview
This project demonstrates the use of the CoinMarketCap API to collect, store, process, and visualize real-time cryptocurrency market data. The workflow includes:
- Data Collection: Automatically fetches data on the top 15 cryptocurrencies (by market cap) at 1-minute intervals using the CoinMarketCap API. The data is normalized and appended to a CSV file for persistent storage.
- Data Preprocessing: Cleans and filters the dataset to keep only the most recent data for each coin. Handles sorting by timestamp and cmc_rank to ensure data relevance.
- Analysis:
  - Calculates average percentage changes (1h, 24h, 7d, 30d, 60d, 90d) for each cryptocurrency
  - Transforms the data for easy visualization.
- Visualization:
  - A point plot is created to compare percentage changes across different time intervals for each cryptocurrency.
  - A line plot is generated to show historical price trends of a selected coin (e.g., Bitcoin) over time.

## Conclusions
- Real-time data collection using CoinMarketCap’s API provides a reliable way to monitor cryptocurrency trends.
- From the point plot, we observe that certain cryptocurrencies exhibit higher short-term volatility compared to others.
- The historical price line plot for Bitcoin shows how price trends evolve over time, useful for tracking momentum or market sentiment.
- This project demonstrates the integration of API usage, data engineering, and basic data visualization—key skills for data analytics and engineering roles.

## Acknowledgment
This project was developed by following the tutorial by Alex The Analyst: Automating Crypto Website API Pull Using Python | Data Analyst Project
YouTube Link: https://www.youtube.com/watch?v=KB2CtEDrglY
Special thanks to Alex for the clear guidance and inspiration.
