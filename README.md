# Investisight

Investisight is a sentiment-driven stock prediction project that explores whether financial news sentiment can improve stock price forecasting. The project combines scraped Pakistani news headlines from DAWN News with HBL stock market data, then uses the combined dataset to train an LSTM model for time-series prediction.

## Overview

Financial markets are often influenced by public sentiment, breaking news, and investor confidence. This project investigates that relationship by extracting sentiment signals from news headlines and integrating them with historical stock data.

The pipeline includes:

- Scraping DAWN News headlines related to Pakistan’s financial and business environment
- Performing sentiment analysis on headlines to calculate negative, neutral, positive, and compound scores
- Merging sentiment features with HBL stock price data
- Preparing historical sequence data for LSTM-based forecasting
- Training an LSTM model to predict future stock price behavior
- Visualizing stock trends, sentiment distributions, and key stock attributes

## Motivation

Traditional stock prediction models often rely only on historical price and volume data. However, market sentiment can provide additional context, especially in markets where news events strongly influence investor behavior.

Investisight was built to test whether headline sentiment can be used as an additional predictive signal for stock forecasting.

## Data Sources

### DAWN News Headlines

DAWN News was used as the primary news source because it is one of Pakistan’s major English-language news outlets. Headlines were scraped and processed to extract sentiment-related features.

For each headline, the following sentiment scores were calculated:

- Negative sentiment
- Neutral sentiment
- Positive sentiment
- Compound sentiment score

### HBL Stock Data

Historical HBL stock data was used as the financial dataset. The stock data was merged with the sentiment data by date to create a combined time-series dataset.

The final dataset included both market indicators and sentiment-based features.

## Methodology

### 1. News Scraping

News headlines were collected from DAWN News and organized by date. These headlines served as the textual input for sentiment analysis.

### 2. Sentiment Analysis

Each headline was processed using a sentiment analysis model to calculate sentiment scores. These scores were then aggregated and aligned with stock market dates.

### 3. Data Integration

The sentiment data was merged with HBL stock data to create a single dataset containing both financial and textual sentiment signals.

This combined dataset allowed the model to learn from historical sequences of stock values and market sentiment.

### 4. LSTM Model Training

An LSTM model was used because it is well-suited for sequential data and time-series forecasting. The dataset was transformed into historical windows so the model could learn temporal patterns across previous stock and sentiment values.

The model was trained to predict a target variable such as future stock price.

### 5. Visualization

The project includes visualizations to support analysis and interpretation, including:

- Time-series graphs of stock prices
- Distribution plots of stock attributes
- Sentiment score trends
- Model performance visualizations

## Key Features

- End-to-end data pipeline from scraping to prediction
- Sentiment analysis on real financial news headlines
- Integration of textual sentiment features with stock market data
- LSTM-based time-series forecasting
- Visual analysis of stock and sentiment trends

## Tech Stack

- Python
- Pandas
- NumPy
- BeautifulSoup / Requests
- Sentiment analysis tools
- TensorFlow / Keras
- Matplotlib
- Seaborn
- Scikit-learn

## Results

The project demonstrated how sentiment data can be incorporated into a stock prediction workflow. By combining DAWN News headline sentiment with HBL stock data, the model was able to learn from both historical market behavior and external sentiment signals.

The visualizations also helped identify trends in stock prices, sentiment distributions, and relationships between news sentiment and market movement.

## Project Timeline

**Sentiment-Driven Stock Prediction, GIKI**  
**Sep 2024 – Jan 2025**

## Resume Summary

Developed a sentiment-driven stock forecasting pipeline by scraping DAWN News headlines, extracting sentiment scores, merging them with HBL stock data, and training an LSTM model on historical sequences to predict future stock behavior. Built visualizations to analyze stock trends, sentiment distributions, and model performance.
