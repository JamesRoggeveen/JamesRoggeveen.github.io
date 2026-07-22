---
layout: page
title: Dispersion in structured channels
description: Asymptotic transport theory for solutes in channels with patterned surface topography.
img: assets/img/dispersion/setup.png
importance: 4
category: phd
related_publications: true
---

Our goal was to determine how surface geometry changes long-time transport in low-Reynolds-number channel flows. Classical Taylor dispersion explains how shear flow enhances spreading in a smooth channel. In {% cite Roggeveen2023a %}, we extended this theory to wide channels with small-amplitude surface topography.

{% include figure.liquid path="assets/img/dispersion/setup.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Problem setup: passive tracers move through a wide channel with a structured lower surface and an imposed shear flow. At long times, cross-channel diffusion averages the dynamics into an effective planar transport problem." %}

The result is an effective long-time convection-diffusion equation with an anisotropic dispersion tensor. By decomposing the surface into Fourier modes, we could compute how each mode modifies the classical dispersion tensor, allowing general patterned surfaces to be treated systematically.

One useful consequence is that tilted surface corrugations can rotate the principal direction of dispersion away from the mean flow direction. Transport can be enhanced along one direction while suppressed along another, giving a controlled way to reason about mixing, spreading, and anisotropic transport in structured channels.

#### Single-mode topography

Because the asymptotic correction is mode-by-mode, a single sinusoidal surface gives the cleanest visual example of the mechanism. For a single sinusoidal mode, the theory predicts both drift and an anisotropic correction to dispersion. The paired animations below show how the surface pattern reorganizes spreading and drift in a shear flow.

{% include video.liquid path="assets/video/dispersion/herringbone_dispersion.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true caption="Baseline Taylor dispersion near a flat surface." %}

{% include video.liquid path="assets/video/dispersion/herringbone_drift.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true muted=true caption="Surface-induced drift for a related single-mode topography. The surface mode is arranged at 45 degrees with respect to the direction of travel." %}

#### Gallery of Fluid Motion

{% include video.liquid path="https://www.youtube.com/embed/RF96-_k9OoU?si=p9JqwWbkZ5XWSgUD" class="img-fluid rounded z-depth-1" width="100%" aspect_ratio="16 / 9" %}

This video was prepared for an APS Division of Fluid Dynamics Gallery of Fluid Motion submission with collaborators. It is a visual companion to the asymptotic theory, showing how surface structure can reorganize solute spreading in a shear flow.
