# Part 3

#### Class 11, 31st Oct
- A1 Under what condition does the relative frequency equal to the probability of an event?
- Sol: 
- A2 If 𝑓(𝑥) = 1 /𝑏−𝑎 is a valid density function in the region 𝑎 ≤ 𝑥 ≤ 𝑏, what is its first moment?
- Sol a+b/2, it is uniformly distributed.
- A3 Write one difference between a classification and a regression problem
- Sol: classification output is discreate and regression it would be continues.
- A4 What is meant by prescriptive analytics?
- Sol: it will not stop after describing it, it will describe the best solution.
- A5 What is the difference between Supervised learning and unsupervised learning?
- Sol: Supervised learning output is also part of training data and also validates with the answer given is write or wrong. In unsupervised learning it is not and no supervise to validate.
- A6 Can two independent events A and B be mutually exclusive?
- Sol: They are not independent
- A7 Define the term Statistic.
- Sol: it is an estimate parameter of a population 
- A8 If a sample is drawn from a normal population, what is the variance of the sample mean?
- Sol: Variance of a sample mean will σ2/n.
- A9 If a bivariate sample data appears to have a non-linear trend in the scatter plot, and the sample data contains both positive and negative values, what sort of transformation would you prefer for making it linear?
- Sol: square and log, move the origin and take everything to the positive. And log transformation.
- A10 Write any two methods for estimating the parameters in a regression problem
- Sol: v2 or mean square, Maximum likelihood estimation
- A11 Two models are proposed for a bivariate process based on a sample – (a) a straight line after a logarithmic transformation and (b) a cubic curve. Analysis of variance is done on both the models and it is found that the F values are 9.25 and 11.46 respectively for models a and b. The corresponding p values are 0.02 and 0.34 respectively. Which model would you choose?
- Sol: 0.02 model solution would be used.
- A12 Write one difference between Gradient Descent method and Stochastic Gradient Descent method of optimization.
- Sol: All the sample points in all the training data at every iteration. In SGD only one training data is chosen for every iteration.
- A13 What are the stopping criteria in training of an Artificial Neural Network?
- Sol: you exhausted the training data, changes in the weights, ie output from threshold value is minimal.
- A14 List two disadvantages of an Artificial Neural Network.
- Sol: Need of identifying the cause of the output. For all unveiled outputs it gives output.
- A15 What is the function and its derivative of RELU?
- Sol: The derivative is: f(x)={0if x<0 & 1 if x>0 & undefined in x=0.
- A simple Neural Network is shown below. The initial values of the weights are given below. w1 = 0.1; w2 = 0.4; w3 = -0.2; w4 = 0.2; w5 = 0.2 and w6 = -0.5. The target output T = 0.1 One of the input set from the training data is I1 = 0.4 and I2 = -0.7. For this input values, execute the back propagation for updating w1. Assume all the nodes in the hidden layer and the output layer has Sigmoid activation,and the Input nodes have identity activation and η is 0.1.
•	Sol: Chain rule. Gradient calculation, forward task, back propagation.


### Data sets
- [Link](https://archive.ics.uci.edu/ml/datasets/Student+Performance)  - As mentioned , the tasks include both classification and regression analysis. The dataset has 649 entries and 33 feature values [x0,x1,...,x32].
- [Link](https://archive.ics.uci.edu/ml/datasets/Wine+Quality)   - This dataset is also suitable for both classification and regression. There are 4898 entries and 12 feature values. However as it is mentioned, the dataset has imbalance, so data for good wines may be much lesser than data for normal wines, which could be a challenge.
- [link](https://archive.ics.uci.edu/ml/datasets/Forest+Fires)   -  The dataset has 517 entries and 13 features. Essentially it is a regression problem but we need to figure out if classification can also be done.
- [These are some datasets that are very popularly used to practice and learn machine learning. A comprehensive list is mentioned in below article:](https://machinelearningmastery.com/standard-machine-learning-datasets/)
- [Data set](https://groups.google.com/d/msgid/ccemachinelearning2020augdec/CAA_asQhGPXn4np%3D0j6doJ3W-tvjXGj%3DQnT4dAimkt8UjPXemWw%40mail.gmail.com.)

#### Some other sample data:
```
Kaggle:
https://www.kaggle.com/datasets

UCI:
https://archive.ics.uci.edu/ml/index.php

Quandl [Financial data]:
https://www.quandl.com/

US Government Open Dataset:
https://www.data.gov/

Indian Government OpenDataset:
https://data.gov.in/

World Bank Dataset:
https://data.worldbank.org/

Group Lens dataset [Recommendation systems eg:Movies] : 
https://grouplens.org/  

Awesome Public Dataset: 
https://github.com/awesomedata/awesome-public-datasets/

Sample datasets:
https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-datase [example csv file to see the features: https://docs.google.com/spreadsheets/d/e/2PACX-1vQU0SIALScXx8VXDX7yKNKWWPKE1YjFlWc6VTEVSN45CklWWf-uWmprQIyLtoPDA18tX9cFDr-aQ9S6/pubhtml ] . The dataset has some details of patients affected by coronavirus in China like age , gender, etc.
https://data.gov.in/resources-from-web-service/3630701  . Small and simple dataset on  Foreign Direct Investment (FDI) Equity Inflows in India.
```
#### Class 11, 7th Nov:

- [Class notes](https://14653191105202215679.googlegroups.com/attach/d203ce2701fb/7_nov_Notes_Trupthi.pdf?part=0.1&view=1&vt=ANaJVrFygro1V-H84HpbORO3BX5V4s_59wMDo-0dP3AEZ1ZxBqgF7KhcS7TN-O_m_86AgIYZ-ypgahcNgp9zV0SOOt-OA0flUR6fmewEFq1eP2hFM-W9_V4)
- **Decision tree - Self-Driving Cars:**
```
Grade Bumpiness Speed limit speed
Steap Bumpy Y Slow
Steap Bumpy Y Slow
flat Bumpy N fast
Steap Smooth N fast
```
- P(slow) = 0.5 P(fast) = 0.5
- Entropy = (0.5log (0.5)) +(0.5log (0.5)) =1
- Total no at Parent =4
- Total no at left child =3
- Total no at right child =1
- Weighted entropy of child =3/4*0.9 + 0= 0.675
- IG (grade)=1-0.675= 0.325
- IG(Bumpiness)=0
- IG (Speed limit) =1

#### Example Fraud Detection:
- Let’s consider there is a data of credit cards which has millions of transactions, by considering 1% of fraud has been detected in turn 1 lakh people have been affected. here there is a dependency on one side of the class which is minority (99% non-fraud transactions)
- Here accuracy depends on training data, how well is the algorithm is trained. Aim is to identify 1% of fraud detection hence it should be taken care when data is biased on one side where there can be a condition machine cannot learn properly. Becomes important to retain fraud conditions in training data.
- It would be difficult for any algorithm to find out if the data sets are biased on one side. In above case if it reaches 99% accuracy we still failed to identify 1% of fraud data.


## Measures:
- False Positive and False negative
- **Confusion Matrix:**

Prediction|xxx|Actual
-----|---|---
xxxx|Positive|negative
Positive| True Positive| False Positive
Negative| False Negative |True negative

- Recall-→ True positive/ ((True positive) + (False negative))
- Precision -→ True positive/ ((True positive) + (False positive))
- If recall increase precision decreases.
- Reading Assignment: Check on the applications on recall and precision or both examples
