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

<div class="row">
  <div class="col-sm-12 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/stander-bal.png" title="STANDER Balancing" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

**Platform:** Led by complete **mechatronic design and fabrication** of robot, integrating EtherCAT real-time communication.

**MPC:** Led by design of a novel **Model Predictive Balance Controller**, validated by reformulating nonlinear dynamics into an efficient representation for real-time QP optimization.

**RL:** Co-developed a **Reinforcement Learning** controller that achieved **zero-shot Sim-to-Real transfer** by integrating identified motor friction parameters.

**Related Materials:**

- [**Paper**] Angular Momentum-Guided Real-Time Control... (T-MECH, Under Review) `[PDF]`
- [**Paper**] Adaptive Curriculum RL... (Robotica) `[PDF]`
- [**Video 1**] **MPC Performance:** Real-time balancing & disturbance rejection `[▶ Watch Video]`
- [**Video 2**] **Sim-to-Real RL:** Zero-shot transfer experiments `[▶ Watch Video]`
