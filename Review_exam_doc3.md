# Part 4

#### Class 13, 28th Nov
-[Class Notes](https://14653191105202215679.googlegroups.com/attach/b57faf493d2a/Notes%2028th%20November%202020.pdf?part=0.1&view=1&vt=ANaJVrFOr3g-JAR6cfJvMW_BzKOMbF-gnMDhIa-wBVXbTbjCs0j9N_ODU_qF99ntIF8AYKJJm5ysRYB2hLfB7OCAO6qoqn7ZyqXEifTUf3YSM-uhW_SZNNw)
#### KNN : K – Nearest Neighbors 
- Algorithm measures the nearest distance and classify the point in the class where the distance is minimum. 
- If K=1(One nearest neighbor),K=2(two nearest neighbor)….K=5)
- **Formula** Calculating nearest point = Minimum distance = √(x2-x1)2+(y2-y1)2
- **Manhatten distance** : The distance between two points measured along axis at right angles
- **Formula** Mdist = |y2-y1|+|x2-x1|
- If the classification is in terms of non-numeric values, we use Hamming distance 
- season -- Summer  - if season =summer then true distance 0/ --- Other or not Summer =if season = not summer, then false distance=1
- If the given data has both numeric and non-neumeric values then we use a combination of nearest point and hamming distance.
- **Formula** = Combination distance = √(x2-x1)2+(y2-y1)2 + (hamming distance)2
- Disadvantages of using K-NN – All points have to be remembered.
- ![KNN](https://miro.medium.com/max/405/0*a3bVVcWFwWBUtZnc.png)
- ![KNN Formula](https://www.analyticsvidhya.com/wp-content/uploads/2015/08/EuclideanDistanceGraphic.jpg)
- ![image of knn proff](https://cambridgecoding.files.wordpress.com/2016/01/knn2.jpg)


#### K means clustering -  Unsupervised learning
-	Consider two dimension with 3 clusters Cluster1, cluster2, Cluster3
-	**Formula** Centroid = (x1+x2+x3+x4+x5/5, y1+y2+y3+y4+y5/5)
-	(x1,y1) – Centroid of cluster1
-	(x2,y2) – Centroid of cluster2
-	(x3,y3) – Centroid of cluster3
-	**Algorithm**
    * 1 Identify the centroid
    * 2 Find the distance of each point in the data to the each of centroid
    * 3 Choose the class with minimum distance
    * 4 Now new points enter the cluster
    * 5 Repeat for all the points
    * 6 Calculate the new value of centroids
    * 7 Repeat step 2 to 5
-	(K- no of clusters) – (in k means clustering)
-	The point in one cluster should be absolutely dissimilar to point in another cluster.
-	The points within the cluster have the similar points. 
-	Choose K is an odd number
-	What happens when some examples are much larger than the other **example** grams vs Tones  or length 2mts with weight 2.2 Tones=2200kg
-	**Solution ** Normalization = x-xmin/xmax-xmin – we get values in between 0 and 1
-	Removing irrelevant parameters ---this can be also done by using domain experts.
-	Normalization is used to make the scale uniform of all numeric parameters. Bring it to a 0 or 1 range by **Normalization** = x-xmin/xmax-xmin –
-	If non numeric is possible values >2, split into multiple parameters with 2 outcomes.
-	Choose the K as odd number to not to have tie between different classes.  
![k Mean](https://miro.medium.com/max/1280/1*5UHmgCaTD8EegsPuKcxC1Q.png)
