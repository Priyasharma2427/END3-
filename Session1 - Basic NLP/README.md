<b> What is a neural network neuron? </b>

Neural Network is the set of neurons organized in layers. 
Each and every neuron takes it’s input, multiplies it by it’s weights, then sums them up and passes the sum through the activation function to other neurons.



Neurons : x1 , x2, x3 ...... xn 

![image](https://user-images.githubusercontent.com/36500978/117363715-93c1fe80-aeda-11eb-8696-59dd6d2e991f.png)


<b> What is the use of learning rate? </b>

Learning rate is a hyperparameter that is used to control the weights of our network with respect the loss gradient.

Lower the value, training will progress very slowly as you are making very tiny updates to the weights in your network. If the value is too high, it can cause undesirable divergent behavior to your loss function. That is why we need to find the optimal learning rate.

![image](https://user-images.githubusercontent.com/36500978/117363533-552c4400-aeda-11eb-8945-dadaaf2d59fb.png)

<b> How are weights initialized? </b>

Weights are initialized with random numbers. Assigning random values to weights is better than just 0 assignment.

Thing to keep in mind if weights are initialized with high or very low values and what is a reasonable initialization of weight values.
a) If weights are initialized with very high values the term becomes significantly higher and if an activation function like sigmoid() is applied, the function maps its value near to 1 where the slope of gradient changes slowly and learning takes a lot of time.
b)If weights are initialized with low values it gets mapped to 0, where the case is the same as above. 
The aim of weight initialization is to prevent layer activation outputs from exploding or vanishing during the course of a forward pass through a deep neural network. If either occurs, loss gradients will either be too large or too small to flow backwards beneficially, and the network will take longer to converge, if it is even able to do so at all.

<b> What is “loss” in a neural network? </b>

Loss in neural network is the quantitave measure of deviation between the predicted output and the True output. It gives the measure of mistakes made by the network in predicting the output.

Basically, loss is nothing but a prediction error of neural net.

<b> What is the “chain rule” in gradient flow? </b>

Chain  is a formula to compute the derivative of a composite function.

The chain rule comes into play when we need the derivative of an expression composed of nested subexpressions. It helps to solve problems by breaking complicated expressions into subexpression whose derivatives are easy to compute.
