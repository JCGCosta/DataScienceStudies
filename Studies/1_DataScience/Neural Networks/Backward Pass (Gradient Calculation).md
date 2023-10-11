The objective of the backward pass is to calculate better weights to fit the ground truth observations. The solution is calculate the gradient between the derivative of a loss function (calculated by the difference between the ground truth and the prediction), and the neural networks weights.

When calculating the gradient there are some rules to easily calculate the gradient value, but is important to know that the value is calculate by the chain rule from calculus.

The rules are:
- Add Gate (+): Gradient from output go to the input.
- Multiply Gate (\*): Multiply the gradient from the output to the switched forward pass value.
- Max Gate (Max): Gradient from output go to the input with the highest forward pass value, the other is 0.

Imagine having two neural connection, between 2 inputs and 1 output like this:

![[Untitled - Frame 1.jpg]]

It can be better represented as (The [[Activation Function]] represented is the [ReLU] function):

![[NN Studies - Frame 2.jpg]]

Then the backward pass (gradient values in red, the forward pass in green) is:

![[NN Studies - Frame 4.jpg]]

In a more generic way when a network generates an output, the [[Lost Function]] (L) shows how well the model predict a class by knowing how different the prediction is from the Ground Truth. The learning come from adjusting the weights in a way to make the [[Lost Function]] decrease. In the backward pass so, the new weight can be adjust using the old weight and the product between the learning rate and the gradient of the loss function in respect of that weight.

$$w_{new} = w_{old} - learningRate * \frac{d_L}{d_w}$$
By looking at the recipe above we can see that we have a value called learning rate which is an arbitrary value, that means that training a neural network is like a optimization problem, where we want to minimize the loss. The problem is that with higher learning rates we will have big jumps in the function, which means that we could never get to a great value. Otherwise, really small learning rates could make us being stuck in a local optimum or really small progress. 


![[3eee0b_33163162ddd94900b7d9f5b049e9b7e3~mv2.gif]]
