---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Summary 
==
Applied Research Engineer with experience in deep learning, multi-agent systems, and control.
My recent work focuses on building and optimizing machine learning systems, including
multi-camera Bird’s-Eye-View (BEV) perception pipelines and efficient Vision Transformer models.

I have a strong foundation in control systems and game-theoretic modeling, with published work
in IJCAI, CDC, and MED. I am particularly interested in ML systems for autonomous and embedded
applications, where accuracy, latency, and reliability must be jointly optimized.


Education
======
* B.E in Electronics and Communication, SJCE, Mysore, 2018
* M.S (by Research) in Control and Optimization, Electrical Engineering, IIT Madras, 2022
* PhD in Control and Optimization (part-time pursuing), Electrical Engineering, 2026 expected

Work experience
======
**Researcher — TCS Research**  
*Sep 2021 – Present*

- Modeled strategic interactions in multi-agent systems using Markov games, with applications to energy markets.
- Designed decentralized learning-based bidding strategies achieving near-optimal performance
  (within ~3–6% of best-known strategies) across varying demand regimes.
- Published peer-reviewed research in IJCAI and CDC on equilibrium computation and learning dynamics.

Skills
======
**Programming:** Python, C++, Julia  
**ML Frameworks:** PyTorch, torch.fx, ONNX  
**Systems & Tools:** Docker, Git, MLflow, TensorBoard, ROS, Gazebo  
**Focus Areas:** Vision Transformers, 3D Perception, Model Quantization, Autonomous Systems, MARL

Projects
=== 
1. Multi-Camera BEV Perception via Geometric Projection and Transformers
2. Post-Training Quantization of Vision Transformers
3. MS Thesis: Formation Control and Trajectory Tracking
4. PhD Research: Learning Equilibria via Better-Response Dynamics


[For more details on projects please refer here]({{ site.baseurl }}/projects/)

  

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>



 Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

<!--  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
====== -->
