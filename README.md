<!-- # Mirror Descent Optimisation -->
This repository hosts the code submitted as part my Individual Project for the 
MSc in Artificial Intelligence at Imperial College London. All code is written in Python3.
<!--For all the dependencies refer to the relevant paragraph of the README file.-->

# Mirror Descent and Interacting Mirror Descent for almost dimension-free optimisation on non-Euclidean spaces

An investigation of Mirror Descent and Interacting particle Mirror Descent optimisation on different problems.
Many fundamental optimisation problems in machine learning and artificial intelligence have at the core of their frameworks the search of an optimal set parameters that lead to the minimisation or maximisation of a differentiable convex or non-convex objective function over either constrained or unconstrained feasible sets. A plethora of these problems utilise iterative methods that compute the gradient of the objective function at each iteration and take a step towards the steepest ascent or descent. A widely used optimisation method is stochastic gradient descent. Stochastic Gradient Descent is typically well-performing for optimising over Euclidean vector spaces. However, Stochastic Gradient Descent  does not always manage to converge to the optimum due to scaling of the dimensionality of the problem on non-Euclidean spaces, or due to noisy computations of the gradient and frequently proves to be expensive if the optimisation is constrained.  In this project we study an other almost dimension-free iterative optimisation algorithm called Mirror Descent and its variant Interacting particles Mirror Descent on six convex frameworks with convex objective functions. Our aim is to observe the performance and  convergence properties  of these methods and also compare them with the standard Stochastic Gradient Descent method. We show that the mirror descent algorithms can outperform Gradient Descent in cases of optimisation over constrained sets with certain geometry, such as the probability simplex. Additionally, we demonstrate the benefits in terms of convergence for allowing particles to interact in the case of Mirror Descent.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Dependencies

Several Python packages are required to be install in order to run this code on your local machine:

```
numpy
torch
scipy
sklearn
matplotlib
tqdm
networkx
```

### Installing

Most of the packages can be intalled using ```pip```, ```pip3```, or ```conda``` if you are using Anaconda. 
For example you can run on your bash the following line to install ```pytorch```:

```
pip install torch torchvision
```
Please refer to the website of each package to find explicitly what you need for your system.


## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

* **George Yiasemis** - *Initial work*


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

## References
The main references of these project are:
* Anastasia Borovykh, Nikolas Kantas, Panos Parpas, and Grigorios Pavliotis. On
stochastic mirror descent with interacting particles: convergence properties and
variance reduction, 07 2020.

* Anastasia Borovykh, Nikolas Kantas, Panos Parpas, and Grigorios A. Pavliotis.
On stochastic mirror descent with interacting particles: convergence properties
and variance reduction, 2020.
