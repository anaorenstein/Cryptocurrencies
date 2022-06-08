# Cryptocurrencies



## Overview

We were approached by Accountability Accounting, an investment firm, studying the prospects of new cryptocurrency investments. The dramatic rise and fall of BitCoin has made the endeavor seem initially  contrived. 

To evaluate the various types of currencies that exist, they requested us to perform an in-depth analysis of the cryptocurrencies that are on the trading market, creating a dataset that will classify and show profitability of each of these cryptocurrencies, and to display the data as tables and graphs that can reveal tendencies.



## Results

### Data Preprocessing Selection and Transformation

These were our steps:

- Preprocessing the data for PCA

  <img src="Images/preprocess.png"  width="60%" height="60%">

  

  - Using *get_dummies()* function to create variables for text features:

    <img src="Images/get_dummies.png"  width="80%" height="80%">


    

  - Standardizing data with *StandardScaler()*:

     <img src="Images/standard_scaler.png"  width="80%" height="80%">

    

- Reducing Data Dimensions Using PCA

  - Creating a DataFrame with three principal components:

    <img src="Images/data_dimensions.png"  width="80%" height="80%">

    

### Clustering Cryptocurrencies Using K-means

First we found the best value for K using the **Elbow Curve** as seen below:

![](Images/elbow_curve.png)



Subsequently, we initialized the **K-Means model** that predicted the clusters:

![](Images/predictions.png)



Finally, we created a new DataFrame that contains the predicted clusters, along with the cryptocurrency features, seen here partially:

![](/Users/anabisker/Desktop/Data_Analytics_Bootcamp/18-Unsupervised-Learning/Cryptocurrencies/Images/new_df.png)



### Visualizing and Interpreting Cryptocurrencies Results

We created visualizations of our results.

- **3D-Scatter with Clusters**

  ![](Images/3-d_plot.png)

  

- **Table with tradable cryptocurrencies**

  ![](Images/tradable-table.png)

  

We are able to predict that there are **532 tradable cryptocurrencies**.

We scaled data using *MinMaxScaler()* to create a **scatterplot with tradable cryptocurrencies**:

![](Images/tradable-scatterplot.png)

