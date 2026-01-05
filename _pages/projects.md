---
title: "Projects"
permalink: /projects/
author_profile: true
---

## **Multi-Camera BEV Perception via Geometric Projection and Transformers**

Implemented an end-to-end Bird’s-Eye-View (BEV) perception pipeline that lifts multi-camera image features into BEV space using calibrated camera geometry and transformer-style aggregation.

- Implemented a multi-camera BEV perception pipeline in PyTorch, lifting 2D image features into Bird’s-Eye-View space via geometric projection and differentiable grid sampling.
- Designed BEV query embeddings with transformer-style feature aggregation using learned height (Z-axis) attention; trained and evaluated on the nuScenes dataset for road and vehicle segmentation.
- Benchmarked inference performance and evaluated the impact of BEV resolution on runtime, achieving $\sim$15 FPS on GPU.

Some of the predictions are as follows 
<div style="display: flex; gap: 12px; justify-content: center;">
  <img src="{{ site.baseurl }}/images/bev/scenario_1.png" width="32%">
  <img src="{{ site.baseurl }}/images/bev/scenario_3.png" width="32%">
</div>
*Qualitative BEV predictions showing road layout and vehicle occupancy from multi-camera inputs.*

---

## **Post-Training Quantization of Vision Transformers**

Built and optimized a lightweight Vision Transformer (ViT) for image classification with a focus on deployment efficiency.

- Implemented a Vision Transformer (ViT) for CIFAR-10 classification in PyTorch, including custom multi-head self-attention modules.
- Applied Post-Training Quantization (PTQ) using \texttt{torch.fx} to trace computation graphs and perform INT8 calibration.
- Achieved 3.3$\times$ model size reduction and 1.5$\times$ inference speedup while maintaining $\sim$70\% top-1 classification accuracy on CIFAR-10, matching the FP32 baseline.

The results are consolidated as 

| Metric        | FP32       | FX INT8    | Impact        |
|--------------|------------|------------|---------------|
| Accuracy (%) | 70.17      | 70.46      | +0.29%        |
| Speed (FPS)  | 3633       | 5679       | 1.6× faster   |
| Size (MB)    | 3.09       | 0.93       | 3.3× smaller |


---

## **Other Projects**

### MS Thesis: Formation Control and Trajectory Tracking

- Designed a nonlinear leader-follower control framework using geometric control to maintain rigid formations while tracking smooth trajectories, with formal stability analysis.
- Validated the approach through simulation and hardware-in-the-loop experiments on quadrotor platforms, demonstrating convergence of rotation tracking error to small steady-state values ($\approx$ 0.2 under a standard rotation error metric).

The implementation video is as follows.
<div class="embed-container">
  <iframe
      src="https://www.youtube.com/embed/wMIaKA5AQtA"
      width="700"
      height="480"
      frameborder="0"
      allow="autoplay; encrypted-media"
      allowfullscreen="true">
  </iframe>
</div>

  

### PhD Research: Learning Equilibria via Better-Response Dynamics
- Developed a Python-based multi-agent simulation framework to study decentralized decision-making and equilibrium-seeking behavior.
- Designed and evaluated learning dynamics inspired by better-response updates, analyzing convergence and performance against baseline multi-agent policies.
