# Executive Summary for Project 3
## Problem Statement
The goal of this project is to use NLP to correctly predict what subreddit a post is from using text and other features from data collected from reddit using the pushshift API. We will collect posts from the subreddits **r/UnresolvedMysteries** and **r/UnsolvedMysteries** for this project.

We will build several models and determine which has better performance, as measured by accuracy, given that the datasets are balanced and we are working on a classification problem.

## Description of data
Using the Pushshift API, about 1000 submissions (also refered to as posts throughout) to r/UnsolvedMysteries and r/UnresolvedMysteries each were gathered. The features gathered were:
- Author: Subreddits tend to have regular posters/participators. This can be important in predicting what subreddit a submission was posted to.
- Awarders: Appears to be a list of users who have given the post and "award". Same as author: people tend to concentrate on subreddits they like.
- Created UTC: Necessary for API function
- Self Text: Main text content of the post. Probably most important feature.
- Subreddit: TARGET
- Title: Good source of relevant text.

Selftext turned wasn't useful since posts to r/UnsolvedMysteries do not include this feature. Our analysis focused on other features instead: Title and Author.

Data from both subreddits is quite similar, with the exception of author, which varies greatly on each subreddit.

## Models
The following models were built, fit on training data and scored on a holdout test set:
- Multinomial Naive Bayes Classifier using Count Vectorizer and 'title' as it's feature. Best Test Score: 65.28% accuracy.
- Logistic Regression using Count Vectorizer and 'title' as it's feature. Best Test Score: 64.14% accuracy.
- Logistic Regression using Count Vectorizer and 'author' as it's feature. Best Test Score: 75.14% accuracy.
- Decision Tree Classifier using Count Vectorizer and 'author' as it's feature. Best Test Score: 72.68% accuracy.
- Voting Classifier between a Decision Tree Classifier and a Logistic Regression, using Count Vectorizer and 'author' as it's feature. Best Test Score: 72.68% accuracy.

## Conclusions & Recommendations
Subreddits can be predicted using title or author features, though not with great accuracy. Most models are underfit, so further hyperparameter optimization can achieve better results. Only one feature was used for each model. Incorporating several features in a single model along with hyperparameter optimization is the logical next step.

A presentation is included with all relevant information, as well as all code and data used.