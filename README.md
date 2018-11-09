# 100-days-machine-learning-journey
Each day i study a little about machine-learning/deep-learning and share what i learnt

# Journey Plan:
1. CNN
    - Classification
    - Regression
    - Differentiation
1. RNN
1. Reinforcement Learning
1. Meta learning
1. Quantum Machine Learning
1. Decentralize Data

# Journey tracking

## Day 1 - 2018/11/06: What is QUANTUM MACHINE LEARNING?
> QUANTUM COMPUTING(QC) allows for calculation speed millions of times faster than current binary technology. So with Quantum Computing, current Machine Learning algorithm can be computed in a fraction of the time it takes now. Therefore, we can build much LARGER and COPLEX algorithm/neural-networks and compute them in the same amount of time current algorithms take place.

**Quantum Machine Learning(QML):** is attemptions to recast Machine Learning problems in the form of quantum algorithm to be run on quantum computers. 

![](https://github.com/krishnakumarsekar/awesome-quantum-machine-learning/raw/master/Quantum%20Machine%20complete%20Architecture.png)

**How to combine ML and QC?**

There are 4 approaches:
    - CC:
    - CQ:
    - QC:
    - QQ:

![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Qml_approaches.tif/lossless-page1-296px-Qml_approaches.tif.png)

**How to program QML?**
- Firstly, we have to have Quantum simulator.
- Create quantum algorithm then run on simulator.

**What is QML programming languague?** 
Cirq - a software toolkit that lets developers create algorithms without needing a background in quantum physics - initiated by Google.

**Great source for read?** [Awesome Quantum Machine Learning](https://github.com/krishnakumarsekar/awesome-quantum-machine-learning#introduction-why-quantum-machine-learning)

## Day 2 - 2018/11/07: What is META LEARNING in Machine Learning?
> Traditional paradigm in ML need huge dataset to train model for specific task. Obviously, it is very far from how human leverages past experiences to learn very quickly new task from only a handset of examples. It is because human **_learns to learn_**.

**WHAT is Meta Learning?** This is no specific/standard definition for Meta Learning yet. In short, Meta Learning is to learn the learning process(or how to quickly learn some tasks from a tiny set of examples). 

**HOW to do Meta Learning?** 

There are some approaches:
    - recurrent models
    - meta-optimization
    - metric learning

Below is how we learn meta-parameters
![](https://cdn-images-1.medium.com/max/1000/1*AcaPiikZErVv_iFJzWekQg.gif)

**Greate source for read?** [From zero to research — An introduction to Meta-learning](https://medium.com/huggingface/from-zero-to-research-an-introduction-to-meta-learning-8e16e677f78a)(this source is meta-optimization approach and included pytorch code)

Another method meta-learning here: [RL — Meta-Learning](https://medium.com/@jonathan_hui/meta-learning-how-we-address-the-shortcomings-of-our-deep-networks-a008aa4b5b2b)

## Day 3 - 2018/11/08: What is NEUROEVOLUTION in Machine Learning?
> Traditional artificial neural networks use gradient descend for backpropagation to optimize the network parameters. This method may need a lot of epochs to reach optimized solution. In some case, if we select not good hyper-parameters(such as too big learning rate), the result is not converged. Or sometimes, the result gets stucked at local optimum. Is there anyway better way to explore optimum solution? That's why you should try NEUROEVOLUTION.

**WHAT is NEUROEVOLUTION?** Neuroevolution is the way to utilizes genetic algorithms to develop artificial neural networks.

**HOW to do it it?**

1. When you are doing genetic optimisation in the context of DNN optimisation, you start from an initial **_population_** of models. Typically, a model is randomly initialised, and several **_offspring_** are derived based on this initial model. In the case of DNN’s, you initialise a model (as you normally do), and you add small random vectors, sampled from a simple Gaussian distribution, to the parameters. This results in a cloud of models, which all reside somewhere on the optimisation surface. Note that this is the first important distinction with gradient descent. You start (and continue to work) with a population of models, instead of a single (point) model.

1. Starting from this original population, the **_genetic optimisation cycles_** start.
![](https://cdn-images-1.medium.com/max/800/1*KQIGKIZOKJudEf9x_sW5Kw.png)

    - First, a fitness evaluation is performed. Fitness evaluation corresponds with checking where the models are in the optimisation surface and determining which of the models perform best (e.g. are the most fit).

    - Next, a **_selection_** is performed based on the fitness evaluation. In evolution strategies, the (pseudo) offspring is reduced to a single model, weighted by the fitness evaluation. For DNN's the fitness is defined as the loss or the reward. 

    - Next, **_reproduction and combination_** is performed. Based on the newly selected 'prime' model, a new set of offspring is derived.

    - Typically, in genetic optimisation, **_mutation_** is also performed in order to improve the variety of the offspring. One example of mutation is to change how the different offspring is created (i.e. different noise levels for the different parameters).

> The researchers at OpenAI and Uber are able to show that the 'gradient approximation' of evolution strategies leads to satisfying (but not necessarily new state-of-the-art) solutions in supervised learning scenario's. On the other hand they are able to show high performance of their methods in reinforcement learning scenario's (comparable to state-of-the-art in some domains).

**P/S:** I believe a combination of neuroevolution and gradient descent methods will lead to a significant improvement in RL performance. One downside of neuroevolution is the massive amounts of compute power that are required in order to train these systems, which might limit the democratisation of these techniques.
