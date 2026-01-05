---
title: "Projects"
permalink: /projects/
author_profile: true
---

## **Multi-Camera BEV Perception via Geometric Projection and Transformers**

Implemented an end-to-end Bird’s-Eye-View (BEV) perception pipeline that lifts multi-camera image features into BEV space using calibrated camera geometry and transformer-style aggregation.

- Lifted 2D CNN features into BEV using explicit geometric projection (`lidar2img`) and differentiable grid sampling
- Designed BEV query embeddings and height-aware aggregation for learning spatial representations
- Trained and evaluated on nuScenes for road and vehicle segmentation
- Benchmarked inference performance (~15 FPS on GPU) and analyzed accuracy–latency trade-offs

Some of the predictions are as follows 

![scenario 1](/images/bev/scenario_1.png)

![scenario 2](/images/bev/scenario_2.png)

![scenario 3](/images/bev/scenario_3.png)



---

## **Post-Training Quantization of Vision Transformers**

Built and optimized a lightweight Vision Transformer (ViT) for image classification with a focus on deployment efficiency.

- Implemented a Vision Transformer from scratch in PyTorch
- Applied post-training quantization (PTQ) using `torch.fx` to enable INT8 inference
- Exported the model to ONNX and verified numerical consistency with PyTorch
- Achieved 3.3× model size reduction and 1.5× inference speedup with no measurable accuracy degradation (~70% Top-1)

---

## **Academic Research (Selected)**

### MS Thesis: Formation Control and Trajectory Tracking
- Designed a nonlinear leader–follower control framework using geometric control to maintain rigid formations while tracking smooth trajectories
- Validated through simulation and hardware-in-the-loop experiments on quadrotor platforms (MED 2021)

### PhD Research: Learning Equilibria via Better-Response Dynamics
- Modeled strategic interactions in energy markets using Markov games and learning-based bidding strategies
- Published results in IJCAI and CDC
