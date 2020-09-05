# Improvised Fake News Classification using Page Rank Algorithm
Prototype for Combining Page Rank algorithm along with Fake News Classification for combating misinformation better


The goal is to better identify fake news articles from the web. The idea is that the pages with Fake news would be referenced far less often than official, more reliable webpages, hence causing the pages containing fake news to appear far less frequently. Therefore, the rank of a webpage found from an algorithm such as the Pagerank algorithm would help us identify fake news articles better.

The work done is as follows:

1. Using the given dataset, a classifier that classfies fake news articles is built
2. The pagerank algorithm is implemented using dataproc on google cloud over a cluster by creating a dummy dataset input to it. (using pyspark)
3. The output of the pagerank gives ranks to each of the URLs
4. Using the rank of each column we can add a new feature to the dataset and compare accuracy.
After trying multiple models, it was found SVMs worked better. Sklearn was used for implementing the SVC.
