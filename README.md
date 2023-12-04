# Dow Jones Index 30 (US30) - CNBC Summary Dashboard

This GitHub repository contains a custom TradingView indicator implemented in Pine Script. The indicator provides a comprehensive summary of the Dow Jones Industrial Average (US30) and its constituent stocks. The code is subject to the terms of the Mozilla Public License 2.0.

## Indicator Overview

The "US30 Dashboard" indicator is designed to give traders and investors a quick overview of the performance of the Dow Jones Industrial Average (US30) and its 30 constituent stocks. It displays various key metrics, including the trend, the number of stocks in an uptrend and downtrend, the percentage of stocks in each trend, the total change in stock prices, and the percentage change in stock prices.

## Data Fetching

Before performing calculations, the code fetches daily closing price data for each of the 30 constituent stocks of the Dow Jones Industrial Average. The list of stocks includes well-known companies such as Boeing (BA), Goldman Sachs (GS), Intel (INTC), Microsoft (MSFT), and others. For each stock, both the current day's closing price and the previous day's closing price are obtained.

## Calculations

The heart of the indicator lies in the `calculations` function. This function calculates the following metrics:

- **Uptrend**: The number of stocks that have experienced a positive percentage change in their closing prices compared to the previous day.
- **Downtrend**: The number of stocks that have experienced a negative percentage change in their closing prices compared to the previous day.
- **Uptrend Change**: The total change in closing prices of stocks in an uptrend.
- **Downtrend Change**: The total change in closing prices of stocks in a downtrend.
- **Uptrend Percentage Change**: The total percentage change in closing prices of stocks in an uptrend.
- **Downtrend Percentage Change**: The total percentage change in closing prices of stocks in a downtrend.

These metrics are calculated for all 30 constituent stocks, and then the percentages are calculated in relation to the total number of stocks, providing a comprehensive summary of the overall trend and performance of the Dow Jones Industrial Average.

## Table Visualization

The indicator presents its findings in a visually appealing table format. The table includes five rows and three columns, displaying the following information:

- **Trend**: A header cell indicating the trend analysis.
- **Uptrend**: The number of stocks currently in an uptrend, displayed in green.
- **Downtrend**: The number of stocks currently in a downtrend, displayed in red.
- **Stocks**: A header cell indicating the number of stocks.
- **Stocks (%)**: The percentage of stocks in an uptrend and downtrend, displayed in green and red, respectively.
- **Change**: The total change in closing prices for uptrending and downtrending stocks.
- **Change (%)**: The total percentage change in closing prices for uptrending and downtrending stocks.


**Disclaimer:** This script is provided for educational purposes and does not constitute financial advice. Use it responsibly and at your own risk when trading or investing.
