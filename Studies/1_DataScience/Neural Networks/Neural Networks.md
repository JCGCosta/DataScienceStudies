Objectives: Classify, Predict, Choose between options.

Layers: 
- Input (Features): The observation that we pretend to classify.
- Hidden: Where the learning happens by weight fitting.
- Output (Predictions): The classification possibilities.

To train a neural network is needed:
- A [[Forward Pass]].
- A [[Backward Pass (Gradient Calculation)]]: This method make the weights go in the directions of the ground truth.

The are different kinds of Neural Networks and Architectures, to solve different problems:
- NN Types: [[Perceptron]], [[MLP]].
- NN Architectures: [[RecurrentNN]], [[ConvolutionalNN]], [[LongShortTermMemory]], [[GRU]], [[Transformer]].

In between the artificial neurons the synapses need an [[Activation Function]], represented by this kind of function: **ActivationFunction(sum(WeightN * XN) + Bias)**.

Representation example:
![[Pasted image 20230925150937.png]]