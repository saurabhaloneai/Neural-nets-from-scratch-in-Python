# Neural-nets-from-scratch-in-Python 🤖


This is an example implementation of a simple neural network using Python and the NumPy and SciPy libraries.

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Description

The neural network implemented in this code consists of an input layer, a hidden layer, and an output layer. The number of nodes in each layer can be specified when creating an instance of the `Nnetwork` class. The network is trained using a learning rate specified in the constructor.

## Installation

To use this code, you will need to have Python 3 installed, as well as the NumPy and SciPy libraries. You can install them using pip:

```sh
pip install numpy scipy
```

## Usage

To use the neural network, create an instance of the `Nnetwork` class with the desired number of input, output, and hidden nodes, as well as a learning rate. Then, call the `train` method with input and target vectors to train the network. Finally, call the `run` method with an input vector to get a result from the network.

Here is an example of how to create and use a simple neural network with 2 input nodes, 2 output nodes, 4 hidden nodes, and a learning rate of 0.6:

```python
from neural_network import Nnetwork

simple_network = Nnetwork(no_of_in_nodes=2, 
                          no_of_out_nodes=2, 
                          no_of_hidden_nodes=4,
                          learning_rate=0.6)

input_vector = [3, 4]
target_vector = [0.7, 0.3]

simple_network.train(input_vector, target_vector)

result = simple_network.run(input_vector)
print(result)
```

The `run` method will return an array of output values for the given input vector.

## Contributing

If you find a bug or have a feature request, please create an issue or submit a pull request.


