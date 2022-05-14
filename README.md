# Cryptocurrencies

The purpose of the challenge is to perform an analysis about offering a new cryptocurrency investment portfolio for customers. The goal is to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. After considerations it was decided to use a clustering algorithm, to group the cryptocurrencies.

## 1.	Preprocessing the Data for PCA

In this first step it was performed a cleaning and preparation process.

The dataframe looks like this:

![image](https://user-images.githubusercontent.com/95872614/168451720-3a5cefde-0851-4516-9968-896325ee66d6.png)

## 2.	Reducing Data Dimensions Using PCA

In order to reduce the dimension, it was necessary to apply PCA algorithm to reduce the dimensions to three principal components. The new dataframe looks like this:

![image](https://user-images.githubusercontent.com/95872614/168451727-c758dcd2-e959-484a-a5c5-d2c134c86203.png)

## 3.	Clustering Cryptocurrencies Using K-means

It was created an elbow chart to find the best value for K from the pcs_df dataframe, resulting:

![image](https://user-images.githubusercontent.com/95872614/168451738-45bc46a3-96c8-44a4-8d20-c3c706165405.png)

The K-means algorithm suggest using 4 clusters to predict the clusters for the data. A dataframe with all the data clustered_df was created.

![image](https://user-images.githubusercontent.com/95872614/168451745-719a6c0d-0a9b-48bf-8404-f46352767f9a.png)

## 4.	Visualizing Cryptocurrencies Results

Afterwards, it is possible to see the clusters that correspond to the 3 principal components with a 3D scatter chart.

![image](https://user-images.githubusercontent.com/95872614/168451759-e0308cf0-fbb8-49d7-ab4a-511a7c2f4594.png)

It was created a table with the hvplot.table functionality.

![image](https://user-images.githubusercontent.com/95872614/168451768-e943e223-2a34-4632-9c99-73e8e7a1f242.png)

Finally, it is possible to visualize the relationship between Total Coin Supply and Total Coins Mined by scaling those variables and plotting them on a scatter chart.

![image](https://user-images.githubusercontent.com/95872614/168451771-c4e3c93c-6033-473d-9087-e1a7698d0127.png)


