# Text Mining Project

## Abstract
In the following project we are going to perform a topic modelling on news headlines using two different methods, namely Latent Dirichlet Allocation (LDA) and HDBSCAN clustering. The goal of the project is to compare the proportion of polarizing topics within  an informal context (Reddit r/worldnews) as compared to a formal newspaper’s headlines (The Irish Times). It is hypothesized that an overrepresentation of polarized topics exists in the informal context, as opposed to the formal news source. Improving understanding on the emergence of polarization through quantifying topic representation is relevant to complement research conducted on this within social sciences disciplines like media studies and political sciences. 

## Research question
-	Does there exist a significant difference in coverage of polarizing topics in the headlines of the informal Reddit r/worldnews news source as compared to the formal Irish Times newspaper?

## Documentation
Clustering.ipynb and LDA.ipynb are the main code files. 
For convenience both files contain the basic preprocessing pipeline as well as the respective topic modeling method. Thus, the files can be runned in any desired order.
The datasets need to be downloaded beforehand, as indicated within the code files. Links to the datasets can be found in the section below.
The TM pres.pdf file contains the slides used for the project presentation.

## Dataset

### Reddit Worldnews headlines:
[Reddit Worldnews](https://www.kaggle.com/datasets/rootuser/worldnews-on-reddit)
-	The dataset is in the form of a CSV file
-	Each datapoint is characterized by 8 features namely “Time created” (Unix timestamp of submission date), “Date created” (creation time in Year-Month-Day format), “Up votes” (how often upvoted), “Down votes”(how often downvoted), “Title” (the headline), “Over 18” (if accessible to minors), “Author” (reddit username of author) and “Subreddit” (the subcategory in reddit, always Worldnews)
-	The categories made use of in our work will be only the “Title” column
-	The dataset contains data collected between 2008 and 2016

### Irish Times headlines:
[Irish Times News](https://www.kaggle.com/datasets/therohk/ireland-historical-news)
-	We chose this dataset since it presented the most global headlines of the datasets we found
-	The dataset contains 1.61 million headlines collected over 25.5 years (mostly about European events)
-	The file is in CSV format
-	The file contains three features per datapoint namely “Publish date”, “Headline category” and “Headline”
-	Again, we will focus on the headline column and will need to exclude especially the categories in order to be able to perform clustering without biasing our model


## List of milestones for the project
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
LDA:
[Topic Modeling in Python: Latent Dirichlet Allocation (LDA)](https://towardsdatascience.com/end-to-end-topic-modeling-in-python-latent-dirichlet-allocation-lda-35ce4ed6b3e0)

Sentence embeddings:
[Top 4 Sentence Embedding Techniques using Python](https://www.analyticsvidhya.com/blog/2020/08/top-4-sentence-embedding-techniques-using-python/)
[Clustering Sentence Embeddings to Identify Intents in Short Texts](https://towardsdatascience.com/clustering-sentence-embeddings-to-identify-intents-in-short-text-48d22d3bf02e)
[Top2Vec: Distributed Representations of Topics (Angelov, 2020)](https://arxiv.org/pdf/2008.09470.pdf)

HDBSCAN:
https://github.com/scikit-learn-contrib/hdbscan
