# Bayesian Optimisation via Normalising Flows

**Abiel Talwar**

Master of Science in Mathematics (Data Science)
Lancaster University

---

## Abstract

Bayesian Optimisation (BO) is a powerful framework for optimising expensive black-box functions, combining surrogate models with acquisition functions to guide sampling. This dissertation focuses on Gaussian Processes as surrogates, emphasising their uncertainty modelling and kernel design, and addresses the challenge of acquisition function scalability in high dimensions. We propose a novel BO method that replaces the acquisition function with a normalising flow framework, using local Gaussian Processes to learn probability distributions over promising points. Experiments show that our approach scales more efficiently with dimension and achieves faster iterations than standard BO, though it tends towards over-exploitation due to limitations of the local models. We outline strategies for improvement, including adaptive local modelling, geometry-aware flows, and spline-based transformations, to enhance robustness in high-dimensional optimisation.

---

## Dissertation

[**Download Dissertation.pdf**](./Dissertation.pdf)

---

## Overview

This research investigates approaches to integrating normalising flows into Bayesian optimisation as a way to replace the need for maximising acquisition functions in high dimensions. We do this by utilising the notion of *local Gaussian Processes* to gauge where the model should sample from next.

### Key Takeaways

- We use the local Gaussian Processes created at each sampled point to determine parameters for radial normalising flows
- We introduce a reparameterisation of radial normalising flows to allow for more sophisticated control
- Our algorithm (FLOWBO) outperforms traditional BO early on but struggles to incorporate the global sampled landscape effectively — leading to stagnation
- As hoped, our model scales well to high dimensions in terms of speed and computational complexity

### Improvements and Further Work

- **Local modelling**: Our local approximation uses the kernel determined by the global GP (trained on all points). This means local approximations are inaccurate for functions whose scale changes drastically over the landscape (e.g., Ackley). Future work could fit many local GPs akin to TuRBO
- **Flexible transformations**: Radial flows may be replaced with more flexible transformations such as spline-based flows 
---

## Keywords

Bayesian Optimisation, Normalising Flows, Gaussian Processes, High-dimensional Optimisation, Machine Learning, Hyperparameter Tuning