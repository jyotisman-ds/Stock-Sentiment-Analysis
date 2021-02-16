# Stock-Sentiment-Analysis

- [Overview](#overview)
- [The problem](#the-problem)
- [Technical Details](#technical-details)
- [Credits](#credits)

## Overview

We look at a NLP problem here related to sentiment prediction for stock markets. It leverages a curated dataset that was provided as part of an in-depth course in Udemy on
[machine learning in Finance](https://www.udemy.com/course/ml-and-python-in-finance-real-cases-and-practical-solutions/). I use several well known techniques commonly used in NLP for preprocessing the texts like *stopwords* removal, *stemming*, *lemmatizing*, etc before training through various techniques.


## The problem

- To rate sentiments on social media platforms like Twitter, Facebook, etc.
- Here, we specifically look at texts relating to stock market sentiments. This in turn could predict present or future stock market behavior of specific companies in real time!

## Technical Details

- The details are in the [notebook](https://github.com/jyotisman-ds/Stock-Sentiment-Analysis/blob/main/Stocks_Sentiment_Analysis.ipynb). Cleaning techniques include *stopwords* removal, *stemming* and *lemmatizing*. The dataset consists of around 6000 texts with labelled sentiment as a binary variable.
- Since we do a word level classification here, a powerful technique to visualize words in a corpus influencing a particular sentiment is *WordCloud*. It highlights the most frequently occurring words. One such image is shown for negative stock sentiment below.  

![cluster1](/negative.png)

- For training, we use a lemmatized version. The problem with a stemmed version is the creation of several meaningless words that results from incorrect stemming of certain words.
- We only use deep learning techniques here. First, we train with a simple model consisting of a Conv and Dense layers and this alone achieves good accuracy. A more sophisticated sequence model is also used but it does not really improve upon the former.

_Tools : python, nltk, TensorFlow, Keras, WordCloud, pandas, gensim, seaborn_

## Credits

I am deeply thankful to Udemy and all the instructors for hosting this wonderful course for [machine learning in Finance](https://www.udemy.com/course/ml-and-python-in-finance-real-cases-and-practical-solutions/). My curiosity to learn Machine Learning/deep learning applications led me to this course and I am glad not only to have learnt some useful techniques but also a great deal about the world of finance in general.
