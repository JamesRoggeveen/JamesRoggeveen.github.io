---
layout: page
title: Elastic hinges
description:
img: assets/img/limit_cycle.png
importance: 2
category: research
related_publications: true
---

Here are animations I made to showcase results from my papers on the motion of hinges in shear flow, {% cite roggeveen_stone_2022 %} and {% cite Roggeveen2025 %}.

In {% cite roggeveen_stone_2022 %}, we studied the motion of rigid hinges in steady shear, which either oscillate vertically while tumbling or drift at a fixed orientation depending on the degree of asymmetry.

{% include video.liquid path="assets/video/elastic_hinge/rigid_hinge_steady_shear_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

When the rigid hinge is replaced with an elastic hinge, as in {% cite Roggeveen2025 %}, with a torsional spring allowing relative rotation of the two arms, the shape of the trajectory is alerted but not fundamentally changed.

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_steady_shear_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

However, when the steady shear flow is replaced with an oscillating shear flow, elastic hinges experience non-reciprocal motion and drift over each period of the flow's oscillation. This is in contrast to rigid hinges, which experience no net displacement over one period of the flow's oscillation.

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

In the paper, we show that the non-reciprocal motion corresponds to one of two limit cycles in the angular coordiantes of the hinge, $\theta$ and $\alpha$. No matter the initial conditions the dynamics eventually settle to one of these two cycles, which correspond to limit cycles in the translational velocity phase plane.

{% include video.liquid path="assets/video/elastic_hinge/combined_converge.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

We can use a Poincar&eacute; map to study the dynamics of these limit cycles. We find two fixed points and two saddle points, corresponding to the phase boudnary, present in the map. Two examples of hinges started near one of the saddle points are given below, along with their $\theta$ - $\alpha$ dynamics and corresponding Poincar&eacute; map.

#### Hinge example one

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example_saddle_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
{% include video.liquid path="assets/video/elastic_hinge/theta_alpha_animation_cycle_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

#### Hinge example two

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example_saddle_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
{% include video.liquid path="assets/video/elastic_hinge/theta_alpha_animation_cycle_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
