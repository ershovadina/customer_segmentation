# Ironhack Final Project: E-commerce Customer Segmentation

*[Berlin, March 2021]*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Links](#links)

## Project Description
The objectives of this project are:
* to do a customer segmentation based on RFM (recency, frequency and monetary value) analysis using ML Clustering Models
* to develop recommendations on customized marketing strategies

## Dataset
* The dataset was taken from [Kaggle](https://www.kaggle.com/olistbr/brazilian-ecommerce).
* Brazilian E-Commerce Database by Olist - department store in Brazilian marketplaces.
* 98,666 orders by 96,096 unique byers from 3,095 sellers during 22 months (2016-2018).
* Olist customers are merchants that are selling their products through the Olist Store (on marketplaces).

## Cleaning and Preprocessing
* Joining datasets in Jupyter Notebook
* Aggregating by seller_id
* Feature engineering (RFM):
     - Recency_max - number of days since the last order
     - Frequency - total number of orders
     - Monetary_value - average payment_value per order
 * Data Transformation, scaling

## Model Training and Evaluation
* The following clustering models were applied and evaluated:
    - K-means Clustering
    - DBSCAN - Density-Based Spatial Clustering
    - Mean Shift Clustering
    - Agglomerative Hierarchical Clustering
* The model performances were compared using the silhouette score
* K-means showed the best performance on the used data

## Conclusion
* Using K-means Clustering 3 seller clusters were identified based on recency, frequency and monetary value:
    - Cows - active with average/stable order payment value -> Action: maintain relationships
    - Dogs - inactive and cheap sellers - > Action: do not waste time & effort 
    - Opportunities - high order value, but churn/dormant - > Action: special marketing campaigns, discounts, recommend to byers

## Links

[Tableau](https://public.tableau.com/profile/dina.ershova#!/vizhome/customer_segmentation_16154137364710/Dashboard1?publish=yes/)
  
[Slides](https://www.canva.com/design/DAEYevry7y8/share/preview?token=Z0LjFjJJGpoA3uA47c_Rng&role=EDITOR&utm_campaign=designshare&utm_source=sharebutton)  