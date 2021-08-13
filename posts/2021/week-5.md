---
author: Abhipsha Das
date: 2021-07-30
tags: pymc
---

# Commits, Commits and More Commits

It’s been a few months since I began contributing to [pymc-examples](https://github.com/pymc-devs/pymc-examples) and the experience so far has been enlightening. For someone who previously could only covetously look upon my fellow classmates as they contributed away to open source projects while I was still struggling with git and the jargon used in a project, I feel like I have come a relatively long way, thanks in no small part to the PyMC community members. I have gained some understanding of Bayesian inference and statistical concepts while updating the example notebooks, which are a set of jupyter notebooks hosted for the reference of newcomers trying to do probabilistic programming with PyMC3. 

For some context, Bayesian inference means drawing statistical inferences using [Bayes’ theorem](https://en.wikipedia.org/wiki/Bayes%27_theorem) to update the probability of a premise/hypothesis as and when we obtain more evidence for our defined premise. We define a statistical model for our data based on which a likelihood function and prior probability is derived, and based on these two, a posterior probability is obtained. It is a common and convenient way to update our hypothesis inside a statistical framework. So the steps of Bayesian inference can be summarized as: get observed data, build a probabilistic model to represent the data, specify prior distributions and apply Bayes’ theorem for inference and updating our hypothesis.

[PyMC3](https://github.com/pymc-devs/pymc3) is basically a tool with which Bayesian inference can be performed. It is a python package for probabilistic programming  - which itself is simply a programming type that employs computer programming for statistical modelling. It is a very useful package that has a well-documented and extensive API for anyone working on and interested in statistical modelling. And since documentation is important, the project provides tutorials for all beginners, intermediate and advanced users of PyMC3 in the form of jupyter notebooks. That’s where I come in! 

Since all software projects are continuously developing, and require maintenance and regular updates to keep up with the best coding practices, the tutorial notebooks hosted at the pymc-examples repository need to all be updated so that they follow the latest practices in python programming. The notebooks also need to be converted to discard the older dependencies that PyMC3 had - like theano - and be updated to depend on python packages like ArviZ, xarray, Aesara, bambi, formulae and more, keeping in mind that the notebooks follow the latest best practices and cover the topic as well as they had with the older dependencies. Also, while these tasks are code-oriented, they mainly serve as references in documentation for users of PyMC3, so the repository aims at covering as much ground as possible with regard to statistical modelling. This means that the documentation needs to be continuously updated too - which I partly help with - and new notebooks covering more statistical concepts need to be added - which is a community effort which I also help with. 

It’s a difficult task to be able to work on notebooks when I could not understand much of the underlying mathematical concepts, especially if the updates I make are not trivial or simply syntax-based (an example of this would be updating instances of `numpy.random` to `numpy.random.default_rng()`), so my mentor and I have come up with a workflow that helps me understand concepts bit-by-bit and not be overwhelmed with the influx of information.

A new version of PyMC3 - PyMC3 v4 (as counterintuitive as the name sounds) - is set to release soon, and when that happens I will have new round of updates to do, so I hope I can update most of the 81 notebooks in the repository to make the transition smoother!