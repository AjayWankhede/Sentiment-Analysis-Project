# Amazon Product Reviews Sentiment Analysis

## Introduction: 
  Natural Language Processing (NLP) is a hotbed of research in data science these days and one of the most common applications of NLP is sentiment analysis. From opinion polls to creating entire marketing strategies, this domain has completely reshaped the way businesses work, which is why this is an area every data scientist must be familiar with. 
  In this Project we train our model and also predict the sentiment of Amazon product as Positive or Negative. 
 
## Objective:
  Reviews on Amazon are not only related to the product but also the service given to the customers. If users get clear bifurcation about product reviews and service reviews it will be easier for them to take the decision, in this analysis we propose a system that performs the classification of customer reviews followed by finding sentiment of the reviews. A rule based extraction of product feature sentiment is also done. Also we provide a visualization for our result summarization.

# Project Architecture / Project Flow:
 1) Product Selection
 2) Reviews Extraction
 3) Preprocessing of Data
 4) Data Visualization
 5) Sentiment Analyser
 6) Feature Engineering
 7) Model Building
 8) Model Evaluation
 9) Deployment using Streamlit

## Product Selection:
  We have selected the product DR VAKU® Swadesi Pulse Oximeter. We selected this product due to ongoing COVID-19 Pandemic and such products is play important roles in this phase. We believe that such products can be very useful to deal with such big issues. We have to improve such products so that people can get the right information and also can take right decisions based on that information. Link:https://www.amazon.in/DR-Oximeter-Fingertip-Monitor-Approved/dp/B08D3KXF9Y/ref=cm_cr_arp_d_product_top?ie=UTF8&th=1
 
## Reviews Extraction:
  We used web scraping to extract the review from Amazon. We use ***Beautiful, Request, Pandas*** libraries to extract the reviews.
import requests
from bs4 import BeautifulSoup
import pandas as pd

## Preprocessing of Data / EDA:
Exploratory Data Analysis is the process of investigating the dataset to discover patterns and get insights from it.
We perform some action to get better insights:

a) Visualize Ratings
b) Combine All The Reviews In One Row
c) Remove Punctuation Marks
d) Perform Tokenization
e) Remove Stopwords
f) Perform Normalization
g) Visualize WordCloud

## Sentiment Analyser:
 We use ***Vader Sentiment Intensity*** analyser for this project which classify reviews in either Positive or Negative.
 from nltk.sentiment.vader import SentimentIntensityAnalyzer
 
## Feature Engineering:
We used ***Count Vectorizer*** for Feature extraction which convert text to numerical data i.e text is transformed to a sparse matrix form.
 
## Model Building and Evaluation:
  Followings models we are used for better result and Analysis:
1) Bernoulli Naïve Bayes
2) Gaussian Naïve Bayes
3) Multinomial Naïve Bayes
4) Random Forest Classifier
5) Decision Tree Classifier
6) Support Vector Machines
7) Logistic Regression
8) Extra Trees Classifier
9) AdaBoost Classifier
10) Gradient Boosting Classifier
11) Voting Classifier (Soft and Hard)

From which we choose ***Soft Voting Classifier*** in which we Combine  Logistic Regression, AdaBoost, Bernoulli Naive Bayes, and Multinomial Naive Bayes Models
to get good values of Precision, Recall and F1 Score.

## Deployment:
 We use Streamlit Library for deploy our model.





	
 
