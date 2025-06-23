# Home Assignment 4 - Neural Networks and Deep Learning

**Course**: CS5720 Neural Networks and Deep Learning  
**Term**: Summer 2025  
**University**: University of Central Missouri  
**Department**: Computer Science & Cybersecurity  
**Total Points**: 100  

---

## Student Information

Name: Thota Praneeth Babu

700#: 700777380

---

## Table of Contents

1. [Overview](#overview)
2. [Assignment Tasks](#assignment-tasks)
3. [Installation](#installation)
4. [How to Run](#how-to-run)
5. [Generated Outputs](#generated-outputs)
6. [Ethical Considerations](#ethical-considerations)
7. [License](#license)

---

## Overview

This assignment covers Generative Adversarial Networks (GANs), AI ethics and harms, and practical implementations of GANs and data poisoning. It is structured around conceptual explanations and coding exercises aligned with Chapters 11 and 12 of the course textbook.

---

## Assignment Tasks

### 1. Adversarial Process in GAN Training

Describes how GANs use competition between a Generator (G) and Discriminator (D) to generate realistic data. The generator maps noise vectors to data space, while the discriminator distinguishes real from fake samples. This adversarial setup pushes both networks to improve iteratively.

> **Goal**: Converge to a point where the discriminator can no longer tell real from fake data (D(x) = 0.5).

### 2. Ethics and AI Harm – *Misinformation in Generative AI*

**Example**: A generative AI used in journalism misreports sensitive topics like election results, spreading misinformation.

**Mitigation Strategies**:
- Require human expert review of AI-generated content.
- Apply digital watermarking to AI outputs for traceability.

### 3. Programming Task: Basic GAN on MNIST

- Implement a GAN using PyTorch or TensorFlow
- Design the Generator and Discriminator
- Train the model on MNIST digits
- Output samples at Epoch 0, 50, and 100
- Plot losses of both models over time

**Deliverables**:
- Image samples from training
- Plots of Generator and Discriminator loss

### 4. Programming Task: Data Poisoning Simulation

- Build a basic sentiment classifier (e.g., on movie reviews)
- Inject poisoned data by flipping labels related to a specific entity
- Evaluate performance before and after poisoning

**Deliverables**:
- Accuracy and confusion matrix (before vs. after attack)
- Short analysis of the impact

### 5. Legal & Ethical Implications of GenAI

Topics covered:
- Memorization of private user data (e.g., GPT-2)
- Generation of copyrighted content

**Discussion**: Justify whether restrictions on training data are necessary to uphold legal and ethical standards.

### 6. Bias & Fairness Tools (Aequitas)

Use Aequitas to audit fairness metrics:
- Choose a bias metric like **false negative rate parity**
- Describe what it measures, its importance, and common pitfalls

---

## Installation

```bash
pip install torch torchvision matplotlib aequitas
```

---

## How to Run

1. Run `gan_mnist.py` for the GAN training task
2. Run `poisoning_simulation.py` for the sentiment classifier poisoning
3. Use `plot_results.py` to generate loss and evaluation plots
4. Run Aequitas analysis via the provided Jupyter Notebook

---

## Generated Outputs

- MNIST digit images (epoch checkpoints)
- Generator/Discriminator loss comparison plots
- Accuracy and confusion matrix for poisoned vs. clean data

---

## Ethical Considerations

The assignment reflects on the broader societal impact of generative models, addressing misinformation, fairness, and privacy. Students are expected to critically engage with these issues alongside technical work.

---
