# ML Class
## Sep 5th, Class 4 [Reff Doc](https://14653191105202215679.googlegroups.com/attach/ef565b999631/20200905_Class%204%20Notes_KaranPardeshi.pdf?part=0.1&view=1&vt=ANaJVrFgHaij7IGVoFsQp49fl15KGglwN4cF89zLwS3QbGbpkUAB9oCoL8mcgX_ji39Ay5glcDYhhtXz0EvipNhgeIXjEeRSPPVgrd-NvIZjR3JkhAheTAw)
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
    * Large sample (n>=30)
    * Small samples (n<30)
- Confidence interval of variances 

-  **What is machine learning**: - A machine performing task T is said to be learning if the performance as measured by P increases with Experience E – Tom Mitchells definition.
- Measurement of likelihood estimation
    * Maximum likelihood estimate function (y - 𝑦̂ , where y is original and y-cap predicted value from model. We try to minimize the error)
    * Minimum square estimate function (y = mx + c. y and x are independent and identically distributed.)
    * Gaussian density function -- 𝐹(𝑥) = ∑ 1/ √2𝜋𝜎. 𝑒 (−𝑥−𝜇) 2 /𝜎 2
    * Basic example where we can use MLE  During a nut bolt manufacturing in a company diameter of bolt is 5 mm, which is instructed to be made. But as lathe machine has some error i.e. due to some limitations, what we get is bolts with 4.5mm or 4.78 mm. So here we are trying to use MLE to bring that value close to 5 mm.
- Types of Techniques in Machine Learning. 
    * A – Regression. B – Classification. (Major difference OUTPUT of regression is continuous and OUTPUT of classification is discrete.)
- Examples of Classification 1. Recognizing digits’ problem. 2. Classifying cars. 3. Face recognition
- Examples of Regression 1. Forecast flow in river, if it has rained some amount in the nearby catchment area. 2. Cost vs Demand. 3. Demand vs Supply
- **Classification:** 
  * Linearly separable classes: A straight line acts as a separator and helps us in classifying 2 separate classes, i.e. 2 separate entities Oranges and Bananas on their respective attributes (size, color, weight etc). Find the closest points and find their mid-point and we take perpendicular bisector to separate them.
  * Linearly Non separable classes: which single line we can’t separate the classes, then use multiple lines like square, ellipse etc, Draw a rectangle which is tightest to all the point with outer and inner rectangle.
  * What if we have totally mixed up data.  In that case we cannot classify, we need to change the parameters --> We can also take help of domain expert. TRIAL and ERROR.
