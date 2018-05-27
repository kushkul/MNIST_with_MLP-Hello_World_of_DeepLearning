# MNIST_with_MLP-Hello_World_of_DeepLearning
Recognizing Hand written digits using Multi layer Perceptrons.

## Getting Started

### MNIST Dataset
The MNIST database of handwritten digits, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from MNIST. The digits have been size-normalized and centered in a fixed-size image. The original black and white (bilevel) images from NIST were size normalized to fit in a 20x20 pixel box while preserving their aspect ratio. The resulting images contain grey levels as a result of the anti-aliasing technique used by the normalization algorithm. the images were centered in a 28x28 image by computing the center of mass of the pixels, and translating the image so as to position this point at the center of the 28x28 field. 

Example of an image from the dataset used:



![alt text](https://github.com/kushkul/MNIST_with_MLP-Hello_World_of_DeepLearning/blob/master/images/MNIST_sample.png)

Dataset used in this study can be downloaded from: http://yann.lecun.com/exdb/mnist/

### Multi-layer Perceptron Model
In a multi-layer Perceptron Model First we receive the input data array and then to send it to the first hidden layer. Then the data begin to have a weight attached to it between layers, which initially, is a random value, and then sent to a node to undergo an activation function. Then it continues on to the next hidden layer until the final output layer. We just use two hidden layer in this model.

Once the transformed data has reached the output layer we need to evaluate it. Here we use a loss function to evaluate how far off we are from the desired resuslt. In this case, how many classes we got correct.

Then we apply an optimization function to minimize the cost calculated in the last step. This is done by adjusting the weights across the network. In this example we are using Adam Optimizer.

We can adjust how quickly to apply to apply this optimization to the weights by changing the learning rate that we defined before. Lower the rate, higher is the possibility of accuracy and hence resolution , but slower is the process of optimization and longer it takes to get to the desired level of accuracy. The higher the rate, quicker is the optimization at the cost of resolution and we may end up diverging from the results.

The two hidden layers are using Relu activation function, which is a simple rectifier function which either returns 0 or x. Final output layer use linear activation function.
This is how a Perceptron looks like:
![alt text](https://github.com/kushkul/MNIST_with_MLP-Hello_World_of_DeepLearning/blob/master/images/perceptron.png)


## Prerequisites
Following are the packages needed to be installed for this study:
1) TensorFlow
2) matplotlib


## License
This project is licensed under the MIT License - see the LICENSE.md file for details.



