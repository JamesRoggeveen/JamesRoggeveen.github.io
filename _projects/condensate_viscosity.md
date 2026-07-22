---
layout: page
title: Measuring condensate material properties
description: Fluid-mechanical models and micropipette aspiration measurements for biomolecular condensates.
img: assets/img/condensate/nucleolus_rescaled_mpa.png
importance: 5
category: phd
related_publications: true
---



Biomolecular condensates are membraneless organelles central to cellular organization, but connecting their biological function to their material properties such as viscosity, surface tension, and viscoelasticity requires quantitative measurements in realistic geometries. Most existing methods identify only one material property, or at best ratios between two properties.

In {% cite Roggeveen2023b %}, we developed a calibration-free model of micropipette aspiration for liquid-like protein condensates. Micropipette aspiration can in principle measure both viscosity and surface tension, but models inherited from membrane-bound objects do not correctly describe unbounded liquid condensates. We derived a hydrodynamic model matched to the aspiration geometry, validated it on silicone oil of known properties, and used it to reinterpret measurements of LAF-1 RGG condensates. Our results indicated LAF-1 RGG has a viscosity of 11±1.1 Pa·s and a surface tension of 0.17±0.02 mN/m.


<div class="row align-items-center justify-content-center">
  <div class="col-md-5">
    {% include video.liquid path="assets/video/condensate/mpa_aspiration.mp4" class="img-fluid rounded z-depth-1 mx-auto d-block" controls=true autoplay=true loop=true muted=true caption="Micropipette aspiration provides a direct mechanical perturbation of small liquid-like condensates. Experiments courtesy of Huan Wang." %}
  </div>
  <div class="col-md-7">
    {% include figure.liquid path="assets/img/condensate/silicone_validation.png" class="img-fluid rounded z-depth-1" zoomable=true caption="By plotting pressure drop against the model fitting parameter, we extract viscosity from the slope and surface tension from the scaled reciprocal intercept." %}
  </div>
</div>

<div class="row justify-content-center">
  <div class="col-md-6">
    {% include figure.liquid path="assets/img/condensate/silicone_collapse.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Collapse of silicone-oil aspiration curves under the calibration-free hydrodynamic model using our experimentally derived material parameters." %}
  </div>
  <div class="col-md-6">
    {% include figure.liquid path="assets/img/condensate/rgg_collapse.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Collapsed aspiration curves for LAF-1 RGG condensates using the same model framework." %}
  </div>
</div>

<div class="float-md-right ml-md-3 mb-3" style="max-width: 120px;">
  {% include video.liquid path="assets/video/condensate/nucleolus_aspiration.mp4" class="img-fluid rounded z-depth-1 mx-auto d-block" controls=true autoplay=true loop=true muted=true caption="Aspiration of two-phase nucleoli in a near-native cellular environment. Purple marks the granular component; green marks the fibrillar component. Experiment by Holly Cheng." %}
</div>

The second part of this line of work applied micropipette aspiration to nucleoli in a near-native cellular environment {% cite Cheng2025 %}. The measurements showed that nucleolar subcompartments have distinct material properties: the outer granular component behaves more fluid-like, while the inner dense fibrillar component is more viscoelastic and depends strongly on RNA.

Because of the wetting properties of these condensates, we could not develop a complete hydrodynamic model. However, we could still show that the elastic response of the fibrillar component arises from cross-linking by long RNA molecules. A viscoelastic solid responds qualitatively differently to aspiration than a fluid; after RNA cleavage, the dense fibrillar component shifted toward a more fluid-like response.

#### Why this matters

Condensates are often described qualitatively as liquid-like or solid-like, but biological function depends on quantitative material properties. This work connects experimental aspiration data to interpretable mechanical models, making it possible to compare viscosity, surface tension, and viscoelastic response across systems and connect those properties to biological function.

{% include figure.liquid path="assets/img/condensate/schematic.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Schematic of the response of different idealized, one-dimensional materials to a stress profile consistent with micropipette aspiration. The fluid-like models (Newtonian, Maxwell) show a linear increase in strain over time, while the solid model (Kelvin-Voigt) saturates at a fixed value." %}
{% include figure.liquid path="assets/img/condensate/untreated.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Untreated nucleoli show distinct mechanical responses across subcompartments. The purple granular component resembles that of a Newtonian fluid while the response of the green fibrillar component resembles a viscoelastic solid." %}
{% include figure.liquid path="assets/img/condensate/treated.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Treated nucleoli show altered aspiration dynamics after perturbing RNA-dependent material structure. Now both materials respond like a fluid." %}