- **Machine learning problem solving** - Flow – Data – Data Cleaning – Keep some data for Training and some for testing and Evaluate the output. The data can be in 80:20 or 70: 30 ratios (Train and Test).
- **Supervised** – Well we have a supervisor to check that weather the output is right or wrong. We already know the output; hence we check if machine has delivered right output or not.
- **Unsupervised** – Hypothesis and optimization done by model itself. There is no supervisor to check the output. The machine itself does the entire job.
- [Other reff definations for supervised vs unsupervised](https://github.com/vurachaitanya/ML_AI/blob/master/Define.md)


## Sep 12, Class 5 [Reff Doc](https://14653191105202215679.googlegroups.com/attach/1b6df9c5a144c/20200912_Neural%20Network%20Intro_GKS.pdf?part=0.1&view=1&vt=ANaJVrG8DWw4qPvZICK_3IE1NlJsUE57GUp3kg5v9QBLUlqRwAL00xk_yP_rFS4aNffghQOVDwrtYBlZaFf0_SZgTMNXlNE0LzqbTl0lhVE9FW6CoWtC-wk) 

- ** Rectangle vs ellipse **
- Improves accuracy
- Shape fits more data points
- Corners points handles better
- Ellips can better represents compared to rectangle area
- **Disadvantages** - extremely complex in higher dimensions, - Boundary is complex
- **Artificial neural networks - ANN**
- **Deep networks**
- **Activation functions** -> Takes to be input and output should be 0 to 1, ->	H11= I1w1+I2w2+I3w3 +b1 (H11 – hidden layer, I-Input, w-weight, b- bias) 
- [Baseic of Activation function and why weights and biases are added  with detailed explanation](https://www.kdnuggets.com/2020/11/building-complete-artificial-neural-network.html)
- **Practical Computer Vision Applications Using Deep Learning with CNNs: With Detailed Examples in Python Using TensorFlow and Kivy** Good book to read


## Exam on Sep 19
-	If X ~ N(0,1), what is P(X=0.3)? -> probability of x=0.3 is 0. As x ranges from 0 or 1.
-	A card is drawn at random from a pack of cards. What is the probability that it is neither a spade nor a Jack? ->52 -16/52 =36/52
-	For a bivariate sample of size 56, a Minimum Least Squared line if fit, and the parameters b0 and b1 are estimated as 3.6 and 1.7. What will be the values of b0 and b1 if we use the Maximum Likelihood method? Assume the underlying process is Gaussian.  -> y=mx+c
-	State Mitchell’s definition of Machine Learning -> A machine performing task T is said to be learning if the performance as measured by P increases with Experience E – Tom Mitchells definition.
-	Define Regression of Y on X -> 
-	List one advantage and one disadvantage of using an ellipse for a classification model where two parameters x1 and x2 decide the classes. ->**ADV** Improves accuracy, Shape fits more data points, Corners points handles better,Ellips can better represents compared to rectangle area **Disadvantages** extremely complex in higher dimensions, - Boundary is complex.
-	Prove that 𝑥̅= ∑ 𝑥/𝑛 is an unbiased estimate of the population mean m ->
-	With respect to a bivariate continuous distribution, define marginal distribution -> y=integral from infinite to -infinite f(x,y)dx
-	What is the assumption made in estimating parameters using a Likelihood function? ->IID (identical)
-	Where does the learning information get stored in an Artificial Neural Network? ->weights
- A box contains three coins, two regular coins and one fake coin with both sides being heads.
  * You pick up a coin at random and toss it . What is the probability that it lands heads up?
  * You pick a coin and toss it and get heads. What is the probability that it is the 2 headed coin?
-	The following are the values of two input variables which classify an output variable, With this training data, set up a Generic, Specific and Candidate Hypothesis, and find the optimal hypothesis. If an additional set of inputs (10,4) is then obtained, find the classification of the new point as per the earlier training.

```
X Y Class X Y Class
2 10 - 15 13 +
5 17 - 16 14 +
7 3 - 17 15 +
8 20 - 17 23 -
12 14 + 18 14 +
14 14.5 + 20 15 -
15 5 - 22 12 -
```

## Class 6, Sep 26th :
-	As we are considering 2 **Activation functions** , **BINARY** step function and **BIPOLAR** step function. 
-	For Binary. Now input function f (in) = 1 if ( in > 0) , 0 if (in <= 0)->**BINARY **
-	For Bipolar f (in) = 1 if (in > 0), -1 if (in <= 0) ->**BIPOLA**

## Hebb’s Rule: 
[Ref Doc:](https://14653191105202215679.googlegroups.com/attach/6caeb96d9ca5e/Deep%20learning%20Class%206%20Notes_karan_p.docx.pdf?part=0.1&view=1&vt=ANaJVrEEXB0Qg9qJfmOT0mEJz8ODkY494dsWg3DRC93tfiBr13gCww9FeilaqICCVD9EROe8ps5NZUqm5fg4vyJYp2b1bTMHEUAyYX0O1TetZ5A5kBSK1vg)

**Hebbian Learning Algorithm Hebbs Rules** 
- Initialize all weights and bias 
- Modify the weights according to the following rule. 
    * Wi(new) = Wi(old) + ∆Wi 
    * ∆Wi = Xi * Y --- Where Xi is input and Y is target output. 
    * Bias b(new) = b(old) + ∆b
    * ∆b = y
    
![Hebbians Formula](https://www.google.com/imgres?imgurl=https%3A%2F%2Fcdn.softwaretestinghelp.com%2Fwp-content%2Fqa%2Fuploads%2F2019%2F08%2FHebbian-Learning-Rule-Step-2.png&imgrefurl=https%3A%2F%2Fwww.softwaretestinghelp.com%2Fneural-network-learning-rules%2F&tbnid=EQlq9RMjV7c-aM&vet=12ahUKEwjgvO7v_L7tAhVDcK0KHf8ADhoQMygaegUIARDeAQ..i&docid=ztRVMApFIc6xbM&w=483&h=122&q=Hebbs%20rule%20with%20truth%20table%20example&ved=2ahUKEwjgvO7v_L7tAhVDcK0KHf8ADhoQMygaegUIARDeAQ)

- Modify the weights according to the following Wi(new)=Wi(old)+Delta Wi
   * According to Hebbs rule – w1 = w2 = b = 0
   * ∆W1 = X1*Y
   * ∆W2 = X2 * Y
   * ∆b = b*Y
   * W1 = old(W1) + new∆W1

- **AND – Gate example**
```
X1 X2 1(Xb) Y ∆W1 ∆W2 ∆b W1 W2 b
1 1 1 1 1 1 1 1 1 1
1 0 1 0 0 0 0 1 1 1
0 1 1 0 0 0 0 1 1 1
0 0 1 0 0 0 0 1 1 1

```
- **Example 2 – Bipolar inputs**  You can say Bivariate inputs in which all zeros are turned to -1 in inputs.
  * According to Hebbs rule – w1 = w2 = b = 0

```
X1 X2 1(Xb) Y ∆W1 ∆W2 ∆b W1 W2 b
1 1 1 1 1 1 1 1 1 1
1 -1 1 -1 -1 1 -1 0 2 0
-1 1 1 -1 1 -1 -1 1 1 -1
-1 -1 1 -1 1 1 -1 2 2 -
```
Y = w(b) + Σx * w = 0

- We see the two partitions i.e. the black dotted line separating + and –
- So What is Hebbs rule telling us ------?
  * Ans: The Hebbian rule is based on the rule that weight vector increases proportionally to the input and learning signal i.e. the output. The weights are incremented by adding the product of the input and output to the old weights.
  * W (new) = w (old) +x*y

## External data more on NN:
- [Example with details on classification in NN](https://towardsdatascience.com/deep-learning-weekly-piece-whats-a-neural-network-aa0df888d8a2)
- [Reff Doc:](https://towardsdatascience.com/multi-layer-neural-networks-with-sigmoid-function-deep-learning-for-rookies-2-bf464f09eb7f)
- Advantages of nonlinear activation function: Without a nonlinear activation function, the neural network is calculating linear combinations of values, or in the case of a deep network, linear combinations of linear functions (i.e., lines). Note that a linear combination of lines is again a line. 
- [Playground for Neural networks tensorflow](http://playground.tensorflow.org/)
- Backpropagation, a procedure to repeatedly adjust the weights so as to minimize the difference between actual output and desired output
- **Brief on backpropagation**, we iterated the importance of designing a neural network so that the network can learn from the difference between the desired output (what the fact is) and actual output (what the network returns) and then send a signal back to the weights and ask the weights to adjust themselves? This will make the network’s output closer to the desired output next time we run it.
- Hidden Layers, which are neuron nodes stacked in between inputs and outputs, allowing neural networks to learn more complicated features (such as XOR logic)
- A hidden layer transforms a single-layer perceptron into a multi-layer perceptron. Hidden layers of a neural network is literally just adding more neurons in between the input and output layers.
- we have m input data (x1, x2, …, xm), we call this m features. A feature is just one variable we consider as having an influence to a specific outcome and we multiply each of the m features with a weight (w1, w2, …, wm) and sum them all together, this is a dot product
- The procedure of how input values are forward propagated into the hidden layer, and then from hidden layer to the output

#### Sigmoid Neurons: An Introduction of why (Step vs Sigmoid) :
- [Class Notes](https://14653191105202215679.googlegroups.com/attach/a31bc8f5c9940/Class7Notes_ANN_priyanka.pdf?part=0.1&view=1&vt=ANaJVrHbx1R-wVnEImTOm3__QP_CNhyoT7csIhY35cgn8bpzSWwjxQSBi78p8RCYcutpBr3fLnatK4JgxOIzlOgZww1uavEVprKqrTkesH9VD9lNJeCLDTE)
- So now we have a more sophisticatedly structured neural network with hidden layers. But we haven’t solved the activation problem with the step function.
- If the activation function is linear, then you can stack as many hidden layers in the neural network as you wish, and the final output is still a linear combination of the original input data
- This linearity means that it cannot really grasp the complexity of non-linear problems like XOR logic or patterns separated by curves or circles.
- **Example** : Think about it: this girl (or boy) has got some serious bipolar issues! One day (for z < 0), (s)he’s all “quiet” and “down”, giving you zero response. Then another day (for z ≥ 0), (s)he’s suddenly “talkative” and “lively”, speaking to you nonstop. Heck of a drastic change! There’s no transition for her/his mood, and you don’t know when it’s going down or up. Yeah…that’s step function
- So basically, a small change in any weight in the input layer of our perceptron network could possibly lead to one neuron to suddenly flip from 0 to 1, which could again affect the hidden layer’s behavior, and then affect the final outcome. Like we said already, we want a learning algorithm that could improve our neural network by gradually changing the weights, not by flat-no-response or sudden jump.

#### Sigmoid function: 
![Sigmoid function](https://miro.medium.com/max/1050/1*TdlBJnoH3GcKwAIFv1ASxg.jpeg)
- its curve and its derivative
- Sigmoid function produces similar results to step function in that the output is between 0 and 1. The curve crosses 0.5 at z=0, which we can set up rules for the activation function, such as: If the sigmoid neuron’s output is larger than or equal to 0.5, it outputs 1; if the output is smaller than 0.5, it outputs 0.
- Sigmoid function does not have a jerk on its curve. It is smooth and it has a very nice and simple derivative of σ(z) * (1-σ(z)), which is differentiable everywhere on the curve.
- Non-linear just means that the output we get from the neuron, which is the dot product of some inputs x (x1, x2, …, xm) and weights w (w1, w2, …,wm) plus bias and then put into a sigmoid function.
- Now, the computer can’t really “see” a digit like we humans do, but if we dissect the image into an array of 784 numbers like [0, 0, 180, 16, 230, …, 4, 77, 0, 0, 0], then we can feed this array into our neural network. The computer can’t understand an image by “seeing” it, but it can understand and analyze the pixel numbers that represent an image.
- neural networks become better by repetitively training themselves on data so that they can adjust the weights in each layer of the network to get the final results/actual output closer to the desired output? So when we actually train this neural network with all the training examples 

#### Why backpropagation
- [Back propagation with example](https://mattmazur.com/2015/03/17/a-step-by-step-backpropagation-example/)
- [Ref Doc:](https://www.quora.com/What-is-the-best-visual-explanation-for-the-back-propagation-algorithm-for-neural-networks/answer/Sebastian-Raschka-1)
- In backpropagation, you simply backpropagate the error (the "cost" that you compute by comparing the calculated output and the known, correct target output)
- Why reverse and not forward? Because it is computationally cheaper! If we'd do it forward-wise, we'd successively multiply large matrices for each layer until we multiply a large matrix by a vector in the output layer
- However, if we start backwards, that is, we start multiplying a matrix by a vector, we get another vector and so forth. So, I'd say the beauty in backpropagation is that we are doing more efficient matrix-vector multiplications instead of matrix-matrix multiplications

#### Loss function:
- [Ref Doc](https://algorithmia.com/blog/introduction-to-loss-functions)
- At its core, a loss function is incredibly simple: it’s a method of evaluating how well your algorithm models your dataset. If your predictions are totally off, your loss function will output a higher number. If they’re pretty good, it’ll output a lower number. As you change pieces of your algorithm to try and improve your model, your loss function will tell you if you’re getting anywhere.
- In fact, we can design our own (very) basic loss function to further explain how it works. For each prediction that we make, our loss function will simply measure the absolute difference between our prediction and the actual value. In mathematical notation, it might look something like abs(y_predicted – y). Here’s what some situations might look like if we were trying to predict
- Notice how in the loss function we defined, it doesn’t matter if our predictions were too high or too low. All that matters is how incorrect we were, directionally agnostic. This is not a feature of all loss functions: in fact, your loss function will vary significantly based on the domain and unique context of the problem that you’re applying machine learning to. In your project, it may be much worse to guess too high than to guess too low, and the loss function you select must reflect that.
- A lot of the loss functions that you see implemented in machine learning can get complex and confusing, loss functions–measuring how well your algorithm is doing on your dataset–you can keep that complexity in check.
- **Mean Squared Error (MSE)** is the workhorse of basic loss functions: it’s easy to understand and implement and generally works pretty well. To calculate MSE, you take the difference between your predictions and the ground truth, square it, and average it out across the whole dataset.

## Ref Doc:
- [MIT Doc on Deeplearning](https://www.deeplearningbook.org/)
- [ANN ref Doc](https://data-flair.training/blogs/learning-rules-in-neural-network/)
