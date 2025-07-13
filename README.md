# SENTIMENT-ANALYSIS

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : SATYAM THEURKAR

*INTERN ID* : CT06DF2424

*DOMAIN* : DATA ANALYTICS

*DURATION* : 6 WEEKS

*MENTOR* : NEELA SANTOSH

# 📊 Sentiment Analysis on Textual Data – Internship Task 4

## 📝 Project Overview

This project is developed as part of an internship task to perform sentiment analysis on textual data using Natural Language Processing (NLP) techniques. The analysis is conducted on a dataset of tweets related to various mobile phones, sourced from Kaggle’s Walmart dataset. The objective is to extract meaningful sentiment insights from user-generated content and visualize sentiment trends associated with different phone models.

## 🔧 Tools & Technologies Used

- **Google Colab** – for writing and running Python code in a collaborative cloud environment.
- **Python** – as the primary programming language.
- **Pandas** – for data manipulation and analysis.
- **NumPy** – for numerical operations.
- **Matplotlib & Seaborn** – for data visualization.
- **NLTK (Natural Language Toolkit)** – for sentiment analysis using VADER (Valence Aware Dictionary for Sentiment Reasoning).
- **Kaggle** – for downloading the Walmart tweet dataset.

## 📂 Dataset Description

- The dataset used in this project is `phone_tweets.csv`, downloaded from Kaggle.
- It contains tweets related to various mobile phones.
- Key columns include:
  - `tweet`: Original tweet content.
  - `phone name`: Model or brand name mentioned.
  - `language`: Language of the tweet.
  - `likes_count`: Number of likes received by the tweet.
  - `link`: URL to the tweet.

## 🔍 Workflow Summary

1. **Data Loading**  
   The dataset was imported using Pandas from the Google Drive path into Colab.

2. **Language Filtering**  
   Only English-language tweets (`language == 'en'`) were retained to ensure compatibility with the VADER sentiment analyzer.

3. **Text Preprocessing**  
   A custom function `clean_tweet()` was created to:
   - Remove URLs, mentions, hashtags, and special characters.
   - Convert all text to lowercase.

4. **Sentiment Analysis**  
   - VADER from the NLTK library was used to assign sentiment scores.
   - Tweets were categorized as:
     - **Positive** (score ≥ 0.05)
     - **Negative** (score ≤ -0.05)
     - **Neutral** (otherwise)

5. **Visualization**  
   - A count plot was generated to visualize the overall sentiment distribution.
   - A stacked bar chart shows sentiment breakdown across different phone brands.

6. **Highlighting Insights**  
   - The top 5 positive tweets (with highest like counts) were identified and displayed.
   - These tweets were likely the most influential in forming public opinion.

7. **Output Generation**  
   - The processed data with sentiment labels and scores was saved to a CSV file named `sentiment_analysis_output.csv`.

## 📈 Key Insights

- Most tweets were either positive or neutral, showing general customer satisfaction.
- Certain brands/models had higher counts of negative sentiments, which could indicate areas for product or service improvement.
- Positive tweets with high like counts can serve as testimonials for brand marketing.

## 💾 Output Files

- `sentiment_analysis_output.csv`: Cleaned and analyzed dataset with sentiment labels.
- Visualizations (count plots, bar charts) are displayed in the notebook.

## 📬 Conclusion

This project successfully demonstrates how NLP techniques can be applied to extract sentiment-based insights from social media text. Using tools like NLTK and visualizing trends helps brands understand public perception and make data-driven decisions.

## Author

Satyam Theurkar
Task 1 – Internship Project
Big Data Analysis using PySpark

## License

This project is licensed under the MIT License.

