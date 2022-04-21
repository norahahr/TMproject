# Text Mining Project

## Abstract
Throughout the project we are going to perform a sentiment analysis on (Australian) news headlines in a study of gendered language in English. The main aim of the project is to investigate whether the sentiment in the reporting changes with gender. We will perform sentiment analysis on gendered headlines (headlines including gender-inclusive language and gendered pronouns) and compare the sentiment between headlines featuring men and women. Our research hypothesis it that there is a stronger positive association with male-gendered headlines than female ones. The underlying motivation for leading this investigation is to create awareness about possibly embedded gender biases within newspaper’s headlines. This would ideally encourage further research regarding possible repercussions on readers’ perception and attitude towards the subsequent article.

## Research questions
- How do news headlines portray the perception of gender?
- How does use of gender-inclusive language in news reports affect the reporting/content?
- Is there a significant difference between how men and women are portrayed?


## Dataset
[A Million News Headlines](https://www.kaggle.com/datasets/therohk/million-headlines)
- Headline published over 18 years
- Headlines only from the australian ABC newspaper (Australian Broadcasting Corporation)
- The dataset is a CSV file that contains two labels per datapoint, namely the date of publication as well as the headline itself (text in english, lowercase)
- The data was collected from early 2003 to the end of 2020
- The headlines include major international events as well as some more australian focused happenings

## A tentative list of milestones for the project
- Filter out irrelevant headlines (non-gendered)
- Classify headlines into “male”- or “female”-gendered
- Part of speech tagging the relevant headlines
- Looking at verbs, adjectives and adverbs
- Sentiment analysis, classification into positive and negative sentiments of the PoS in question (this process will also require a sentiment dataset, not yet decided upon.)
- Compare results between male and female sentiment

## Sources

[The Social Perception of Heroes and Murderers: Effects of Gender-Inclusive Language in Media Reports](https://www.frontiersin.org/articles/10.3389/fpsyg.2016.00369/full)


[Good Secretaries, Bad Truck Drivers? Occupational Gender Stereotypes in Sentiment Analysis](https://arxiv.org/pdf/1906.10256.pdf)

[A Sentiment Analysis of Language & Gender Using Word Embedding Models](https://academicworks.cuny.edu/cgi/viewcontent.cgi?article=3473&context=gc_etds)
-graduate work

[Mitigating Gender Bias in Natural Language Processing: Literature Review](https://arxiv.org/ftp/arxiv/papers/1906/1906.08976.pdf)

## Documentation
