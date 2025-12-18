# VAE-with-a-VampPrior
PyTorch implementations of Standard VAE, VampPrior VAE, and Hierarchical VampPrior VAE via the paper implementation of VAE with a VampPrior.

The Notebook provides code to train a Standard VAE, VampPrior VAE, and Hierarchical VampPrior VAE on MNIST dataset, and
provides plots of the prediction comparison, loss plots, KL and reconstruction plots.


VAE with VampPrior in PyTorch

This repository contains PyTorch implementations of Variational Autoencoders (VAEs) with different prior configurations, including:

Standard VAE

VampPrior VAE

Hierarchical VampPrior VAE

These implementations are based on the paper “VAE with a VampPrior”, and demonstrate how alternative priors like VampPrior can improve latent space expressiveness and prevent posterior collapse compared to a standard Gaussian prior.

Features

Train VAEs on MNIST: Easily run experiments on the MNIST dataset.

Comparison Across Models: Train and evaluate Standard VAE, VampPrior VAE, and Hierarchical VampPrior VAE in a single notebook.

Visualization of Results:

Data vs Reconstruction: Compare original MNIST digits with model reconstructions.

Data vs Model Predictions: Compare predictions from Standard VAE, VampPrior VAE, and Hierarchical VampPrior VAE side-by-side.

Loss Curves: Track reconstruction loss and KL divergence over training iterations.

KL Divergence Analysis: Analyze the impact of VampPrior on latent space regularization.

Hierarchical VAE Support: Explore advanced hierarchical VampPrior structures for richer latent representations.
