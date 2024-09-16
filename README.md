# Math-For-Machine-learning
Math For Machine learning


## Gradient Descent (GD) is an optimization algorithm used to minimize a function by iteratively moving towards the steepest descent, i.e., the negative gradient of the function at the current point. It's widely used in machine learning to minimize cost functions, particularly in models like linear regression and neural networks.
Equation:
![image](https://github.com/user-attachments/assets/46166636-c0a2-43e1-8033-7f7cbcdd7b00)

## Function requirements
Gradient descent algorithm does not work for all functions. 
There are two specific requirements. A function has to be:


•	differentiable

•	convex

## Simplified Example:
Imagine you’re on a hill, and it’s very foggy so you can’t see far ahead. Your goal is to get to the bottom of the hill (the lowest point), but you don’t have a map or a clear view of where it is.
Here’s what you do:
1.	Look around your feet: You feel the ground around you to sense which direction is sloping downward.
2.	Take a small step in that direction: Once you know where the ground is lower, you take a step in that direction.
3.	Repeat: After each step, you again feel the ground around you and take another step downwards, always heading to the lowest spot you can sense.
Eventually, you reach the bottom of the hill because each step brings you closer to the lowest point. This is essentially how gradient descent works!
In machine learning, the "hill" is the error or cost we want to minimize, and "steps" are adjustments we make to the model’s parameters. By iteratively taking steps (adjusting parameters in small increments), we get closer to the best model that makes the least error. The "fog" is the uncertainty or complexity of the data, and gradient descent helps find the best solution without needing to see the entire landscape at once.


## Purpose:
In machine learning, this often involves finding the optimal parameters for a model to minimize the error between its predictions and the true values. By iteratively adjusting the parameters in the direction of steepest descent, gradient descent helps to find the best possible fit for the given data.


## Differentiate between Batch, Stochastic, and Mini-batch Gradient Descent: 
Describe each variant of GD and provide examples of scenarios where each might be most appropriate. 

1. Batch Gradient Descent (BGD)
•	Description: In BGD, the entire training dataset is used to calculate the gradient of the cost function before updating the model's parameters.
•	Example: Suitable for small to medium-sized datasets where computational resources are not a constraint.
2. Stochastic Gradient Descent (SGD)
•	Description: In SGD, a single random data point is used to calculate the gradient and update the model's parameters at each iteration.
•	Example: Suitable for large datasets or online learning scenarios where computational efficiency is a priority.
3. Mini-batch Gradient Descent (MBGD)
•	Description: In MBGD, a small subset (mini-batch) of the training data is used to calculate the gradient and update the model's parameters at each iteration.
•	Example: Suitable for medium to large datasets where computational resources are a concern, but faster convergence is desired.
Difference:

Variant	Gradient Calculation	Update Frequency	Advantages	Disadvantages
Batch Gradient Descent (BGD)	Entire dataset	Once per epoch	Accurate gradient, stable convergence	Slow, computationally expensive for large datasets
Stochastic Gradient Descent (SGD)	Single data point	After each data point	Fast, suitable for online learning	Noisy gradient, less stable
Mini-batch Gradient Descent (MBGD)	Mini-batch of data	After each mini-batch	Faster than BGD, more stable than SGD	May still be computationally expensive for very large datasets

In practice, MBGD is often the preferred choice due to its balance of speed, stability, and computational efficiency. However, the optimal variant may vary depending on the specific problem and available resources.
