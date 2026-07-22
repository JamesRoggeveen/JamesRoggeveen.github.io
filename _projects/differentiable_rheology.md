---
layout: page
title: Differentiable constitutive modeling
description: Automatic differentiation and model discovery for learning constitutive laws from partial flow measurements.
img: assets/img/auto_rheo/overview.png
importance: 2
category: postdoc
related_publications: true
---

At Harvard I have been building a differentiable tool for learning the tensorial constitutive behavior of complex fluids from partial observations of flow. Constitutive laws relate fluid stress to deformation. For non-Newtonian fluids, those relationships can be nonlinear and difficult to infer from standard bulk rheology alone. Making matters worse, direct flow observations can include confounding geometric factors when those flow observations are averaged over measurement volumes.

{% include figure.liquid path="assets/img/auto_rheo/overview.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Differentiable model fitting for rheology: experimental or simulated flow data are passed through a differentiable solver, allowing candidate constitutive models and parameters to be fit directly from observed stresses and strain rates." %}

In {% cite Sunol2025 %}, we built an end-to-end framework that differentiates through a non-Newtonian fluid solver. The method learns tensor-valued stress responses from partial flow measurements, such as velocity fields, rather than assuming that the correct constitutive law is already known.

The central idea is to combine physical simulation, automatic differentiation, and structured machine learning. A frame-invariant tensor-basis neural network represents the unknown stress response, while differentiable simulation supplies gradients from observable flow data back to the constitutive model.

My main contribution was the differentiable one-dimensional fitting and model-identification layer. Rather than treating a neural constitutive closure as the final output, this part of the workflow turns learned or measured stress responses back into interpretable rheology. I built an ODE-based fitting framework that jointly fits families of classical constitutive laws to rheometry time series, ranks candidate models with the Bayesian Information Criterion, and recovers physical parameters from the best-supported model.

This is important because a model that fits one experiment but cannot be interpreted or transferred to another geometry is usually not enough for scientific or engineering use. The recovered models are compatible with existing flow simulations and reflect the idea that we should not use a more complex constitutive law than the available data justify.

The model-identification results also show that failures are informative. When the fitting procedure chooses the wrong constitutive family, those failures cluster in particular parameter regimes, indicating that the experimental protocol did not sufficiently probe the relevant material response. This points toward an adaptive workflow whereby direct flow measurements or 1D rheometry traces could be selected iteratively to target the regimes where the current data are least informative.

{% include figure.liquid path="assets/img/auto_rheo/parameter_id.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Parameter and model identification across simulated constitutive laws using differentiable fitting of one-dimensional rheometry traces. Model-identification failures are not random: they correlate with particular parameter ranges, revealing blind spots where the available forcing protocol does not sufficiently distinguish candidate models. This suggests an adaptive experimental loop in which new measurements are chosen on the fly to target parameter regimes where the current protocol is least informative." %}
