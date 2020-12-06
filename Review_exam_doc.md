## ML Class Sep 5th:  [Class 4 reff doc](https://14653191105202215679.googlegroups.com/attach/ef565b999631/20200905_Class%204%20Notes_KaranPardeshi.pdf?part=0.1&view=1&vt=ANaJVrFgHaij7IGVoFsQp49fl15KGglwN4cF89zLwS3QbGbpkUAB9oCoL8mcgX_ji39Ay5glcDYhhtXz0EvipNhgeIXjEeRSPPVgrd-NvIZjR3JkhAheTAw)
- Sampling Distributions
-	Deterministic – which can be calculated and given a accurate value. Stone falling from 100m
-	Sarcastic variable - Forecast of weather – close to real value
-	Discreet variable – average time taken to server a customer by a tea vendor
#### Topics :
- Statistical inference
- Population parameters and statistics
- Sampling distributions
- Sampling distribution of mean
- Sampling distribution of variance
- Central limit Theorem
- Confidence intervals
- Confidence intervals for means
    •	Large sample (n>=30)
    •	Small samples (n<30)
- Confidence interval of variances 

-  **What is machine learning**: - A machine performing task T is said to be learning if the performance as measured by P increases with Experience E – Tom Mitchells definition.
- Measurement of likelihood estimation 
   • Maximum likelihood estimate function (y - 𝑦̂ , where y is original and y-cap predicted value from model. We try to minimize the error)
   • Minimum square estimate function (y = mx + c. y and x are independent and identically distributed.)
   • Gaussian density function -- 𝐹(𝑥) = ∑ 1/ √2𝜋𝜎. 𝑒 (−𝑥−𝜇) 2 /𝜎 2
   • Basic example where we can use MLE  During a nut bolt manufacturing in a company diameter of bolt is 5 mm, which is instructed to be made. But as lathe machine has some error i.e. due to some limitations, what we get is bolts with 4.5mm or 4.78 mm. So here we are trying to use MLE to bring that value close to 5 mm.
- Types of Techniques in Machine Learning. 
    *  A – Regression. B – Classification. (Major difference OUTPUT of regression is continuous and OUTPUT of classification is discrete.)
- Examples of Classification 1. Recognizing digits’ problem. 2. Classifying cars. 3. Face recognition
- Examples of Regression 1. Forecast flow in river, if it has rained some amount in the nearby catchment area. 2. Cost vs Demand. 3. Demand vs Supply
- **Classification:** 
  * Linearly separable classes: A straight line acts as a separator and helps us in classifying 2 separate classes, i.e. 2 separate entities Oranges and Bananas on their respective attributes (size, color, weight etc). Find the closest points and find their mid-point and we take perpendicular bisector to separate them.
  * Linearly Non separable classes: which single line we can’t separate the classes, then use multiple lines like square, ellipse etc, Draw a rectangle which is tightest to all the point with outer and inner rectangle.
  * What if we have totally mixed up data.  In that case we cannot classify, we need to change the parameters --> We can also take help of domain expert. TRIAL and ERROR.
- **Machine learning problem solving** - Flow – Data – Data Cleaning – Keep some data for Training and some for testing and Evaluate the output. The data can be in 80:20 or 70: 30 ratios (Train and Test).
- **Supervised** – Well we have a supervisor to check that weather the output is right or wrong. We already know the output; hence we check if machine has delivered right output or not.
- **Unsupervised** – Hypothesis and optimization done by model itself. There is no supervisor to check the output. The machine itself does the entire job.
- [Other reff definations for supervised vs unsupervised](https://github.com/vurachaitanya/ML_AI/blob/master/Define.md)

