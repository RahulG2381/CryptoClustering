# CryptoClustering
# Title: Cryptocurrency Clustering Analysis: Predicting Price Change Effects
# Introduction:

## Objective: Utilize Python and unsupervised learning techniques to predict the impact of duration(time/days)  and the price changes on cryptocurrencies.
# Data Exploration and Preparation:

## Load and Explore Data: 
Load the provided crypto_market_data.csv into a DataFrame and perform initial data exploration.
## Data Normalization: 
Utilize StandardScaler() module to normalize the data, ensuring consistent scales for analysis.
## Feature Selection: 
Create a DataFrame with scaled data, setting "coin_id" as the index for further analysis.

# Finding Optimal Clusters (k):

## Elbow Method: 
Employ the elbow method to determine the optimal number of clusters (k) by plotting inertia values against different k values.
## Interpretation: 
Identify the elbow point as the optimal k value for subsequent clustering.

# Clustering Cryptocurrencies: Original Scaled Data:

## K-means Clustering: 
Initialize K-means model with the optimal k value and fit the model using the original scaled DataFrame.
## Visualization: 
Plot clusters using a scatter plot to visualize the grouping of cryptocurrencies based on price changes.

# Optimizing Clusters with Principal Component Analysis (PCA):

## PCA Analysis: 
Perform Principal Component Analysis on the original scaled DataFrame to reduce features to three principal components.
## Variance Assessment: 
Assess the explained variance of each principal component to gauge information retention.

# Finding Optimal k Using PCA Data:

## Elbow Method on PCA Data: 
Apply the elbow method on the PCA data to determine the optimal k value.
## Comparison: 
Evaluate the difference in optimal k value obtained from PCA compared to the original data.

# Clustering Cryptocurrencies: PCA Data:

## K-means Clustering: 
Initialize K-means model with the optimal k value derived from PCA and fit the model using PCA data.
## Visualization: 
Plot clusters using a scatter plot, highlighting the impact of using fewer features for clustering.

# Analysis and Conclusion:
* Question: What is the total explained variance of the three principal components?
* Answer: 89%


* **Question:** What is the best value for `k` when using the PCA data?
* **Answer:** 4

* **Question:** Does it differ from the best k value found using the original data?
* **Answer:** No
