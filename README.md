# Wikipedia-Article-Clustering

### Data
The July 1st, 2023 Wikipedia snapshot data used for the clustering is from [Kaggle](https://www.kaggle.com/datasets/jjinho/wikipedia-20230701). It was not included in the repo as it was far too large. Use the Kaggle link to access the same data.

### Usage
``Project2_1.ipynb`` is the first file that must be run. This performs a random sample of the data to create a smaller, but still diverse, dataset for the clustering to run on. Due to the limitations of my machine, only 2% of the data was kept, but this could be changed on a machine with more capacity. 

Next, the data is custered using K-Means in ``Project2_2.ipynb``. The generated clusters will be saved to the project folder (but are not included here due to storage constaints) and their counts are stored in ``Topic_Counts.csv``. This notebook will also calculate the similarity scores of the clusters and a random sample as a baseline and then save them in ``cosine_similarity_scores.csv``.

Last, ``Project2_3.ipynb`` is run to evaluate the similarity of the categories given in the Wikipedia corpus. The random categories used and their counts and similarity scores will be saved in ``given_categiry_cosine_similarity_scores.csv``

### Viewing an Article
To view an article more easily for analysis, instead of manually looking through the article in one line in the ``.csv`` files, you can simply put the article title into the *article_title* field of ``DisplayArticle.ipynb``

### Graphs
The graph included in the paper was created using the code in ``graphs.ipynb``.
