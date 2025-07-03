# COCO-PUF Linear Modeling

This repository contains the mathematical derivation and implementation of a linear model to predict the behavior of Cross-Connection Physically Unclonable Functions (COCO-PUFs), as part of the CS771 Machine Learning course project.

## Problem Statement

We aim to model the response of a 32-bit COCO-PUF system by predicting the outputs `r₀(c)` and `r₁(c)` based on a binary challenge vector `c ∈ {0, 1}³²`. The problem is formulated as a classification task using a linear model derived from signal delay differences in the PUF architecture.

## Approach

- Constructed a mapping φ̃ from the 32-bit challenge vector to a 63-dimensional real-valued feature space.
- Derived a linear decision function of the form: r(c) = (1 + sign(Wᵀ φ̃(c) + b)) / 2
  
- Modeled the upper and lower path signal propagation times as linear functions with distinct time constants.
- Used the difference between signal delays of cross-connected paths to derive the final binary responses.

## Contents

- `CS771_COCOPUF.pdf`: Derivation of the linear model and problem setup.


## References

- Lecture notes from CS771: Introduction to Machine Learning (IIT Kanpur)
- Research on Arbiter PUF and COCO-PUF delay modeling

## Author

- Vashi Diwakar
- CS771 Course Project | IIT Kanpur | July 2024

