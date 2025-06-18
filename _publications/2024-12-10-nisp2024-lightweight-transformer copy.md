---
title: "Interpretable lightweight transformer via unrolling of learned graph smoothness priors"
collection: publications
category: conferences
permalink: /publication/2024-12-10-nisp2024-lightweight-transformer
excerpt: #''
date: 2024-12-10
venue: 'Advances in Neural Information Processing Systems 37 (NeurIPS 2024)'
slidesurl: #''
paperurl: 'https://proceedings.neurips.cc/paper_files/paper/2024/file/0c38f54740062529aa4117a04b583f3c-Paper-Conference.pdf'
bibtexurl: #''
citation: #''
---

<!-- We build interpretable and lightweight transformer-like neural networks by unrolling iterative optimization algorithms that minimize graph smoothness priors---the quadratic graph Laplacian regularizer (GLR) and the ℓ1-norm graph total variation (GTV)---subject to an interpolation constraint. The crucial insight is that a normalized signal-dependent graph learning module amounts to a variant of the basic self-attention mechanism in conventional transformers. Unlike "black-box" transformers that require learning of large key, query and value matrices to compute scaled dot products as affinities and subsequent output embeddings, resulting in huge parameter sets, our unrolled networks employ shallow CNNs to learn low-dimensional features per node to establish pairwise Mahalanobis distances and construct sparse similarity graphs. At each layer, given a learned graph, the target interpolated signal is simply a low-pass filtered output derived from the minimization of an assumed graph smoothness prior, leading to a dramatic reduction in parameter count. Experiments for two image interpolation applications verify the restoration performance, parameter efficiency and robustness to covariate shift of our graph-based unrolled networks compared to conventional transformers. -->