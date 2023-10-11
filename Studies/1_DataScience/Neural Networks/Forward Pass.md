Imagine having two neural connection, between 2 inputs and 1 output like this:

![[Untitled - Frame 1.jpg]]

It can be better represented as (The [Activation Function] represented is the [ReLU] function):

![[NN Studies - Frame 2.jpg]]

If X1 = 3, W1 = -4, X2 = 6, W2 = 2, Bias = 1, then the forward pass will look like this:

![[NN Studies - Frame 3.jpg]]

In a higher abstraction level if we isolate one neural connection between one input neuron and one output neuron we can have the example below:

![[NN Studies - Frame 5 (1).jpg]]

To calculate the value of **y** we can follow the recipe below (assuming we are using the [ReLU] - [Activation Function]: $$y = Max(0, Max(0, Max(0, x * w1 + b1) * w2 + b2) * w3 + b3)$$
Which is a composition of the following recipes:
- $x_1 = Max(0, x * w1 + b1)$
- $x_2 = Max(0, x_1 * w2 + b2)$
- $y = Max(0, x_2 * w3 + b3)$


