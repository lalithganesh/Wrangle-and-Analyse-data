# Wrangle and Analyse We Rate Dogs Twitter data.

This project was done as a part of Udacity's Data Analyst Nano Degree .

# Introduction
In this project, I try to gather data from various sources, clean and tidy up the data and perform analysis.
Data was gathered from a csv file, twitter and udacity server.

# Tools Used
- Jypyter Notebooks - Environment used for the project
- Python - Programming language in which the analysis was done
- Python libraries :
  - Numpy and Pandas for Data Wrangling
  - requests to download data
  - tweepy to access twitter data
  - json to handle json data from twitter
  - beautiful soup to parse data from html tag
  - Matplotlib for Data Visualization


# Summary of Findings

The following issues were found and cleaned:

Quality Issues
df_twitter
 - tweet_id is of type int instead of str
 - source column has text content within anchor tag
 - timestamp is of type datatype object instead of datetime
 - retweeted_status_id and retweeted_status_user_id are of type float instead of string
 - retweeted_status_timestamp is of type datatype object instead of datetime
 - in_reply_to_status_id and in_reply_to_user_id are of type float instead of string
 - values other than 10 in rating_denominator
 - extreme values of 10 and 1776 in numerator
 - Animals other than dogs are also present in the tweets. Many of them are also given ratings
df_twitter_new
 - tweet_id is of type int instead of str
 - Rows are lesser than that of df_twitter.Total rows = 2342. No of rows in df_twitter = 2356
df_img
 - tweet_id is of type int instead of str
 - img_num is of type instead of category
 - Rows are lesser than that of df_twitter. Total rows = 2075. No of rows in df_twitter = 2356

Tidyness Issues
 - According to the rules of tidy data, df_twitter_new can be merged with twitter archieved dataframe to form a single observational unit
 - Dog stages doggo,floofer, puppo, pupper are in seperate columns

- Most of the dog rating tweets that are favourited were also retweeted.
- People those who have responded to these tweets like puppo's and doggo's relatively more and pupper's were the least favourite.


