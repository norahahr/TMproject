# Text Mining Project

## Abstract
In the following project we are going to perform a topic modelling on news headlines using two different methods, namely Latent Dirichlet Allocation (LDA) and HDBSCAN clustering. The goal of the project is to compare the proportion of polarizing topics within  an informal context (Reddit r/worldnews) as compared to a formal newspaper’s headlines (The Irish Times). It is hypothesized that an overrepresentation of polarized topics exists in the informal context, as opposed to the formal news source. Improving understanding on the emergence of polarization through quantifying topic representation is relevant to complement research conducted on this within social sciences disciplines like media studies and political sciences. 

## Research question
-	Does there exist a significant difference in coverage of polarizing topics in the headlines of the informal Reddit r/worldnews news source as compared to the formal Irish Times newspaper?

## Documentation
[Clustering.ipynb](https://github.com/norahahr/TMproject/blob/main/clustering.ipynb) and [LDA.ipynb](https://github.com/norahahr/TMproject/blob/main/LDA.ipynb) are the main code files. To run the code, clone the repository and use pip to install the requirements from the command line, using ```pip install -r requirements.txt```.
For convenience both files contain the basic preprocessing pipeline as well as the respective topic modeling method. Thus, the files can be runned in any desired order.

The datasets need to be downloaded beforehand, as indicated within the code files. Links to the datasets can be found in the section below and in the code files.
The [TM pres.pdf](https://github.com/norahahr/TMproject/blob/main/TM%20pres.pdf) file contains the slides used for the project presentation and the final report can be found in the file [Report.pdf](https://github.com/norahahr/TMproject/blob/main/Report.pdf).

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

## References
Aggarwal, C. C., Hinneburg, A., & Keim, D. A. (2001). On the Surprising Behavior of Distance Metrics in High Dimensional Space. Database Theory — ICDT 2001, 420–434. https://doi.org/10.1007/3-540-44503-x_27

Allaoui, M., Kherfi, M. L., & Cheriet, A. (2020). Considerably Improving Clustering Algorithms Using UMAP Dimensionality Reduction Technique: A Comparative Study. Lecture Notes in Computer Science, 317–325. https://doi.org/10.1007/978-3-030-51935-3_34

Arbaoui, B., De Swert, K., & van der Brug, W. (2016). Sensationalism in News Coverage: A Comparative Study in 14 Television Systems. Communication Research, 47(2), 299–320. https://doi.org/10.1177/0093650216663364

Azeem, A. A., Hunter, J. A., & Ruffman, T. (2019). News headlines or ideological beliefs: What affects readers’ interpretations of news stories about immigration, killing in the name of religion and other topical issues? A cross-cultural analysis. New Zealand Journal of Psychology, 48(1), 56–61.

Blei, D., Edu, B., Ng, A., Jordan, M., & Edu, J. (2003). Latent Dirichlet Allocation. Journal of Machine Learning Research, 3, 993–1022.

Blom, J. N., & Hansen, K. R. (2015). Click bait: Forward-reference as lure in online news headlines. Journal of Pragmatics, 76, 87–100. https://doi.org/10.1016/j.pragma.2014.11.010

Campello, R. J. G. B., Moulavi, D., & Sander, J. (2013). Density-Based Clustering Based on Hierarchical Density Estimates. Advances in Knowledge Discovery and Data Mining, 160–172. https://doi.org/10.1007/978-3-642-37456-2_14

Campello, R. J. G. B., Moulavi, D., Zimek, A., & Sander, J. (2015). Hierarchical Density Estimates for Data Clustering, Visualization, and Outlier Detection. ACM Transactions on Knowledge Discovery from Data, 10(1), 1–51. https://doi.org/10.1145/2733381

Carothers, T., & O’Donohue, A. (2019). Democracies Divided: The Global Challenge of Political Polarization. Brookings Institution Press.

Chris. (2016). Worldnews on Reddit from 2008 to Today. Kaggle. https://www.kaggle.com/datasets/rootuser/worldnews-on-reddit

Google Code Archive. (2013). word2vec. Google.com. https://code.google.com/archive/p/word2vec/

Kroon, A. C., Trilling, D., & Raats, T. (2020). Guilty by Association: Using Word Embeddings to Measure Ethnic Stereotypes in News Coverage. Journalism & Mass Communication Quarterly. https://doi.org/10.1177/1077699020932304

Kulkarni, R. (2022). Irish Times - Waxy-Wany News. Kaggle. https://www.kaggle.com/datasets/therohk/ireland-historical-news

Majid, A. (2022, March 2). Most popular websites for news in the world: Monthly top 50 listing. Press Gazette. https://pressgazette.co.uk/most-popular-websites-news-world-monthly/

Manikonda, L., Beigi, G., Liu, H., & Kambhampati, S. (2018). Twitter for Sparking a Movement, Reddit for Sharing the Moment: #metoo through the Lens of Social Media. https://doi.org/https://doi.org/10.48550/arXiv.1803.08022

McCoy, J., & Somer, M. (2018). Toward a Theory of Pernicious Polarization and How It Harms Democracies: Comparative Evidence and Possible Remedies. The ANNALS of the American Academy of Political and Social Science, 681(1), 234–271. https://doi.org/10.1177/0002716218818782

McInnes, L., Healy, J., Saul, N., & Großberger, L. (2018). UMAP: Uniform Manifold Approximation and Projection. Journal of Open Source Software, 3(29), 861. https://doi.org/10.21105/joss.00861

Moody, C. E. (2016). Mixing Dirichlet Topic Models and Word Embeddings to Make lda2vec. https://doi.org/https://doi.org/10.48550/arXiv.1605.02019

Pérez-Escolar, M., & Noguera-Vivo, J. M. (2021). Hate Speech and Polarization in Participatory Society. Routledge. https://doi.org/10.4324/9781003109891

Rousseeuw, P. J. (1987). Silhouettes: A graphical aid to the interpretation and validation of cluster analysis. Journal of Computational and Applied Mathematics, 20, 53–65. https://doi.org/10.1016/0377-0427(87)90125-7

Rückle, E., Peyrard, S., & Gurevych, M. (2018). Concatenated Power Mean Word Embeddings as Universal Cross-Lingual Sentence Representations. https://doi.org/https://doi.org/10.48550/arXiv.1803.01400

Wintrode, J. (2011). Using latent topic features to improve binary classification of spoken documents. 2011 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP). https://doi.org/10.1109/icassp.2011.5947615

Yan, R., & Gao, G. (2020). Topic Analysis by Exploring Headline Information. Web Information Systems Engineering – WISE 2020, 129–142. https://doi.org/10.1007/978-3-030-62008-0_9
