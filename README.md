# Bayesian Optimisation via Normalising Flows

**Abiel Talwar**

Master of Science in Mathematics (Data Science)
Lancaster University

---

## Abstract

Bayesian optimisation has emerged as a powerful sample-efficient global optimisation technique for expensive black-box functions. It finds extensive applications in hyperparameter tuning, automated machine learning, and experimental design. At its core, BO iteratively selects the next point to evaluate by maximising an acquisition function built upon a probabilistic surrogate model—typically a Gaussian Process.

However, the performance of standard BO can significantly deteriorate in high-dimensional settings due to the curse of dimensionality. A promising approach to address this challenge is to assume a lower-dimensional latent structure underlying the objective function.

This dissertation explores a novel approach to high-dimensional Bayesian optimisation by embedding normalising flows into the optimisation process. Normalising flows are generative models that learn complex, flexible transformations between probability distributions, enabling efficient density estimation and sampling. We develop and analyse algorithms that embed normalising flows into the BO framework across three distinct integration strategies. Firstly, we embed flows as probabilistic encoders to learn low-dimensional latent representations of the input space. Secondly, we incorporate flows to learn flexible, non-Gaussian acquisition functions. Thirdly, we integrate flows to enhance the Gaussian Process surrogate model by learning non-Gaussian likelihoods and posterior distributions.

We provide a comprehensive theoretical and empirical analysis of these approaches. Through extensive experiments on synthetic benchmarks and real-world hyperparameter optimisation tasks, we demonstrate that flow-enhanced BO can achieve competitive performance compared to standard baselines. The flexibility and expressiveness of normalising flows offer a promising avenue for extending Bayesian optimisation to challenging high-dimensional regimes.

---

## Dissertation

You can view or download the full dissertation below:

[**Download Dissertation.pdf**](./Dissertation.pdf)

### View Online

<div align="center">
  <iframe
    src="./Dissertation.pdf"
    width="100%"
    height="800px"
    style="border: 1px solid #ddd; border-radius: 8px;"
  ></iframe>
</div>

*Note: If the PDF viewer above doesn't load in your GitHub view, please click the download link above or view this repository on GitHub Pages for the best reading experience.*

---

## Overview

This research investigates three novel approaches to integrating normalising flows into Bayesian optimisation:

1. **Flow-based Latent Embedding**: Learning low-dimensional representations of high-dimensional input spaces
2. **Flow-enhanced Acquisition Functions**: Flexible, non-Gaussian acquisition functions
3. **Flow-improved Surrogate Models**: Enhanced Gaussian Processes with non-Gaussian likelihoods

---

## Keywords

Bayesian Optimisation, Normalising Flows, Gaussian Processes, High-dimensional Optimisation, Machine Learning, Hyperparameter Tuning