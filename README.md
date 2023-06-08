# CryptoClustering
For Crypto Clustering project, I apply K-Means and Principal Component Analysis (PCA) to cluster crypto currencies. 

#### Elbow Curve Using Original Scaled Data
I created a list with the number of K-values range from 1-11. Then I create a KMean model using the loop counter for the n_clusters; fit the model and append the model using .inertia_ to the inertia list. Then I created a data frame to plot the Elbow curve. 
As the curve shown below, the best value for K is 4.
![alt text](https://github.com/TaiShan16/CryptoClustering/blob/main/Image/Elbow%20Curve.png)

#### Cluster Cryto currencies with K-Means Using the Original Scaled Data
![alt text](https://github.com/TaiShan16/CryptoClustering/blob/main/Image/CryptoCluster.png)

##### Elbow Curve Using PCA model
In this section, I create a PCA model and set 'n_components=3' and use PCA model with 'fit_transform' to reduce to 3 principal components. The best value for K when using PCA data is also 4, which does not different from the besk K value found using the Original Scaled Data.  
![alt text](https://github.com/TaiShan16/CryptoClustering/blob/main/Image/PCA%20Elbow%20Curve.png)

##### Cluster Cryptocurrencies with K-means Using the PCA Data
![alt text](https://github.com/TaiShan16/CryptoClustering/blob/main/Image/PCA%20Cluster.png)

After visually analyzing the cluster analysis result, we can say that by using a fewer features, we can get similar performance fo the model since we still identify 4 clusters.
