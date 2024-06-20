🚀 Stock News Monitoring System 📈

Welcome to the Stock News Monitoring System! This project is designed to keep you updated on significant stock price changes and relevant news articles for your favorite companies. If you're a stock enthusiast or investor, this tool is perfect for you!

🎯 Project Overview

This Python script leverages the power of APIs to monitor stock prices and fetch related news articles. It uses the Twilio API to send updates directly to your phone, ensuring you never miss important market movements or news.

🔧 Features

Stock Price Monitoring: Tracks daily closing prices for a specified stock.
Percentage Change Calculation: Calculates the percentage change in stock price and detects significant changes.
News Fetching: Fetches the latest news articles related to the specified company when a significant stock price change occurs.
SMS Notifications: Sends SMS notifications with stock price updates and news articles using Twilio.

VIRTUAL_TWILIO_NUMBER = 'your_twilio_number'
VERIFIED_NUMBER = 'your_verified_number'
STOCK_NAME = "TSLA"
COMPANY_NAME = "Tesla Inc"
STOCK_API_KEY = "your_alphavantage_api_key"
NEWS_API_KEY = "your_newsapi_api_key"
TWILIO_SID = 'your_twilio_sid'
TWILIO_AUTH_TOKEN = 'your_twilio_auth_token'


1.Monitor Stock Prices: The script fetches the closing prices for the specified stock and calculates the percentage change.

2.Fetch News Articles: If the stock price change exceeds the defined threshold, it fetches the latest news articles related to the company.

3.Receive SMS Notifications: You will receive SMS notifications with the stock price update and a brief of the top 3 news articles.

📚 How It Works

Stock Price Monitoring:

Fetches the closing prices for yesterday and the day before.
Calculates the percentage change in price.
News Fetching:

Uses the News API to fetch the latest articles related to the company.
Selects the top 3 articles.
SMS Notifications:

Formats the news articles.
Sends each article as a separate SMS via Twilio.
