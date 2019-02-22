# Project Table of Contents:
* Gathering Data
* Assessing Data for this Project
* Cleaning Data for this Project
* Storing, Analyzing, and Visualizing Data for this Project
* Reporting for this Project


# Goal:
Wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations.


# Introduction of Data Set :
The dataset is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.


## 3 Data Sets: 
* twitter_archive_enhanced.csv ( download manually ) 

* image_predictions.tsv 
The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

* tweet_json.txt 
Each tweet's retweet count and favorite ("like") count at minimum, and any additional data you find interesting. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count. Note: do not include your Twitter API keys, secrets, and tokens in your project submission.

### Three data sets are provided in my project folder. You can download directly.
please keep the data set as it is. Do not try to put twitter-archive-enhanced.csv and twitter-archive-master.csv into project4_data folder

# What Software Do I Need?
* pandas
* NumPy
* requests
* tweepy
* json


