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

[The Social Perception of Heroes and Murderers: Effects of Gender-Inclusive Language in Media Reports](https://www.frontiersin.org/articles/10.3389/fpsyg.2016.00369/full)


[Good Secretaries, Bad Truck Drivers? Occupational Gender Stereotypes in Sentiment Analysis](https://arxiv.org/pdf/1906.10256.pdf)

[A Sentiment Analysis of Language & Gender Using Word Embedding Models](https://academicworks.cuny.edu/cgi/viewcontent.cgi?article=3473&context=gc_etds)
-graduate work

[Mitigating Gender Bias in Natural Language Processing: Literature Review](https://arxiv.org/ftp/arxiv/papers/1906/1906.08976.pdf)

## Documentation
