1. What is a decision boundary, and how does it relate to classification tasks?

**Answer:** A decision boundary is a line (in 2D), plane (in 3D), or hyperplane (in higher dimensions) that separates different classes in the feature space. For classification tasks, the model learns to position this boundary to split the input space into regions where each region corresponds to a predicted class. The quality of classification depends on how well this boundary separates the classes.

2. How does the bias term in a neuron affect the position of the decision boundary?

**Answer:** The bias term shifts the decision boundary parallel to itself, without changing its orientation. Mathematically, for a neuron with output y = w₁x₁ + w₂x₂ + b, changing the bias moves the boundary along the perpendicular direction to the weight vector. A larger bias shifts the boundary further from the origin.

3. Explain with an example how changing weights affects the orientation of the decision boundary.

**Answer:** The weights determine the orientation (slope) of the decision boundary. For example:
- If w = [1, 0] (weight only on feature 1), the boundary is vertical
- If w = [1, 1], the boundary is diagonal at 45°
- Changing weights rotates the boundary around the origin (or around a point shifted by the bias)

4. Why is it important to visualize the decision boundary when training a model?

**Answer:** Visualization helps identify:
- Whether the model is overfitting or underfitting
- How well classes are separated
- Whether the boundary makes intuitive sense for your data
- Convergence during training

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

**Solution:**

Given:
- Initial weights: w = [0.2, -0.1]
- Bias: b = 0.1
- Learning rate: η = 0.1
- Input: x = [1, 1]
- Target: t = 1
- Perceptron output: y = 0

Calculate the error term: (t - y) = 1 - 0 = 1

**New weights:**
w_new = [0.2, -0.1] + 0.1 × 1 × [1, 1]
w_new = [0.2, -0.1] + [0.1, 0.1]
w_new = [0.3, 0.0]

**New bias:**
b_new = 0.1 + 0.1 × 1 = 0.2

**Answer:**
- **New weights:** w = [0.3, 0.0]
- **New bias:** b = 0.2

