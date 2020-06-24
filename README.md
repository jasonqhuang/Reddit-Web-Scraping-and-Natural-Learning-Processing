# Project 3 - Web APIs & NLP (Reddit)

### Executive Summary


Using Pushshift API, posts were web scraped from Reddit.com with the purpose of creating a Natural Language Processing (NLP) model that can predict the original subreddit. 

The data was saved to dataframes and combined to create a large dataset. The data was then cleaned with exploratory data analysis to check for nulls and missing values. Title text was then tokenized and lemmatized to get into a work-able form for our models. The data went through CountVectorizer, TD-IDF, and Multinomial Naive Bayes models. A confusion matrix was created and accuracy metrics were determined. The model was iterated while changing the pipeline gridsearch parameters to determine the best score for each model. 

#### Background

Whiskey and Whisky are two ways to refer to the popular liquor. The respective subreddits hold multiple daily posts referrring to the drinks. 

#### Problem Statement

How well does a model perform at determining if a post came from the bourbon or scotch subreddits?

#### Data

Imports
Webscraping
Combine Dataframes
EDA
Lemmatizing
Stopwords
Baseline Model
Countvectorizer
TF-IDF
Multinomial Naive Bayes
Confusion Matrix
Word Frequency Visualization

### Data Dictionary

| Predictive Variable | Data type | Description |
  ------------------- | --------- | ----------- 
| title | ordinal | Title Text |
| selftext | ordinal | Text in post |
| subreddit | Ordinal | Original subreddit of post |


### Conclusions/Recommendations

The model performed very well with a score of 84.5% and accuracy of 84.5%. This can be attributed to very specific words making it easy to determine original subreddit. To improve the model, adding comments and searching for flavor profile text can improve the complexity of the model. 