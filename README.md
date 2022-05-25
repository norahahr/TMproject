# Text Mining Project

## Abstract
In the following project we are going to perform a topic modelling on news headlines. The goal of the project is to compare the distribution of topics in an informal context of Reddit news headlines and a formal newspaper’s headlines. The investigation is guided by the hypothesis of finding an overrepresentation of some more polarized topics in the informal context, as opposed to the null hypothesis that there is no significant difference in topic distribution between both types of headlines. Finding a statistically significant difference would be for instance helpful in the discipline of media studies; understanding how polarization emerges from different news channels.

## Research questions
-	Does there exist an overrepresentation of controversial topic in an informal news source such as Reddit?

## Dataset
[Reddit Worldnews](https://www.kaggle.com/datasets/rootuser/worldnews-on-reddit)
### Reddit Worldnews headlines:
-	The dataset is in the form of a CSV file
-	Each datapoint is characterized by 8 features namely “Time created” (Unix timestamp of submission date), “Date created” (creation time in Year-Month-Day format), “Up votes” (how often upvoted), “Down votes”(how often downvoted), “Title” (the headline), “Over 18” (if accessible to minors), “Author” (reddit username of author) and “Subreddit” (the subcategory in reddit, always Worldnews)
-	The categories made use of in our work will be only the “Title” column
-	The dataset contains data collected between 2008 and 2016

[Irish Times News](https://www.kaggle.com/datasets/therohk/ireland-historical-news)
### Irish Times headlines:
-	We chose this dataset since it presented the most global headlines of the datasets we found
-	The dataset contains 1.61 million headlines collected over 25.5 years (mostly about European events)
-	The file is in CSV format
-	The file contains three features per datapoint namely “Publish date”, “Headline category” and “Headline”
-	Again, we will focus on the headline column and will need to exclude especially the categories in order to be able to perform clustering without biasing our model


## A tentative list of milestones for the project
1.	Tokenizing headlines of both datasets
2.	Lemmatization the headlines
3.	Create sentence embeddings
4.	Calculate sentence embeddings similarity measures
5.	Visually present the embeddings on a similarity vector space (dimensionality reduction)
6.	Manually distinguishing some topics
7.	Applying a clustering method
8.	Compare the topic distributions through a statistical testing
9.	Conclude whether some topics are over/underrepresented in an (in)formal news context

## Sources
[Twitter for Sparking a Movement, Reddit for Sharing the Moment: #metoo through the Lens of Social Media](https://arxiv.org/abs/1803.08022)

#### Non-Academic sources
LDA:
[Topic Modeling in Python: Latent Dirichlet Allocation (LDA)](https://towardsdatascience.com/end-to-end-topic-modeling-in-python-latent-dirichlet-allocation-lda-35ce4ed6b3e0)

Sentence embeddings:
[Top 4 Sentence Embedding Techniques using Python](https://www.analyticsvidhya.com/blog/2020/08/top-4-sentence-embedding-techniques-using-python/)
[Clustering Sentence Embeddings to Identify Intents in Short Texts](https://towardsdatascience.com/clustering-sentence-embeddings-to-identify-intents-in-short-text-48d22d3bf02e)

## Documentation
HDBSCAN: https://github.com/scikit-learn-contrib/hdbscan
