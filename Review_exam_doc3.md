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

