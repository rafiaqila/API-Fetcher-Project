# Automated New York Weather Forecasting & Visualization

## Project Overview
This project fetches hourly weather forecast data using the [NOAA Weather API](https://www.weather.gov/documentation/services-web-api), processes the data into a structured format using `pandas`, and visualizes key weather metrics.

The automation is scheduled to run every hour, fetching updated forecasts and generating plots which are saved locally for later review or reporting.

## Fetch Weather Data
We create  `weather_api_runner()` function to retrieves the hourly weather forecast from the NOAA API for a specific grid point (in this case, New York - `OKX/36,36`). It extracts and organizes relevant weather features such as: `temperature`, `humidity`, `probabilityOfPrecipitation`, `windSpeed`, and `shortForecast`

## Data Visualization
Three plots are generated after each fetch:
  - **Line Plot**: Temperature, Humidity, and Precipitation over time
  - **Bar Plot**: Frequency of `shortForecast` conditions (e.g. Rain, Sunny)
  - **Line Plot**: Wind Speed over time

## Automation with Scheduler
We use the `schedule` library to automatically run the `weather_api_runner()` function every hour. It runs immediately once. Then, continues to fetch and plot data every hour on the hour.

## Conclusion
This project demonstrates how to:
- Use public APIs for live weather data
- Automate data fetching and visualization
- Save results for reporting or future analysis
