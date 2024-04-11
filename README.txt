This model implements the perceptron algorithm to predict wether the email received is spam or not.

DOn't hesitate to visit the link for further information:
https://en.wikipedia.org/wiki/Perceptron

The perceptron algorithm is one of the earliest forms of supervised learning algorithms for binary classification tasks. It was proposed by Frank Rosenblatt in 1957 and is the simplest form of a single-layer neural network. Here's a detailed explanation of how the perceptron algorithm works:

Perceptron Model: The perceptron is a binary classifier that maps input vectors to output values through a process of weighted summation followed by a thresholding operation. It takes a vector of input features 
�
=
[
�
1
,
�
2
,
.
.
.
,
�
�
]
X=[x 
1
​
 ,x 
2
​
 ,...,x 
n
​
 ] and produces a binary output 
�
^
y
^
​
  indicating the predicted class label.

Initialization: Initially, the weights 
�
1
,
�
2
,
.
.
.
,
�
�
w 
1
​
 ,w 
2
​
 ,...,w 
n
​
  are set to small random values or initialized to zeros. A bias term 
�
b is also initialized.

Weighted Sum: For each input feature 
�
�
x 
i
​
 , the weighted sum of the inputs is calculated:
�
=
∑
�
=
1
�
�
�
×
�
�
+
�
z=∑ 
i=1
n
​
 w 
i
​
 ×x 
i
​
 +b
Here, 
�
�
w 
i
​
  represents the weight associated with input feature 
�
�
x 
i
​
 , and 
�
b is the bias term.

Activation Function: The weighted sum 
�
z is then passed through an activation function. In the case of the perceptron, the activation function is a step function (also called a threshold function), which is defined as:

1 & \text{if } z \geq 0 \\
0 & \text{if } z < 0
\end{cases} \]
The output \( \hat{y} \) is the predicted class label.
Training: The perceptron algorithm iterates through the training data, adjusting the weights based on the errors in prediction. The algorithm can be summarized as follows:

For each training example, calculate the predicted output 
�
^
y
^
​
 .
Compute the error 
�
=
�
−
�
^
δ=y− 
y
^
​
 , where 
�
y is the true class label.
Update the weights and bias according to the perceptron learning rule:
�
�
=
�
�
+
�
×
�
×
�
�
w 
i
​
 =w 
i
​
 +α×δ×x 
i
​
 
�
=
�
+
�
×
�
b=b+α×δ
Here, 
�
α is the learning rate, which controls the step size of the weight updates.
Convergence: The algorithm continues iterating through the training data until convergence, which occurs when all data points are classified correctly or a maximum number of iterations is reached.

Decision Boundary: The decision boundary of the perceptron is a hyperplane that separates the input space into two regions corresponding to the two class labels. It is determined by the weights and bias learned during training.

Limitations: The perceptron algorithm has several limitations, such as its inability to learn non-linear decision boundaries and its sensitivity to the initial choice of weights. These limitations were addressed by later developments in neural network architectures, such as multi-layer perceptrons and deep learning models.

Despite its limitations, the perceptron algorithm played a crucial role in the development of neural network theory and served as the foundation for more complex neural network architectures.