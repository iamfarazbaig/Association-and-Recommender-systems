# Association and Recommender Systems

This project is split into 2 parts.

First we look at the Association analysis for a popular dataset [Online Retail](http://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx) followed by Recommender Systems for [Movielens](http://www.grouplens.org/system/files/ml-1m.zip) dataset.

* Association Analysis

We begin with a basic data cleaning process followed by an initial visualization of the data to get an idea of where significant data lies. 
With the key sets of items within the dataset identified, we apply the association rules to discover purchase behavior patterns. Then we filter the rules by looking only at the cases having large life and high confidence values. This gives us an opportunity to use the popularity of one product to increase the sales of another.

* Recommender Systems

We use the well-known MovieLens dataset (in this case the 1M version).
The detail about the dataset is in the README[Readme](http://files.grouplens.org/papers/ml-1m-README.txt)
 
 After loading and merging all the the data into one dataframe, we perform exploratory data analysis to find any possible outliers and to observe the data distribution. We then filter the data to a small threshold as it will remain persistent to the data. We plot the data with a histogram over the variance of using count and average values.
 
 Then we use basic prediction algorithms such as SVD, KNNBasic which are supported by the Surprise library. We observe the performance of algorithms by using root mean squared error as the accuracy metric and also taking the time under consideration.
