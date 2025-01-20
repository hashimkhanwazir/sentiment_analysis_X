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
   
   API_KEY=your_api_key
   
   API_SECRET_KEY=your_api_secret_key
   
   ACCESS_TOKEN=your_access_token
   
   ACCESS_TOKEN_SECRET=your_access_token_secret

4. Run the Notebooks to Extract Tweets
   Now that you have everything set up, you can start extracting tweets. Since the project is using Jupyter Notebooks (`.ipynb` files), follow these steps:

 a. **Open Jupyter Notebook**:
   - In your terminal, navigate to the directory where your notebooks are stored.
   - Launch Jupyter Notebook by running the following command:
     ```bash
     jupyter notebook
     ```
   - This will open a new tab in your browser with the Jupyter interface. Navigate to the notebook files listed below:
     
     - `data_extractor.ipynb`
     - `data_cleaner.ipynb`
     - `data_merger.ipynb`
     - `data_translater.ipynb`
     - `sentimentAnalysis.ipynb`

b. **Run the Notebooks one by one**:
   - Open each notebook one by one, starting with `data_cleaner.ipynb`.
   - To run a cell, click on the cell and press `Shift + Enter` or use the "Run" button in the toolbar.
   - Follow the order:
     1. **`data_extractor.ipynb`**: Extract tweets from X (formerly Twitter) using the Tweepy API.
     2. **`*data_cleaner.ipynb`**: Clean the extracted tweet data.
     3. **`data_merger.ipynb`**: Merge the extracted tweet data.
     4. **`data_translater.ipynb`**: Translate the tweets from German to English.
     5. **`sentimentAnalysis.ipynb`**: Perform sentiment analysis on the translated tweets.

c. **Extract Tweets**:
   - The **`data_extractor.ipynb`** notebook will execute the code that extracts tweets based on the specified hashtags.
   - Ensure that your **Tweepy API credentials** are properly set up in the notebook (using the `.env` file you created in Step 3).
   - Rest of the steps are self explanetory.

d. **Check the Output**:
   - The extracted tweets will be displayed within the notebooks or saved into files, depending on the direcory path and file names.

## Dependencies

- **tweepy**: For interacting with the Tweepy API.
- **vaderSentiment**: For sentiment analysis using the Vader Sentiment model.
- **pandas**: For data manipulation.
- **matplotlib** and **seaborn**: For data visualization.
- **dotenv**: For loading environment variables.

### License

This project is licensed under the MIT License - see the LICENSE file for details.

### Acknowledgments

- Special thanks to the creators of the **Tweepy API** for providing an easy-to-use interface for extracting tweets from X (formerly Twitter).
- Thanks to the creators of the **Vader Sentiment** model for providing an efficient tool for sentiment analysis.

### Contributors

- **[Hashim Khan]** - Project lead, Maintaine
  - GitHub: [@hashimkhanwazir](https://github.com/hashimkhanwazir)
  - LinkedIn: [@hashim-khan-36b97818/](https://www.linkedin.com/in/hashim-khan-36b97818/)
  
- **[Bojan Mircheski]** - Team member
  - GitHub: [@Bojch](https://github.com/Bojch)
  - LinkedIn: [@bojanmircheski/](https://www.linkedin.com/in/bojanmircheski/)
  
- **[Tristan Mertins]** - Team member
  - GitHub: [@TrisMert](https://github.com/TrisMert)
  - LinkedIn: [@tristen-mertins](https://www.linkedin.com/in/tristan-mertins/)
