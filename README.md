# Binance-Crypto-Data-Downloader
This Python script retrieves historical OHLC (Open-High-Low-Close) price data for cryptocurrencies listed on Binance using the Binance API. The script is designed to download data within specified time frames and intervals.

Features:
1499040000000,      // Open time
"0.01634790",       // Open
"0.80000000",       // High
"0.01575800",       // Low
"0.01577100",       // Close
"148976.11427815",  // Volume
1499644799999,      // Close time
"2434.19055334",    // Quote asset volume
308,                // Number of trades
"1756.87402397",    // Taker buy base asset volume
"28.46694368",      // Taker buy quote asset volume
"17928899.62484339" // Ignore

Data Retrieval: Utilizes the Binance API to fetch OHLC data for a specified cryptocurrency pair.
Flexible Parameters: Allows customization of ticker symbol, time interval (e.g., 4 hours, 1 hour, 1 day), start and end date for the data.
Data Processing: Converts the retrieved data into a Pandas DataFrame for easy manipulation and analysis.
Automatic Pagination: Handles pagination within the API response to retrieve historical data beyond the default limit.
Usage:
Function: get_binance_data_by_requests

Parameters:
ticker: Cryptocurrency pair symbol (default: 'ETHUSDT')
interval: Time interval for OHLC data (default: '4h')
start: Start date for data retrieval (default: '2020-01-01 00:00:00')
end: End date for data retrieval (default: '2023-07-01 00:00:00')
Output: Returns a Pandas DataFrame containing OHLC data within the specified time range.

How to Use:
Ensure you have the necessary libraries installed (e.g., requests, datetime, pandas, numpy).
Call the get_binance_data_by_requests function with desired parameters to download data.
Perform analysis, visualization, or any required operations on the retrieved data.
Note:
The script automatically handles pagination to download complete historical data within the specified time frame.
It's recommended to review Binance API documentation for endpoint rate limits and usage guidelines.
Feel free to use, modify, or contribute to this script for your cryptocurrency data analysis needs.

