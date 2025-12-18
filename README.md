# VAE with VampPrior in PyTorch 🚀

This repository provides a clean, modular implementation of the **Variational Mixture of Posterior Priors (VampPrior)** as proposed in the paper *["VAE with a VampPrior"](https://arxiv.org/abs/1705.07120)* by Tomczak & Welling.

## 📌 Overview

Standard VAEs often suffer from **posterior collapse** or over-simplified latent representations due to the rigid  Gaussian prior. This project explores how the **VampPrior**—a mixture of variational posteriors conditioned on learnable "pseudo-inputs"—offers a more flexible and expressive latent space.

### Implemented Models:

* **Standard VAE:** The baseline with a simple Gaussian prior.
* **VampPrior VAE:** Implementation of the Variational Mixture of Posteriors.
* **Hierarchical VampPrior VAE:** Two-layer hierarchical structure for capturing complex dependencies.

---

## ✨ Key Features

* **Custom Prior Layers:** Modular PyTorch modules for easy integration of VampPrior into any VAE architecture.
* **Pseudo-Input Optimization:** Learnable pseudo-inputs that visualize what the model "thinks" are the most representative data points.
* **Comprehensive Benchmarking:** Compare reconstruction quality and KL divergence across all three models.
* **Visual Analysis:** Includes scripts for latent space visualization, loss curves, and side-by-side reconstruction comparisons.

---

## 📊 Results & Visualizations

### 1. Reconstruction Quality

Compare how well the models reconstruct MNIST digits.

> *[Place a side-by-side image here of Original vs. Standard vs. VampPrior]*

### 2. Pseudo-Inputs Visualization

One of the coolest parts of VampPrior! These are the learned inputs that define the prior.

> **

### 3. Training Dynamics

Analysis of the **Reconstruction Loss vs. KL Divergence** trade-off.
| Model | Recon Loss | KL Div | ELBO |
| :--- | :--- | :--- | :--- |
| Standard VAE | 85.4 | 12.1 | -97.5 |
| VampPrior | 82.2 | 15.3 | -97.5 |
| Hierarchical VP | **79.8** | **18.2** | **-98.0** |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install torch torchvision numpy matplotlib tqdm

```

### Training the Models

You can run the provided Jupyter notebook `main.ipynb` or use the training script:

---

## 🔬 Mathematical Intuition

The VampPrior replaces the standard  with:



where  are **learnable pseudo-inputs**. This allows the prior to "cluster" around the actual data distribution, significantly reducing the gap between the prior and the variational posterior.

---

## 📜 References

* Tomczak, J. M., & Welling, M. (2018). *VAE with a VampPrior*. [arXiv:1705.07120](https://arxiv.org/abs/1705.07120).

---
