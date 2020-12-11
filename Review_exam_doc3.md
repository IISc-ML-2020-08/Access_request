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
-	**Solution** Normalization = x-xmin/xmax-xmin – we get values in between 0 and 1
-	Removing irrelevant parameters ---this can be also done by using domain experts.
-	Normalization is used to make the scale uniform of all numeric parameters. Bring it to a 0 or 1 range by **Normalization** = x-xmin/xmax-xmin –
-	If non numeric is possible values >2, split into multiple parameters with 2 outcomes.
-	Choose the K as odd number to not to have tie between different classes.  
![k Mean](https://miro.medium.com/max/1280/1*5UHmgCaTD8EegsPuKcxC1Q.png)




####  Dec 5th
[Class Notes](https://14653191105202215679.googlegroups.com/attach/188a16448fcb1/ClassNotes_5th%20_December_2020.pdf?part=0.1&view=1&vt=ANaJVrFZzFNvkOeMcdwuenhRrDfkSlcgE_AD0ihb7KCqEpZzNx4_EdWWhgoTxiv6mBN8fMvS44TdzvKgaE5tLU39LGU6tGOjEWoC6TmPwIwAZejOailXz_U)

#### Principal component analysis (PCA)
-	Dimensionality reduction y = Bo+B1x --- Bivariate reduction
-	Estimating parameters Bo,B1 from the sample
-	T-Test |P – Test to indicate the confidence @ which values are obtained.
-	The individual errors in Bo,B1 gives the collective error in y
-	Considering a General case: `y = Bo+B1x+B2x2+…BnXn` n+1 parameters causes accumulated error
-	More parameters, More Error accumulated.
-	Since X1,X2,X3….Xn are causing variation in Y, accumulated error increases.
-	There is a tradeoff between incremental accuracy and the error are after a point this accuracy I low
-	So Seek to reduce the no of variables ie Dimensionality reduction.
-	One of the  methods is PCA.

#### Occams Razor: Simplest solution to be chosen 

#### Basics of linear Algebra:
-	No of elements in a vector 1D gives its dimension 
-	Matrices is of 2D
	
-	Consider the vector matrix [1/1] = 2 X 1 
-	2[1/1] = [2/2]
-	Consider a square matrix
-	[2/0 0/2] [1/1] = [2/2] in this case magnitude has increased 
-	[0/1 -1/0][1/1]=[-1/1]  In this plot magnitude is same but direction has changed by 90 degrees
-	Consider a combination of the above:
-	[0/1 -1/0][2/0 0/2][1/1]=[-2/2] :. Multiplication can results in change in magnitude, direction or both
-	From Above [0/2 -2/0][1/1]=[-2/2]
-	A-1=[0/-1/2 1/2/0]  A Inverse
-	On multiplication with above [0/-1/2 1/2/0]  [-2/2] = [1/1]
-	The original matrix is obtained on multiplication with the changed vector 

#### Eigen Values and Eigen Vectors:
-	IF A = Square matrix and V = Vector
-	On multiplying the two  If Av=λv then λ = Eigne Value and V = Eigne Vector of A
-	If A is symmetric ie A=A-1 then eigne vectors are arthogonal 


-	Consider the point (x1,y1) which will make sense only if origin and direction of Axes is defined . 
-	This is called Basis 
-	Suppose the definition has changed to 
-	Basis being origin O1 then the coordinates will change to (x1i,x2i)
-	Also if axes change direction to P & Q orthogonal to each other, point changes to (p,q).
-	Therefore as basis changes origin or axes the coordinates of particular point changes,
-	**Note** Origin changed by adding magnitude and axes changed by multiplication of vectors.
-	Covariance : Cov(x,y) =  Σ(x-x’)(y-y’)/n-1
-	If covariance recorded of X values with respect to y then Covariance matrix obtained. 
![Covariance Matrix]( https://www.statlect.com/images/cross-covariance-matrix__15.png)
-	Covariance Matrix : Square Matrix, Diagonal values are variance
-	Symmetric Matrix
-	Then the eighen vectors are orthogonal 
-	There are N Eigen values and n Eigen vectors.

#### PCA 
-	Arrange eigen values in descending order
-	Eigne values represents information contained in that combination
-	Remove the last few which has least values ex considering eigen values.
-	E1=100, e2=98,….en-3=0.04,en-2=0.02,en-1=0.017, en=0.004
-	Remove 4 values total values = n-4 with corresponding n-4 eigen vectors.
-	Change the basis to n-4 eigen vectors, the coordinate system of sample changes to n-4
-	In this new basis model is fit
-	On aligning data with the eigen values the eigen vectors corresponding to highest eigen values is called principal component.
-	With less parameters basis is along principal component and forecast using this model
-	Since physical data along original axes multiply by inverse to change the basis back 
-	Model performs better as accuracy is increased even throught soe information lost.
-	**Challenges**: Standardize the variables as PCA is sensitive to scale.
