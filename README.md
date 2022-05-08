# AmazonProductSearchOptim
This project is to classify each match between Amazon's query and product into four classes (ESCI) which are used to measure the relevance of the items in the search results: Exact (E), Complement (C), Substitute (S), Irrelevant (I). We proposed multiple methods using transformer-based models, graph-based models and machine learning models. Explicitly, we show how we apply transformer models to get embeddings from queries and product search results and the distance between the embedding space of queries and products to be used as features for graph neural networks and machine learning models. We also show how we use query and product to create graph and build GNN model.

# Quick Navigation
[Background](#background)  
[Data](#data)  
[Models](#models)  
[Repo Structure](#repo-structure)  
[Contact Info](#contact-info)  


# Background  

In recent decades, modern online shopping platforms (e.g. Taobao, eBay, Amazon) have become increasingly important in people’s daily life. Amazon, as one of the most influential e-commerce companies in the world, serves active users from different countries to find what they need from billions of products. Product search is also an essential part of Amazon contributing to almost the largest percentage of transactions among all channels. Since a small number of irrelevant items can break the user experience, Amazon is trying to improve the user experience and user engagement with search. One challenge for their product search is correctly classifying items in a multilingual environment for a particular user search query for shopping. To deal with this challenge and increase the semantic matching of queries and products, we will mainly focus on product classification in this paper. To be specific, we will break down relevance into the following four classes (ESCI) which are used to measure the relevance of the items in the search results: Exact (E), Complement (C), Substitute (S), Irrelevant (I). With the correct classification, the search engine can reduce the number of irrelevant products in a particular user search query so as to increase the user experience and maintain a dominant position in a highly competitive market.

# Data

The dataset is provided by Amazon KDD cup: https://www.aicrowd.com/challenges/esci-challenge-for-improving-product-search#timeline

# Models

fabriceyhc/bert-base-uncased-amazon_polarity, Graph-Based Neural Network, SVM, KNN, Random Forest

# Repo Directory Structure

The repository contains files for AmazonProductSearchOptim project, coding and other related materials.

Details:

- README.md: overall introduction and information of the project

- 10-DataCleaning.ipynb: Python coding notebook for data cleaning and data joining

- 11-GetEmbeddings.ipynb: Python coding notebook for get embedding space and calculate the cosine similarity

- 20-EDA.ipynb: Python coding notebook for exploratory data analysis on products table

- 31-heteograph-approach-2D.ipynb Python coding notebook for creating graph and building GNN using data with 2 dimensions

- 31-heteograph-approach-768d.ipynb Python coding notebook building GNN using data with 768 dimensions

- 31-heteograph-approach-88D.ipynb Python coding notebook for building GNN using data with 88 dimensions

- 32-ML-models.ipynb Python coding notebook for using machine learning methods, such as KNN, SVM, RandomForest


Explanation:

The repo is structured as follows: All *0- (e.g., 10-, 20-, 30-) files contain finalized work for the purpose described (e.g., "process-data"). Subfiles related to the task (e.g., 11-, 12-) should be created in order to explore and document relevant or interesting subtasks.

# Contact Info

- Zihan Fang zihan.fang@vanderbilt.edu

- Weiqing Huang weiqing.huang@vanderbilt.edu

- Yuechen Yang yuechen.yang@vanderbilt.edu
