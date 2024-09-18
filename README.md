# CryptoClustering

## Background

In this challenge, we’ll use our knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Approach

1. Prepare the Data
   - Use the `StandardScaler()` module from `scikit-learn` to normalize the data from the CSV file.
2. Find the Best Value for k Using the Original Scaled DataFrame
   - Use the elbow method to find the best value for `k`
3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data
   - Cluster the cryptocurrencies for the best value for `k` on the original scaled data
4. Optimize Clusters with Principal Component Analysis
   - Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
   - Retrieve the explained variance to determine how much information can be attributed to each principal component
5. Find the Best Value for `k` Using the PCA Data
   - Use the elbow method on the PCA data to find the best value for `k`
6. Cluster Cryptocurrencies with K-means Using the PCA Data
   - Cluster the cryptocurrencies for the best value for `k` on the PCA data

## Folders and Files

- [Resources](https://github.com/blmccourt/CryptoClustering/tree/main/Resources) Folder with provided crypto_market_data.csv file
- [Crypto_Clustering.ipynb](https://github.com/blmccourt/CryptoClustering/blob/main/Crypto_Clustering.ipynb) Jupyter notebook with python code.