# Sentiment Analysis for Stock Discussions

## Overview
This project performs sentiment analysis on Reddit posts related to stock symbols. Using PRAW for Reddit API integration and TextBlob for sentiment analysis, the program analyzes posts from a specified subreddit, classifies the sentiment (Positive, Negative, Neutral), and visualizes the results using bar charts and pie charts.

## Problem Statement
This project addresses the KYNNOVATE 2025 problem statement: *Sentiment Analysis Track*.

*Requirements:*
- Perform real-time sentiment analysis.
- Identify trending topics.
- Generate sentiment reports.
- Provide actionable insights.

## Key Features
- *Real-time Sentiment Analysis:* Extracts and analyzes sentiment from Reddit posts related to a specific stock symbol.
- *Visualization:* Generates graphical representations of sentiment distribution.
- *Configurable Input:* Users can specify stock symbols and the number of Reddit posts to analyze.

## Tools and Technologies
- *Python*: Programming language used for implementation.
- *PRAW (Python Reddit API Wrapper)*: Accesses Reddit data.
- *TextBlob*: Performs sentiment analysis on the text.
- *Matplotlib*: Visualizes sentiment data with bar charts and pie charts.

## How It Works
1. *Input Stock Symbol:* Users enter the stock symbol they want to analyze.
2. *Fetch Reddit Posts:* The script fetches posts from the specified subreddit (default: stocks) related to the symbol.
3. *Analyze Sentiment:* Each post is analyzed using TextBlob, classifying sentiment as Positive, Negative, or Neutral.
4. *Visualize Data:* Bar and pie charts are generated to represent sentiment distribution.

## Prerequisites
1. *Python 3.x*: Ensure Python is installed on your system.
2. *Dependencies*:
    - PRAW: pip install praw
    - TextBlob: pip install textblob
    - Matplotlib: pip install matplotlib
3. *Reddit API Credentials*:
   - Create a Reddit app via [Reddit API](https://www.reddit.com/prefs/apps).
   - Obtain client_id, client_secret, and user_agent.

## Installation and Setup
1. Clone the repository or copy the script.
2. Install required libraries:
   bash
   pip install praw textblob matplotlib
   
3. Replace the client_id, client_secret, and user_agent values in the script with your Reddit API credentials.
4. Run the script:
   bash
   python sentiment_analysis.py
   

## Project Structure
- sentiment_analysis.py: Main script to perform sentiment analysis and visualization.

## Usage
1. Execute the script:
   bash
   python sentiment_analysis.py
   
2. Enter the stock symbol when prompted.
3. View the sentiment analysis results and visualizations.

## Example
*Input:* TSLA

*Output:*
- Bar Chart: Sentiment distribution (Positive, Negative, Neutral).
- Pie Chart: Sentiment proportions.

## Limitations
- The script currently analyzes a limited number of posts (default: 20).
- Sentiment accuracy depends on TextBlob's performance, which might not capture sarcasm or domain-specific nuances.

## Future Enhancements
- *Trending Topics:* Extend functionality to identify trending stocks and topics.
- *Sentiment Reports:* Generate detailed sentiment reports for download.
- *Improved Analysis:* Use advanced NLP models (e.g., BERT) for better sentiment classification.
- *Dashboard:* Build a web-based dashboard for real-time visualization and insights.

## Contribution
Contributions are welcome! Please fork the repository, make changes, and submit a pull request.

## License
This project is licensed under the MIT License. See LICENSE for details.
