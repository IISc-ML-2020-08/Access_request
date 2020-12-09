# PART 2

### Class 7, OCT 3rd :
- [Class Notes](https://14653191105202215679.googlegroups.com/attach/a31bc8f5c9940/Class7Notes_ANN_priyanka.pdf?part=0.1&view=1&vt=ANaJVrHbx1R-wVnEImTOm3__QP_CNhyoT7csIhY35cgn8bpzSWwjxQSBi78p8RCYcutpBr3fLnatK4JgxOIzlOgZww1uavEVprKqrTkesH9VD9lNJeCLDTE)
- [Ref on Sigmoid vs  Tanh vs ReLU](https://machinelearningmastery.com/rectified-linear-activation-function-for-deep-learning-neural-networks/)
-	**Activation function** is the function in an artificial neuron that delivers an output based on inputs.
-	** Stochastic descent** : Adjusting the weights until we reach the final required target is call sarcastic descent 
-	From Wiki **Stochastic gradient descent** (often abbreviated SGD) is an iterative method for optimizing an objective function with suitable smoothness properties (e.g. differentiable or subdifferentiable). It can be regarded as a stochastic approximation of gradient descent optimization, since it replaces the actual gradient (calculated from the entire data set) by an estimate thereof (calculated from a randomly selected subset of the data). Especially in high-dimensional optimization problems this reduces the computational burden, achieving faster iterations in trade for a lower convergence rate
-	Layer by layer and optimize. But as we don’t have the target until where the optimization should be done. We choose to use Back/Forword propagation.
-	**Forward propagation** : you keep adjusting weight (Stochastic descent) and keep adjusting weights as we know the target, adjust the weights, until you reach the target. Cost for completion/ CPU computation is very hight.
-	**Back propagation** : The Backpropagation algorithm looks for the minimum value of the error function in weight space using a technique called the delta rule or gradient descent. The weights that minimize the error function is then considered to be a solution to the learning problem. 
- [BP Artical with examples](https://www.edureka.co/blog/backpropagation/)
- [Ref Doc](The Backpropagation algorithm looks for the minimum value of the error function in weight space using a technique called the delta rule or gradient descent. The weights that minimize the error function is then considered to be a solution to the learning problem. )

#### Relu (Rectified Linear Unit): 
- Non-linear activation function,  it does not activate all the neurons at the same time.
- Neurons will only be deactivated if the output of the linear transformation is less than 0.
- For the negative input values, the result is zero, that means the neuron does not get activated. Since only a certain number of neurons are activated, the ReLU function is far more computationally efficient when compared to the sigmoid and tanh function
- As you know, each connection in a neural network has an associated weight, which changes in the course of learning. According to it, an example of supervised learning, the network starts its learning by assigning a random value to each weight. Calculate the output value on the basis of a set of records for which we can know the expected output value. This is the learning sample that indicates the entire definition. As a result, it is called a learning sample. The network then compares the calculated output value with the expected value. Next calculates an error function ∈, which can be the sum of squares of the errors occurring for each individual in the learning sample.
- Perform the first summation on the individuals of the learning set, and perform the second summation on the output units. Eij and Oij are the expected and obtained values of the jth unit for the ith individual. The network then adjusts the weights of the different units, checking each time to see if the error function has increased or decreased. As in a conventional regression, this is a matter of solving a problem of least squares. Since assigning the weights of nodes according to users, it is an example of supervised learning.

#### Hebbian Learning Rule
- The Hebbian rule was the first learning rule. In 1949 Donald Hebb developed it as learning algorithm of the unsupervised neural network. We can use it to identify how to improve the weights of nodes of a network.
- The Hebb learning rule assumes that – If two neighbor neurons activated and deactivated at the same time. Then the weight connecting these neurons should increase. For neurons operating in the opposite phase, the weight between them should decrease. If there is no signal correlation, the weight should not change.
- When inputs of both the nodes are either positive or negative, then a strong positive weight exists between the nodes. If the input of a node is positive and negative for other, a strong negative weight exists between the nodes.
- At the start, values of all weights are set to zero. This learning rule can be used0 for both soft- and hard-activation functions. Since desired responses of neurons are not used in the learning procedure, this is the unsupervised learning rule. The absolute values of the weights are usually proportional to the learning time, which is undesired.

## Class 8 Oct 10
-	[Class Notes](https://14653191105202215679.googlegroups.com/attach/78edc9260b6be/Class8_notes_SGD_ShruthiM.pdf?part=0.1&view=1&vt=ANaJVrFHdeY9VPjDh4wu5JXU8RwM17WqGdObiNN61PS0tF6E5kqENtqmsHgxgW88hzaI61uoK94abydlkOMW78-z1W_cSTvPwH3ykFT9gkZYUuyGkKaWkN4)
#### Agenda
-	Back propagation 
-	Hibbs rule
-	Modified Delta rule
-	Gradient Descent
-	Stochastic gradient descent

-	Going calculus is expensive. Competitional expensive and inefficient 
-	Better to go with numerical optimization technics, which will come to near solution to our solution.  
-	Chain rule in calculus
-	**Gradient Descent formula**
-	dc/dw =2[(y1-x1)+ (y2-x2)+ (y3-x3)] 
-	Wn=wo – N(dc/dw) 
-	N = Learning rate , Wn= New weights, Wo= Old weights, x1,x2,x3 are first second third iterations of input values and y1 y2 y3 are outputs for respective x input iterations. 
-	By adjusting weights, we will reach the optimum values.
-	As we are moving down it is call gradient descent.
-	If we have 1000 variables, then we need to do 6K iterations of additions (6 addition). 3k weights x1k variables iterations should be done. Very complex for higher values. 
-	**Stochastic gradient descent** SGD
-	Randomly choose the points and implement Gradient descent formula.
-	Computationally efficient is very high in SGD
-	Cost function = (output – target)2- square
-	Wn=Wo-Ndc/dw (N= Learning rate, w0 old weight, Wn=New Weights)
-	Cost function= Σ(output – target)2 
-	Back propagation - output layer to input layer.


# Class 8th, Oct 17
- [Class notes](https://14653191105202215679.googlegroups.com/attach/34cac17cc049c/ClassNotes-%20Back%20Propagation-17Oct-by-Prasenjit.pdf?part=0.1&view=1&vt=ANaJVrFbL3nvkdZ-pNfuGJwObAstKWMfnWslJ1lf-56v_IkXqe8UEfXrHFvKGZO5GK324S5iK4dfivpAVwVSyncfuehLaFGMni9dSldZLjser987YySaLDc)

#### Drawback of Stochastic gradient descent
-	SGD Stochastic gradient descent – it has step until some value after it oscillate for long time to reach final goal. Which is so called as zone of confusion is the drawback.
-	Step size for a learning rate is large then coming to a min point may take out of scope because of more oscillations, as steps size is more. SGD is sensitive to learning rate. LR(learning rate) start with 0.1 rather than higher values 0.5,0.8 etc.
-	Pytorch we can set learning rate at high value and later can be changed.
