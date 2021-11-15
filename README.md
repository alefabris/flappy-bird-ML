# Machine Learning using NEAT to play Flappy Bird

## Index:
* ### [Flappy Bird] (#fb)<br>
* ### [Algorithm] (#algo)<br>
* ### [Instruction] (#inst)<br>

## Flappy Bird (Original Game) <a id=fb> </a>

Flappy Bird is a mobile game developed by Vietnamese video game artist and programmer Dong Nguyen (Vietnamese: Nguyễn Hà Đông), under his game development company [.Gears](http://dotgears.com). The game is a side-scroller where the player controls a bird, attempting to fly between columns of green pipes without hitting them. Nguyen created the game over the period of several days, using a bird protagonist that he had designed for a cancelled game in 2012.


## Algorithm: <a id=algo> </a>
* ### [Neural Network (NN)](#nn)<br>
* ### [Genetic Algorithm (GA)](#ga)<br>
* ### [NeuroEvolution of Augmenting Topologies (NEAT)](#neat)<br>

### Neural Network (NN) <a id=nn> </a>

An Neural Network (NN) is based on a collection of connected units or nodes called artificial neurons, which loosely model the neurons in a biological brain. Each connection, like the synapses in a biological brain, can transmit a signal to other neurons. An artificial neuron receives a signal then processes it and can signal neurons connected to it. The "signal" at a connection is a real number, and the output of each neuron is computed by some non-linear function of the sum of its inputs. The connections are called edges. Neurons and edges typically have a weight that adjusts as learning proceeds. The weight increases or decreases the strength of the signal at a connection. Neurons may have a threshold such that a signal is sent only if the aggregate signal crosses that threshold. Typically, neurons are aggregated into layers. Different layers may perform different transformations on their inputs. Signals travel from the first layer (the input layer), to the last layer (the output layer), possibly after traversing the layers multiple times.

### Genetic Algorithm (GA) <a id=ga> </a>

A genetic algorithm (GA) is a metaheuristic inspired by the process of natural selection that belongs to the larger class of evolutionary algorithms (EA). Genetic algorithms are commonly used to generate high-quality solutions to optimization and search problems by relying on biologically inspired operators such as mutation, crossover and selection.
n a genetic algorithm, a population of candidate solutions (called individuals, creatures, or phenotypes) to an optimization problem is evolved toward better solutions. Each candidate solution has a set of properties (its chromosomes or genotype) which can be mutated and altered; traditionally, solutions are represented in binary as strings of 0s and 1s, but other encodings are also possible.


### NeuroEvolution of Augmenting Topologies (NEAT) <a id=ga> </a>

In this project for the machine learning I use an algorithm called NEAT. 

NeuroEvolution of Augmenting Topologies (NEAT) is a genetic algorithm (GA) for the generation of evolving artificial neural networks (a neuroevolution technique) developed by Ken Stanley in 2002 while at The University of Texas at Austin. It alters both the weighting parameters and structures of networks, attempting to find a balance between the fitness of evolved solutions and their diversity. It is based on applying three key techniques: tracking genes with history markers to allow crossover among topologies, applying speciation (the evolution of species) to preserve innovations, and developing topologies incrementally from simple initial structures ("complexifying"). On simple control tasks, the NEAT algorithm often arrives at effective networks more quickly than other contemporary neuro-evolutionary techniques and reinforcement learning methods. Traditionally a neural network topology is chosen by a human experimenter, and effective connection weight values are learned through a training procedure. This yields a situation whereby a trial and error process may be necessary in order to determine an appropriate topology. NEAT is an example of a topology and weight evolving artificial neural network (TWEANN) which attempts to simultaneously learn weight values and an appropriate topology for a neural network.
In order to encode the network into a phenotype for the GA, NEAT uses a direct encoding scheme which means every connection and neuron is explicitly represented. This is in contrast to indirect encoding schemes which define rules that allow the network to be constructed without explicitly representing every connection and neuron allowing for more compact representation.
The NEAT approach begins with a perceptron-like feed-forward network of only input neurons and output neurons. As evolution progresses through discrete steps, the complexity of the network's topology may grow, either by inserting a new neuron into a connection path, or by creating a new connection between (formerly unconnected) neurons.
I implement this algorithm using [neat-python](https://github.com/CodeReclaimers/neat-python).


## Instruction <a id=inst> </a>

You just need to run ```flappy bird ML.py```, the file ```config.txt``` contain the best configuration for the NEAT so this file help you to speed up the training process.
