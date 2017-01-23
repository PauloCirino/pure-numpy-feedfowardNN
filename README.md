# pure-numpy-feedfowardNN
Simple feedforward neural network class written in pure python+numpy

## Characteristics
* Can be used to create a fully connected feed forward with as many hidden layers as needed, of any size.
* Implements backpropagation : [link 1](http://neuralnetworksanddeeplearning.com/chap2.html), [link 2](https://www.youtube.com/watch?v=TrxeIv7RD_0&t=109s), [link 3](https://www.youtube.com/watch?v=CaRzkVaC_rs) 
  (does not implement gradient checking)
* Uses gradient descent for optimization
* Uses Sum Squared Error cost function

## How to use
1. Create an instance  
  `nn = NeuralNetwork()`
2. Add layers  
  The first input layer is created automatically  
  `nn.add_layer(shape=(input_dim1, output_dim1))`  
  `nn.add_layer(shape=(input_dim2, output_dim2))`
3. Train  
  `nn.train(features, targets, num_epochs, learning_rate)`
4. Predict  
  `nn.predict(features)`
