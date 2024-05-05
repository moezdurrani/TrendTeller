# Trend Teller: A Stock Prediction App

Trend Teller is a user-friendly web application built with Streamlit that allows users to generate stock price predictions for a selected stock based on historical data. The app leverages the powerful Prophet library for time series forecasting, providing insightful visualizations and forecasts.

## Features

- Select from a predefined list of stocks (Apple, Google, Microsoft, and GameStop)
- Specify the number of years for which you want to generate the stock price prediction
- Visualize historical stock data with open and closed prices
- Generate stock price forecasts using the Prophet library
- View forecast data and plot
- Analyze forecast components plot for a deeper understanding of the trend

Here is an animation of the app working:


![Recording-ezgif com-video-to-gif-converter](https://github.com/moezdurrani/TrendTeller/assets/103555283/c92f671c-9907-4b50-a3cb-0a02e18d2d1a)

Here is the step-by-step breakdown of the process:

- A drop-down menu for selecting a stock dataset from a predefined list
<img width="763" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/9eb70254-339c-4b7f-8564-343a42243615">

- A slider to allow the user to select the number of years for which they want to make predictions
<img width="756" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/40fc5876-131c-40b9-a9e1-0789ccde0482">

- Fetching historical stock data using the Yahoo Finance API. Added a function that caches the data to improve performance by avoiding redundant data fetching
<img width="584" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/dc117765-8a85-4088-a75c-d68e384f3c3f">

- Plotting the historical stock data (open and close prices) using Plotly. A slider was added to change the range of years for which the data is displayed
<img width="729" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/625e8126-4b70-4aa2-aa12-266df97283c1">


- Predicting the future data for the specified number of years using the Prophet model developed by Facebook
<img width="741" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/ec2d3bc0-4152-4fbf-abdc-ab14737b36ae">


- Plotting the predicted stock data using Plotly. A slider was added to change the range of years for which the data is displayed
<img width="932" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/e0491540-daae-46f3-b41f-d15c8330a22c">


- Plotting the components of the predicted data
<img width="741" alt="image" src="https://github.com/moezdurrani/TrendTeller/assets/103555283/ffe0b110-0990-4969-8867-a5c6d86040c7">


## Installation

### Clone the Repository:

```bash
git clone https://github.com/moezdurrani/TrendTeller
```




### Install Dependencies:
```bash
pip install streamlit prophet yfinance plotly
```

### Run the App:
```bash
streamlit run app.py
```
