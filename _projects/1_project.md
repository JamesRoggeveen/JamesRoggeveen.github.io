---
layout: page
title: Geometry-driven dynamics in viscous flows
description: Shape, elasticity, and nonreciprocal drift in low-Reynolds-number shear flows.
img: assets/img/hinge/elastic_hinge_drift.png
importance: 3
category: phd
related_publications: true
---

This project studies the dynamics of passive bodies in low-Reynolds-number shear flows. The classical study of these dynamics dates back to Jeffery, who found that rigid ellipsoids tumble in repeating orbits whose dynamics are governed solely by the particle's aspect ratio and initial orientation relative to the flow. 

{% include figure.liquid path="assets/img/hinge/jeff.png" class="img-fluid rounded z-depth-1 mx-auto d-block" width="50%" zoomable=true caption="Path traced out by major axes of ellipsoids undergoing Jeffery orbits. The trajectory is set by the particle's aspect ratio and the initial orientation of the particle relative to the axis of vorticity." %}

In {% cite roggeveen_stone_2022 %}, we studied how hinged particles, consisting of two slender bodies joined at a point, moved in similar kinds of flows. In particular, we were interested in how particle geometry, with a particular focus on asymmetry, drives long-time particle motion.

{% include figure.liquid path="assets/img/hinge/schematic.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Schematic of the hinged particle system. Note the asymmetry parameter q and the hinge angle α." %}

{% include video.liquid path="assets/video/elastic_hinge/rigid_hinge_steady_shear_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true caption="A symmetric rigid hinge in steady shear flow simply tumbles, much like an ellipsoid, but with some periodic vertical motion." %}

{% include video.liquid path="assets/video/elastic_hinge/asym_hinge.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true caption="An asymmetric rigid hinge adopts a fixed orientation and drifts with a persistent vertical motion (horizontal scales are shrunk by a factor of 10)." %}

We found that some asymmetric shapes adopt fixed orientations and drift persistently across streamlines. This gives a minimal model for understanding how particle geometry can produce cross-streamline migration and influence dispersion in suspensions.

Our later work, {% cite Roggeveen2025 %}, asked what changes when the hinge is allowed to open and close under a torsional spring. In steady shear, the elastic body still undergoes Jeffery-like periodic motion, but elasticity adds an internal degree of freedom that changes the trajectory.

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_steady_shear_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}

The most interesting behavior appears in oscillating shear. A rigid body in a time-periodic shear flow has no net displacement over a cycle, but an elastic hinge can execute nonreciprocal shape changes and drift. The direction and magnitude of this drift depend on geometry, spring stiffness, and flow parameters.

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}

{% include figure.liquid path="assets/img/hinge/control.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Effect of changing elasticity on drift speed (left) and the effect of changing equilibrium angle (center) and oscillation frequency (right) on the velocity vector." %}

The dynamics organize around attracting limit cycles in the angular coordinates of the hinge, θ and α. Initial conditions eventually settle to one of two cycles, which correspond to distinct translational drift behaviors. This gives a compact dynamical-systems description of how a passive elastic particle can move in a time-periodic, force-free environment.

{% include video.liquid path="assets/video/elastic_hinge/combined_converge.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}

We used a Poincar&eacute; map to study the basin structure of these cycles. The map contains attracting fixed points and saddle points that define the phase boundary between the two long-time behaviors.

{% include figure.liquid path="assets/img/hinge/poincare_map.png" class="img-fluid rounded z-depth-1 mx-auto d-block" width="50%" zoomable=true caption="Poincaré-map view of the angular dynamics. Periodic orbits of the elastic hinge correspond to fixed points of the map, and saddle points organize the phase boundary between long-time drift states." %}

As the control parameters vary, fixed points and saddles in the Poincar&eacute; map collide and reorganize, producing bifurcations and new long-time drift states. The drifting states appear in mirror-symmetric pairs through subcritical pitchfork bifurcations.

{% include figure.liquid path="assets/img/hinge/bifurcations.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Bifurcation map of the Poincar&eacute; fixed points as the elasticity is varied, showing both the movement of the points on the map plane and in a more traditional bifurcation diagram." %}

#### Long-time drift states

The examples below show hinges initialized near different parts of the phase boundary, together with their θ–α dynamics.

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example_saddle_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}
{% include video.liquid path="assets/video/elastic_hinge/theta_alpha_animation_cycle_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}

{% include video.liquid path="assets/video/elastic_hinge/elastic_hinge_sin_flow_example_saddle_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}
{% include video.liquid path="assets/video/elastic_hinge/theta_alpha_animation_cycle_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true %}
