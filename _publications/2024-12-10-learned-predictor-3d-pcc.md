---
title: "Learned Nonlinear Predictor for Critically Sampled 3D Point Cloud Attribute Compression"
collection: publications
category: conferences
permalink: /publication/2024-12-10-learned-predictor-3d-pcc
excerpt: #''
date: 2024-10-30
venue: 'IEEE International Conference on Image Processing (ICIP 2024)'
slidesurl: #''
paperurl: 'https://arxiv.org/pdf/2311.13539'
bibtexurl: #''
citation: #''
---
We study 3D point cloud attribute compression via a volumetric approach: assuming point cloud geometry is known at both encoder and decoder, parameters \\(\theta\\( of a continuous attribute function \\(f: \mathbb{R}^3 \mapsto \mathbb{R}\\( are quantized to \\(\hat{\theta}\\( and encoded, so that discrete samples \\(f_{\hat{\theta}}(\x_i)\\( can be recovered at known 3D points \\(\x_i \in \mathbb{R}^3\\( at the decoder Specifically, we consider a nested sequences of function subspaces \\(\cF^{(p)}_{l_0} \subseteq \cdots \subseteq \cF^{(p)}_L\\(, where \\(\cF_l^{(p)}\\( is a family of functions spanned by B-spline basis functions of order \\(p\\(, \\(f_l^*\\( is the projection of \\(f\\( on \\(\cF_l^{(p)}\\( and encoded as low-pass coefficients \\(F_l^*\\(, and \\(g_l^*\\( is the residual function in orthogonal subspace \\(\cG_l^{(p)}\\( (where \\(\cG_l^{(p)} \oplus \cF_l^{(p)} = \cF_{l+1}^{(p)}\\() and encoded as high-pass coefficients \\(G_l^*\\(. In this paper, to improve coding performance over \textbf{\cite{do2023volumetric}}, we study predicting \\(f_{l+1}^*\\( at level \\(l+1\\( given \\(f_l^*\\( at level \\(l\\( and encoding of \\(G_l^*\\( for the \\(p=1\\( case (RAHT(\\(1\\()). For the prediction, we formalize RAHT(1) linear prediction in MPEG-PCC in a theoretical framework, and propose a new nonlinear predictor using a polynomial of bilateral filter. We derive equations to efficiently compute the critically sampled high-pass coefficients \\(G_l^*\\( amenable to encoding. We optimize parameters in our resulting feed-forward network on a large training set of point clouds by minimizing a rate-distortion Lagrangian. Experimental results show that our improved framework outperformed the MPEG G-PCC predictor by \\(11\\( to \\(12\%\\( in bit rate reduction.