---
layout: page
title: IFGF-Accelerated Electromagnetic Solver
permalink: /projects/thesis/
---

This work was completed as part of my fourth-year thesis in the Engineering Science program at the University of Toronto. It was conducted under the supervision of Prof. Piero Triverio at the [Modelics](http:\\modelics.org) Lab.

<div style="text-align: center;">
  <img src="/assets/images/ifgf.png" alt="Thesis"
       style="width: 400px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);
              margin-bottom: 1rem; border-radius: 12px" />
</div>

<hr style="margin-top: 2.5rem; margin-bottom: 1.5rem;">

## Abstract
<p>The boundary integral formulation of the scattering problem is central to computational electromagnetics, but it results in dense linear systems whose solution is computationally demanding. Fast algorithms such as the Fast Multipole Method (FMM) and the Adaptive Integral Method (AIM) mitigate this cost but can face challenges with parallelism, kernel generality, and high-frequency performance. The Interpolated Factored Green Function (IFGF) method offers a recent alternative, achieving \( \mathcal{O}(N \log N) \) complexity through a decomposition of the Green's function into oscillatory and smooth factors, the latter of which is efficiently interpolated in space. This thesis investigates the IFGF method from both theoretical and practical perspectives. A serial implementation of IFGF was developed in Python for prototyping, and then reimplemented in C++ with an Eigen-based linear algebra engine for integration into \( \texttt{REBEL} \), a GMRES-based electromagnetic solver. The algorithm was validated against direct kernel evaluations and benchmarked for runtime and memory efficiency. In parallel, the performance and scalability of IFGF are discussed in relation to FMM and AIM, with attention given to their structural trade-offs. Experimental results confirm that IFGF achieves near-log-linear scaling in both runtime and memory while preserving accuracy across a range of problem sizes and wavenumbers. This work demonstrates the viability of IFGF as a general-purpose fast solver and establishes a foundation for further comparative studies on complex geometries and large-scale electromagnetic simulations.</p>

<hr style="margin-top: 2.5rem; margin-bottom: 1.5rem;">

You can view the full copy of my thesis [here](/assets/Acquaviva-Thesis_Interpolated-Factored-Green-Function-Method.pdf)

Or view a slideshow summary of the algorithm and results [here](/assets/Acquaviva-Thesis_IFGF-Presentation.pdf)


<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" async></script>
