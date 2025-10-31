---
layout: page
title: project 1
description: a project with a background image
img: assets/img/12.jpg
importance: 1
category: research
related_publications: true
---

Here is a brief description of my project on developing a novel, meshless spectral method for solving inverse problems over PDEs on irregular domains. This method leverages automatic differentiation and modern optimizers to achieve exponential convergence.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include combined_converge.html path="assets/video/elastic_hinge/combined_converge.mp4" class="img-fluid rounded z-depth-1" autoplay=true %}
    </div>
</div>
<div class="caption">
    This animation shows the solver finding a solution for a complex boundary value problem.
</div>

The solver is built using JAX and is designed to be a powerful engine for inverse problems, control, and optimization.
