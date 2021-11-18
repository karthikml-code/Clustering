K-means Clustering Intuition:
![image](https://user-images.githubusercontent.com/85920192/142433197-bd3e3801-0303-47b5-b7f9-c74eb72f72d5.png)
Steps to be followed,
  1. Choose the number K of clusters
  2. Select at random K points, the centroids(no necessarily from your dataset)
  3. Assign each data point to the closest centroid -> That forms K clusters
  
  ![image](https://user-images.githubusercontent.com/85920192/142433671-35e80b3c-699d-4e9a-8ea0-72aa60ebf9da.png)
  
  After this move the cluster points to center of their respecting clusters and do the Euclidian distance. Then re-arrange the plots like how we did earlier. Repeat the process until the equidistance line doesn’t make any change. 
  In some cases, we would end up Random initialization trap which is putting the clusters on a different place than required. To avoid this we need to use K-means++ algorithm instead of K-means.

  
  4. Compute and place the new centroid of each cluster
  5. Reassign each data point to the new closest centroid. If any reassignment took place, go to step 4. Otherwise the model is done. 

Practical way of choosing the clusters. Below, we have selected clusters k as 2. Than we two random k points in the plot and assigning each data point to the closest cluster.

![image](https://user-images.githubusercontent.com/85920192/142434360-cad69cad-14e2-4491-b01a-e00ba4ead070.png)

The lesser the wcss score, the effective model would be. 





