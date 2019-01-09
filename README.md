# Predicting Category of Reddit Post

![header](Images/reddit.png)

## Goal
Build a classifier that predict category of a given Reddit Post to one of the following categories: Art or Programming

## Data Cleaning
- A list of subreddit titles, classified (Kaggle). We extracted the 21 subreddits EACH classified as ‘arts’ and as ‘programming’ -- balanced data!
- The .tsv file can be found here: https://www.kaggle.com/mswarbrickjones/reddit-selfposts#subreddit_info.csv
- 1,000 reddit posts from every subreddit - we pulled 42,000 posts from our 42 subreddits

## Data Preprocessing / Feature Engineering
Given clean, merged data, we used NLTK to tokenize, lemmatize and filter the data, giving us 95,000 unique features (words). From there we vectorized the data via TF-IDF calculation and dropped words below a threshold of 0.0001, words such as 'abcdefghijklmnopqrstuvwxyz'. This left us with around 5,000 words to model!

## Visualization of Data in Reduced Dimensions
![header](Images/2d.png)

![header](Images/3d.png)

## Performance of ML Models
![header](Images/evaluation.png)

## Winner Winner Chicken Dinner!
![header](Images/mnb.png)
