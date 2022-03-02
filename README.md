
# People influence People

Recommender systems are part of our daily life. It doesn't matter where. We do appreciate a good suggestion. Recommender systems are a win-win game for both service providers' and users' sides. They reduce transaction costs of finding and selecting items in an online shopping environment. 

The two most common types of recommender systems are ***Content-Based*** and ***Collaborative Filtering***. While the first one uses item features to recommend the other items similar to what the user likes, Collaborative Filtering uses the "wisdom of the crowd" to recommend. 

Collaborative Filtering methods or "CF" methods are more common because they can lead to better results and are relatively easy to implement. CF can be divided into memory-based and model-based techniques. In this notebook, I will focus on implementing the ***low-rank matrix factorization*** method as part of the model-based CF technique to recommend top K movies to any desired user.


Since there are not many user-rating movie datasets out there, I'll use a relatively small Movielens dataset which is available [here](https://grouplens.org/datasets/movielens/latest/).

* Gathered and loaded MovieLens dataset
* Performed an exploratory data analysis and observed long-tail problem
* Made user predictions regarding each movie using low-rank matrix factorization (with the help of singular value decomposition)

![MovieLens](movie-lens.jpg)