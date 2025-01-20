# Sentiment Analysis of New Year Event in Germany Tweets

## Project Overview

This project aims to perform sentiment analysis on tweets extracted from [X](https://x.com/) (formerly Twitter) using the [Tweepy](https://docs.tweepy.org/en/stable/) API. 
The goal is to analyze public sentiment surrounding the New Year event, focusing on tweets related to fireworks, firecrackers, and any incidents such as injuries.

The dataset includes approximately 350 tweets in German, which have been translated into English for analysis. The tweets are extracted based on relevant **hashtags** related to the New Year celebration, specifically:

- **#Bombe** (German for "bomb")
- **#Feuerwerk** (German for "fireworks")
- **#Silvester** (German for "New Year's Eve")
- **#Boller** (short for "Böller" — German for "firecracker")

These hashtags are used to collect tweets that mention or are related to these topics, providing insight into public sentiment regarding the events surrounding the celebration, including fireworks displays, the use of firecrackers, and any incidents such as injuries.

## Features

- **Tweet Extraction**: Collects tweets related to the New Year event, specifically those that mention fireworks, firecrackers, or incidents, based on specific hashtags (`#Bombe`, `#Feuerwerk`, `#Silvester`, `#Boller`).
- **Data Cleaning**: Preprocesses the extracted tweet data by removing unnecessary information, standardizing formats, and preparing it for sentiment analysis.
- **Data Merging**: Combines relevant tweet data (such as tweet content, location, and engagement metrics) for further analysis.
- **Translation from German to English**: Translates the collected tweets from German to English to ensure consistency and ease of sentiment analysis.
- **Sentiment Analysis**: Uses the Vader Sentiment model to classify tweets as positive, negative, or neutral, providing insight into public sentiment toward the New Year event and associated topics.

## Installation

1. Clone the repository:

   ```bash
   git clone git@github.com:hashimkhanwazir/sentiment_analysis_X.git
   cd ./sentiment_analysis_X
   
2. Install the required dependencies:
   pip install -r requirements.txt

3. Set up the Tweepy API by creating an application in the `X Developer Portal` and obtain your credentials (API key, API secret key, Access token, and Access token secret). Store these credentials in a `.env` file.

Example `.env` file:
