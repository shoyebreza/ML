1. What is a decision boundary, and how does it relate to classification tasks?

2. How does the bias term in a neuron affect the position of the decision boundary?

3. Explain with an example how changing weights affects the orientation of the decision boundary.

4. Why is it important to visualize the decision boundary when training a model?

**Math :** 

**1\. Weight Update (Perceptron Learning Rule)**

 A perceptron has:

* Initial weights: w \= \[0.2, \-0.1\]

* Bias: b \= 0.1

* Learning rate: η \= 0.1

For a training example with:

* x \= \[1, 1\]

* Target t \= 1

If the perceptron output is y \= 0, calculate the **new weights and bias** after one update using:

w\_new \= w \+ η \* (t \- y) \* x  
 b\_new \= b \+ η \* (t \- y)

