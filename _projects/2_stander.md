---
layout: page
title: Design and Control of Balancing Robot, STANDER
description: Project Lead | 2022 – 2025
img: assets/img/projects/stander-bal.png
importance: 2
category: work
related_publications: true
---

STANDER is a self-developed, underactuated triple-pendulum platform I engineered from scratch. It serves as a foundational testbed for validating advanced control algorithms.

<div class="row justify-content-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    <img src="/assets/img/projects/stander-bal.png" alt="STANDER Balancing" class="rounded z-depth-1" style="max-width: 100%; max-height: 400px; display: block; margin: 0 auto;">
  </div>
</div>

**Platform:** Led by complete **mechatronic design and fabrication** of robot, integrating EtherCAT real-time communication.

**MPC:** Led by design of a novel **Model Predictive Balance Controller**, validated by reformulating nonlinear dynamics into an efficient representation for real-time QP optimization.

**RL:** Co-developed a **Reinforcement Learning** controller that achieved **zero-shot Sim-to-Real transfer** by integrating identified motor friction parameters.

**Related Materials:**

- [**Paper**] Angular Momentum-Guided Real-Time Control for Stabilizing Under-actuated Triple Pendulums (T-MECH, Under Review) `[PDF]`
- [**Paper**] Adaptive Curriculum Reinforcement Learning with Sim-to-Real Strategy in Balance Control of Underactuated Triple Pendulum Robots (Robotica) `[PDF]`

<div class="row mt-4">
  <div class="col-sm-6">
    <h4>Video 1: MPC Performance</h4>
    <p>Real-time balancing & disturbance rejection</p>
    <div class="embed-responsive embed-responsive-16by9">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/7xTXajSdNSc" allowfullscreen></iframe>
    </div>
  </div>
  <div class="col-sm-6">
    <h4>Video 2: Sim-to-Real RL</h4>
    <p>Zero-shot transfer experiments</p>
    <div class="embed-responsive embed-responsive-16by9">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/2-yskXyq0DA" allowfullscreen></iframe>
    </div>
  </div>
</div>
