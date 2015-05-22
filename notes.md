---
layout: page
title: Workshop Notes
---

# Rich Turner

Rich talked about the challenges of using inducing point methods in time series and introduced a chain-structured pseudo point approximation. The key twist is to place a chain structure on the inducing inputs.

Inducing variables delete links until it looks like factor analysis. Here you delete dependencies until you get an LDS.

A further approximation within the FITC/PITC class where you replace the prior with a first order dynamical system.


work with Thang Bui

# Marc Deisenroth

Properties of approximations

Scale to large data sets

Good approximation to the ground truth.

Preditions indepedendent of computational graph.

# Michalis

Is the actual problem that we should be finding ways to represent a Gaussian process in a non-distributed manner?

Have global property that the full GP is the sum of some local GPs.

Partition the kernel using squashing functions. Assume conditional dependence which respects the clustering strucure. 

# Jose

Use Assumed Density Filtering ideas plus a factorized approximation to the posterior to give a stochastic back propagtion-like algorithm for optimizing Bayesian neural networks.

Use autograd or Theano for back propagation.

Good performance on range of data sets (Boston, Concrete, Energy etc).

Interesting the different effect of the rectified linear units vs sigmoidal.

# Ole

1) Can we derive convergence conditions for EP?

In practice empirically, it seems EP is actually a lower bound. Is this true? Ulrich will talk more about this tomorrow.

For Ising model, tilted distribution is tractable.

Can proove that if a fixed point exists it's attractive for GP in a box and for repeated box factors (see John Cunningham talk).

2) Can we justify parallel and damped versions of EP.

Pre EP work, adaptive TAP (Winther and Opper) is looking for the same fixed points of EP.

Show that if the dynamics covergence they do to EP fixed points.

# Michael

Structured Sparsity Models, where data is both structured and sparse. Build priors to encode this information.

# James

Sparse Variational GPs for classification.


# Simo

Hilber space methods for approximate


# Manfred

Esitmating the drift of Gaussian processes.

Handling non-linear noise terms in SDEs.

# Heiko