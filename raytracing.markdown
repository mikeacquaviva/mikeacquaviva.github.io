---
layout: page
title: Deep Learning-Accelerated Ray Tracing
permalink: /projects/raytracing/
---

This work was supported by an [NSERC](https://www.nserc-crsng.gc.ca/students-etudiants/ug-pc/usra-brpc_eng.asp) reserach grant. It was performed under the supervision of [Prof. Costas Sarris](https://sites.google.com/view/cem-pact) as part of a summer research project.

<div style="max-width: 700px; text-align: center; margin: 2rem auto;">
  <img src="/assets/images/Model-High-Level-Flowchart.png" alt="RT-Model" style="width: 100%;  height: auto; border-radius: 12px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

Ray-tracing is a computationally expensive process, especially in complex geometric environments where many reflections, transmissions, and diffractive effects (collectively referred to as *ray-interactions*) must be accounted for. In this project, we limited the number of ray-interactions in our ray-tracer runs to produce low-fidelity maps of recieved signal strength (RSS) from a wireless access point (WAP). The RSS maps were then passed to a physics-informed generative adversarial network (GAN) to improve their fidelity and accuracy. Overall, we saw a reduction in runtime of 85% with a 4% relative error against ground-truth.

Read the paper [here](/assets/Acquaviva_GAN-Paper.pdf).