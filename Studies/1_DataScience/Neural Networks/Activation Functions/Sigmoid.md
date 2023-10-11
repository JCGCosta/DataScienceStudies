A Sigmoid Activation Function in the context of neural networks is a function to introduce the property of non-linearity to the output of deep learning models.

Graphical representation of $$f(x) = \frac{1}{1+e^{-x}}$$
![[Pasted image 20230927145242.png]]

The issue with sigmoid activation function is that in large networks it occur an issue called vanishing gradient, which is when the weights remain unchanged as the derivate almost vanishes. What we usually do to solve that problem is use a [[ReLU]] as an [[Activation Function]].