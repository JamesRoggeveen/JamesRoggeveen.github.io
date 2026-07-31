---
layout: about
title: about
permalink: /
subtitle: Agent Evaluation | Scientific Reasoning | Applied Mathematics

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >

news: true # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

I am a researcher and applied mathematician building agent evaluations for scientific and engineering domains. My work combines expert-designed tasks, programmatic grading, task quality assessment, and differentiable scientific computing to test and extend the capabilities of frontier AI systems.

I am currently a Postdoctoral Fellow at Harvard University with Prof. Michael Brenner and a Visiting Faculty Researcher at Google DeepMind. At Google DeepMind, I contribute scientific and engineering expertise to evaluating advanced AI reasoning and was publicly credited for foundational support to the [Gemini Deep Think team](https://deepmind.google/blog/accelerating-mathematical-and-scientific-discovery-with-gemini-deep-think/).

My recent work is focused on three connected areas:

- **[Scientific AI Evaluation](/projects/scientific_ai_evaluation/)**: I build infrastructure for evaluating language-model agents on authentic scientific and engineering work. I co-led [HARDMath2](https://arxiv.org/abs/2505.11774), a 211-problem benchmark for graduate-level applied mathematics, and built evaluation infrastructure for [CMT-Benchmark](https://arxiv.org/abs/2510.05228), a condensed-matter theory benchmark built by expert researchers.
- **[Meshless PDE Solvers](https://arxiv.org/abs/2510.25752)**: I developed a meshless, differentiable spectral method for PDE inverse problems on irregular geometries. A useful pattern has been to require coding agents to pass independent numerical checks before reporting results, which helps catch invalid implementations while extending the solver to new applications.
- **[Automated Model Discovery](https://arxiv.org/abs/2510.24673)**: I build differentiable tools for discovering physical laws from partial measurements, including a framework for identifying tensor-valued constitutive laws from sparse flow data.

My Ph.D. in Mechanical Engineering at Princeton University, advised by Prof. Howard A. Stone, focused on particle dynamics in low-Reynolds-number flows and creating improved hydrodynamic models for characterizing the material properties of biological condensates using micropipette aspiration.

Across these projects, I am especially interested in building systems that let domain experts contribute high-quality scientific tasks without needing to own the full evaluation harness. My background gives me both sides of that problem: deep experience in physical modeling and scientific computing, and hands-on experience designing benchmark infrastructure for frontier language models.

Current focus: agent evaluations for scientific and engineering domains; expert-built benchmarks; programmatic grading; symbolic and numerical verification; independent checks for agent-generated scientific code; and task quality assessment.
