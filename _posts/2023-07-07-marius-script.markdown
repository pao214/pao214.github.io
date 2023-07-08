---
layout: post
title:  "Marius Script"
---

The task here is to develop a tool to simplify development on a state-of-the-art graph neural network designed at Madison called [MariusGNN](https://github.com/marius-team/marius). To begin, graph neural networks are a more recent family of  deep neural network architectures that are an amazing fit for graph style data. The [book](https://www.cs.mcgill.ca/~wlh/grl_book/) on graph representation learning provides an amazing introduction to the topic. In short, graph neural networks (GNNs for short) use a combination of message passing, neighborhood sampling, feed forward networks, and wisdom from deep neural networks to train embeddings of graph nodes. GNNs can be used for various purposes but can be mainly catergorized into node classification, edge prediction, and graph global classification. The arXiV paper on [MariusGNN](https://arxiv.org/abs/2202.02365) gives an amazing explanation on the same.

There are several challenges with GNNs that make it a difficult problem. Popular frameworks include Amazon's DGL, PyTorch Geometric, and TF-GNN. However, these frameworks do not perform too well because of millions of nodes and billions of edges in contemporary graph data. MariusGNN provides great solutions to mitigate these challenges.

Currently, one of the major drawbracks of Marius is that it is requires certain expertise both in C++ as well as insight into how Marius works. If Marius were to become truly widely adopted, it is imperative that the framework is user-friendly and complies with a very familar interface like Amazon's DGL framework. Much of my work in this project involved designing a compiler that transforms code in a familiar pythonic interface into a C++ one while also abstracting away all the nitty-gritty details of how Marius works.

