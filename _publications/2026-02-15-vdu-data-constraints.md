---
title: "📝 Unlearning in Diffusion Models under Data Constraints: A Variational Inference Approach"
collection: publications
permalink: /publication/2025-10-05-vdu-data-constraints
excerpt: '🎯 The principal objective of this work is to propose a machine unlearning methodology that can prevent the generation of outputs containing undesired features from a pre-trained diffusion model in a data-constrained setting, where the whole training dataset is inaccessible.'
date: 2026-02-15
venue: 'Transaction on Machine Learning Research.'
authors: 'Subhodip Panda, Varun M S, Shreyans Jain, Sarthak Kumar Maharana, Prathosh A. P'
venue_short: 'TMLR 2026'
year: 2026
type: 'preprint'
image: 'VDU.drawio.png'
paperurl: 'https://arxiv.org/abs/2510.04058'
citation: ''
---
👥 **Co-authors:** [Varun MS](https://scholar.google.com/citations?user=iMHsOeUAAAAJ&hl=en), [Shreyans Jain](https://in.linkedin.com/in/shreyans-jain-1b56aa247), [Sarthak Maharana](https://sarthaxxxxx.github.io/), [Prathosh A.P](https://sites.google.com/view/prathosh/home).

![VDU](/images/VDU.drawio.png#right)

For a responsible and safe deployment of diffusion models in various domains, regulating the generated outputs from these models is desirable because such models could generate undesired, violent, and obscene outputs. To tackle this problem, recent works use machine unlearning methodology to forget training data points containing these undesired features from pre-trained generative models. However, these methods proved to be ineffective in data-constrained settings where the whole training dataset is inaccessible. Thus, the principal objective of this work is to propose a machine unlearning methodology that can prevent the generation of outputs containing undesired features from a pre-trained diffusion model in such a data-constrained setting. Our proposed method, termed as **Variational Diffusion Unlearning (VDU)**, is a computationally efficient method that only requires access to a subset of training data containing undesired features. Our approach is inspired by the variational inference framework with the objective of minimizing a loss function consisting of two terms: plasticity inducer and stability regularizer. Plasticity inducer reduces the log-likelihood of the undesired training data points, while the stability regularizer, essential for preventing loss of image generation quality, regularizes the model in parameter space. We validate the effectiveness of our method through comprehensive experiments for both class unlearning and feature unlearning. For class unlearning, we unlearn some user-identified classes from MNIST, CIFAR-10, and tinyImageNet datasets from a pre-trained unconditional denoising diffusion probabilistic model (DDPM). Similarly, for feature unlearning, we unlearn the generation of certain high-level features from a pre-trained Stable Diffusion model trained on LAION-5B dataset. ⏩ [Full Paper](https://arxiv.org/abs/2510.04058)
