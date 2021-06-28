# Topic modeling and sentiment analysis for Airbnb text data
 The final project of my text mining course
## Table of Contents
1. Installation
2. Project Motivation
3. Data Description

## 1. Installation
  [python (>=3.6)](https://www.python.org/downloads/)\
  [pandas](https://pandas.pydata.org/)\
  [numpy](https://numpy.org/)\
  [sklearn](https://sklearn.org/)\
  [nltk](https://www.nltk.org/)\
  [html.parser](https://docs.python.org/3/library/html.parser.html)\
  [pattern3](https://pypi.org/project/pattern3/)\

## 2. Project Introduction
In this project, our group analyzed text data in the listings and reviews dataset of the Airbnb Boston Area from September 2009 to February 2021. Specifically, we focused on neighborhood description, room description, and customer reviews.
We identified neighborhood themes, room characteristics, and customers' preferences for those themes and characteristics; we also explored customers' considerations when giving reviews and the relationship between numeric rating and text reviews. Based on those findings, we provided three pieces of operation and marketing suggestions for Airbnb.
• Provide coupons if renters write comments of more than 30 words.
• Target customers based on their preferences and provide content-based recommendation
• Exploit more rooms a little bit far from downtown but can give renters a good experience.
We performed sentimental analysis and topic modeling. For sentimental analysis, we chose the VADER model, considering slang, punctuation, capital words, and syntax. We excluded reviews with a foreign language for convenience. For topic modeling, we first normalized and vectorized and then chose the Latent Dirichlet Allocation (LDA) method.

## 3. Data Description

We found publicly available data of Airbnb on the [Inside Airbnb](http://insideairbnb.com/get-the-data.html). The data have been cleansed and aggregated by the website. We use Boston listings data scrapped in February 2021 and reviews data from August 2009 to February 2021. The data could be download at 
There are two CSV files, "listings.csv" and "reviews.csv" which contain information about rooms listed on Airbnb and customer reviews for those rooms. The listings dataset has 74 columns. For topic modeling, we chose "description" which describes the room, and "neighborhood_overview" which describes the overall environment. The reviews file has six columns; we used the column "comments" which listed each customer's review of the rental experience to conduct topic modeling and sentiment analysis. There are 2960 rows in the listings dataset and 109,721 rows in the reviews dataset.
