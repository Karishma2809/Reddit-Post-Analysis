# Reddit Post Analysis

This repository hosts the project on analyzing Reddit posts from the Petioles subreddit, focusing on cannabis consumption and cessation. The project employs Large Language Models (LLM) and General AI for text mining, along with various natural language processing techniques such as sentiment analysis with VADER and emotional analysis with BERT. The aim is to extract deep insights into the patterns of cannabis use, reasons for cessation, and the emotional and sentiment dynamics within the community discussions.

## Table of Contents
- [Project Overview](#project-overview)
- [Objective](#objective)
- [Dataset](#dataset)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Analysis Techniques](#analysis-techniques)
  - [Sentiment Analysis with VADER](#sentiment-analysis-with-vader)
  - [Emotional Analysis with BERT](#emotional-analysis-with-bert)
  - [LLM Model and Prompt Engineering](#llm-model-and-prompt-engineering)
- [Findings](#findings)
- [Project Deliverables](#project-deliverables)
- [Installation](#installation)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Project Overview
Cannabis, also known as marijuana, is one of the most used psychoactive substances. In 2023, 17% of Americans reported that they smoke marijuana, and approximately half of the population stated that they have tried it at some point. However, some users seek to quit for various personal, health, or professional reasons.

Platforms like Reddit provide unique insights into personal experiences and community support regarding substance cessation. The Petioles subreddit is rich with discussions, advice, and shared experiences about quitting cannabis. This project aims to analyze the posts in this subreddit using advanced text mining and NLP techniques to understand the reasons for consumption and the methods used for quitting.

## Objective
The primary objective is to collect and analyze Reddit posts from the Petioles subreddit to understand the reasons for cannabis consumption and the methods used for quitting.

1. **Exploration Using LLMs:**
   - Investigate Reddit posts to identify underlying patterns and motivations.
   - Use Large Language Models (LLMs) to explore and interpret user discussions.

2. **Examine Consumption Patterns:**
   - Investigate reasons for cannabis use and strategies individuals employ to reduce or quit consumption.
   - Identify common triggers, methods, and psychological factors.

3. **Sentiment and Emotional Analysis:**
   - Apply sentiment analysis tools to assess the emotional tone of posts.
   - Gain insights into the emotional states associated with different stages of consumption and cessation.

4. **Social Support Analysis:**
   - Examine the relationship between social support (measured by upvotes) and the content of posts.

## Dataset
The dataset contains Reddit posts from the Petioles subreddit:

### Columns
- **Author:** The Reddit username of the post's creator.
- **Title:** The heading or title of the Reddit post.
- **Score:** The number of upvotes a post has received.
- **Created:** The date and time when the post was made.
- **Link:** Direct URL to the Reddit post.
- **Text:** The full text content of the post.
- **URL:** Any external links included within the post.

### Data Collection Source
- Subreddit: `/r/Petioles`
- Data Archive: [Redarcs Dataset](https://the-eye.eu/redarcs)

## Data Cleaning and Preprocessing
1. **Removing Null Values:** Posts with null values in key fields like 'Text' or 'Author' were removed.
2. **Word Count Filtering:** Removed posts with less than 30 words to ensure meaningful analysis.
3. **Removing Duplicates:** Posts with duplicate usernames, post titles, or full posts were removed.
4. **Renaming Variables:** Columns were renamed for clarity.

## Analysis Techniques

### Sentiment Analysis with VADER
- **Purpose:** Evaluate the sentiment of posts (positive, negative, neutral, and compound scores).
- **Insights:**
  - Identified sentiment trends in posts.
  - Correlated sentiment scores with post engagement (upvotes) and post length (word count).

### Emotional Analysis with BERT
- **Purpose:** Evaluate the emotions (like happiness, sadness, anger) in posts using the text-2-emote approach and transformer model technology.
- **Insights:**
  - Identified emotional trends (e.g., Sadness, Joy, Anger).
  - Correlated emotional scores with user interactions like upvotes.

### LLM Model and Prompt Engineering
- **Model Used:** ChatGPT-4 for its advanced natural language understanding and generation capabilities.
- **Prompt Engineering:** Customized prompts were designed to extract specific information and insights from the data.
- **Application of LLM in Project:**
  - **Theme Identification**
  - **Reason Identification**
  - **Strategy Identification**
  - **Support Identification**

## Findings
1. Approximately 20% of users consume cannabis for recreational enjoyment and relaxation, while 30% discontinue use due to health concerns.
2. Over half of the users consume cannabis daily.
3. Most users prefer a gradual approach to quitting rather than abrupt cessation.
4. Sentiments expressed in the posts are generally positive, but positivity has declined in recent years, likely due to COVID-19.
5. Emotional analysis reveals significant expressions of sadness and fear during the quitting process.
6. A significant increase in posts and user engagement was observed from 2020 onward, likely related to increased stress levels during the pandemic.

## Project Deliverables
- **Presentation Deck:** Detailed Presentation of Analysis [Detailed Presentation Deck.pptx](path/to/Detailed_Presentation_Deck.pptx)
- **Code Notebooks:**
  - [Theme Analysis](path/to/Basic_analysis_on_Theme.ipynb)
  - [Sentiment Analysis using VADER](path/to/Sentiment_Analysis_using_VADER.ipynb)
  - [Emotion Scores using BERT](path/to/Emotion_scores_using_BERT.ipynb)
  - [Regression Analysis on Full Post](path/to/Regression_Analysis_on_Full_Post.ipynb)
  - [Regression Analysis on Post Title](path/to/Regression_Analysis_on_Post_Title.ipynb)

## Installation
To run the analysis notebooks and reproduce the results, you need Python and Jupyter Notebook. Follow the steps below to install the necessary packages:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Karishma2809/Reddit-Post-Analysis.git
   cd Reddit-Post-Analysis
