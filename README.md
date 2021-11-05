# Machine Learning using NEAT to play Flappy Bird


## Flappy Bird Original Game

Flappy Bird is a mobile game developed by Vietnamese video game artist and programmer Dong Nguyen (Vietnamese: Nguyễn Hà Đông), under his game development company [.Gears](http://dotgears.com). The game is a side-scroller where the player controls a bird, attempting to fly between columns of green pipes without hitting them. Nguyen created the game over the period of several days, using a bird protagonist that he had designed for a cancelled game in 2012.


## Algorithm

In this project for the machine learning I use an algorithm called NEAT. 

NeuroEvolution of Augmenting Topologies (NEAT) is a genetic algorithm (GA) for the generation of evolving artificial neural networks (a neuroevolution technique) developed by Ken Stanley in 2002 while at The University of Texas at Austin. It alters both the weighting parameters and structures of networks, attempting to find a balance between the fitness of evolved solutions and their diversity. It is based on applying three key techniques: tracking genes with history markers to allow crossover among topologies, applying speciation (the evolution of species) to preserve innovations, and developing topologies incrementally from simple initial structures ("complexifying"). On simple control tasks, the NEAT algorithm often arrives at effective networks more quickly than other contemporary neuro-evolutionary techniques and reinforcement learning methods. Traditionally a neural network topology is chosen by a human experimenter, and effective connection weight values are learned through a training procedure. This yields a situation whereby a trial and error process may be necessary in order to determine an appropriate topology. NEAT is an example of a topology and weight evolving artificial neural network (TWEANN) which attempts to simultaneously learn weight values and an appropriate topology for a neural network.
In order to encode the network into a phenotype for the GA, NEAT uses a direct encoding scheme which means every connection and neuron is explicitly represented. This is in contrast to indirect encoding schemes which define rules that allow the network to be constructed without explicitly representing every connection and neuron allowing for more compact representation.
The NEAT approach begins with a perceptron-like feed-forward network of only input neurons and output neurons. As evolution progresses through discrete steps, the complexity of the network's topology may grow, either by inserting a new neuron into a connection path, or by creating a new connection between (formerly unconnected) neurons.
I implement this algorithm using [neat-python](https://github.com/CodeReclaimers/neat-python).


## Instruction

You just need to run ```flappy bird ML.py```, the file ```config.txt``` contain the best configuration for the NEAT so this file help you to speed up the training process.
