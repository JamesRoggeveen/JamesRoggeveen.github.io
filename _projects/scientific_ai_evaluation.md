---
layout: page
title: Scientific AI evaluation
description: Expert-built benchmarks and programmatic evaluation infrastructure for scientific reasoning.
img: assets/img/sci-ai-sheet.png
importance: 0
category: postdoc
related_publications: true
---

Frontier language models have improved rapidly at code, partly because software tasks come with unusually clear correctness signals and mature evaluation workflows. Continued progress in mathematics, science, and engineering requires evaluations built by domain experts, grounded in real practice, and graded by symbolic, numerical, or programmatic checks without relying on other language models as judges.

My work in scientific AI evaluation focuses on building domain-centered benchmarks and the infrastructure that makes them possible. With the right programmatic evaluation tools, experts can focus on writing, testing, and refining authentic problems while the evaluation system handles model execution, collaborative review, answer parsing, grading, and failure analysis.

One lesson from this work is that flexible but constrained evaluation interfaces help experts scale. Rather than asking every author to build an arbitrary grading harness from scratch, a shared set of programmatic checks lets contributors generate more problems faster while keeping the benchmark reproducible. In this setting, constraints often breed creativity.

{% include figure.liquid path="assets/img/sci-ai-sheet.png" class="img-fluid rounded z-depth-1" zoomable=true caption="Example evaluation pipeline for HARDMath2: domain experts authored and reviewed problems in shared Google Sheets and Colab notebooks, while the evaluation system handled model runs, parsing, grading, and live feedback directly on the Google Sheet." %}

#### Benchmark Infrastructure

My two published benchmarks relied on infrastructure I developed to integrate model querying and grading directly into Google Sheets. Problem authors could write prompts and symbolically graded LaTeX answers in a shared sheet, run live model evaluations on their own problems, and receive immediate feedback on parsing, prompt clarity, and difficulty.

This let authors systematically fix problems in real time and ensured that the final benchmark contained many problems already compatible with the evaluation pipeline. Authors could contribute many tasks without needing to manage model APIs, grading harnesses, or evaluation bookkeeping themselves, which was especially important because many contributors were not software experts by training.

#### HARDMath2

I co-led HARDMath2 {% cite hardmath2 %}, a 211-problem benchmark for graduate-level applied mathematics accepted to NeurIPS Datasets & Benchmarks 2025. The benchmark was built with more than 40 graduate students in a Harvard applied mathematics course, who developed and peer-reviewed original problems across asymptotics, perturbation methods, PDEs, and related topics as part of their weekly homework assignments. All problems were written with symbolic LaTeX answers that were parsed and evaluated programmatically by my custom LaTeX parsing script.

For this project, I built the collaborative authoring, testing, and automated symbolic-verification infrastructure. The system helped students test problems against frontier models, refine solutions, and produce machine-checkable answers without needing to directly manage the evaluation harness. The course structure created an iterative task-design loop: students tested candidate problems against increasingly capable models and refined them until they reached the desired difficulty level.

{% include figure.liquid path="assets/img/hardmath2-results.png" class="img-fluid rounded z-depth-1" zoomable=true caption="HARDMath2 evaluation results: solve rates across applied-mathematics categories show substantial variation by topic and model, with frontier systems still missing many graduate-level applied math problems." %}

#### CMT-Benchmark

I deployed this evaluation infrastructure for CMT-Benchmark {% cite Pan2025 %}, a condensed-matter theory benchmark built by expert researchers. The benchmark contains 50 original research-level problems evaluated across 17 frontier language models. This benchmark also required enhancing the programmatic verifier to support non-commutative operators, which are critical in many condensed-matter theory tasks.

{% include figure.liquid path="assets/img/cmt-results.png" class="img-fluid rounded z-depth-1" zoomable=true caption="CMT-Benchmark evaluation results: research-level condensed-matter theory tasks remain difficult for frontier models, with low overall solve rates across categories such as DMRG, exact diagonalization, Hartree-Fock, PEPS, QMC, statistical mechanics, and VMC." %}

#### Evaluation Philosophy

Expert creativity scales best when the evaluation interface is constrained enough to be reliable, but flexible enough to express real domain problems. In practice, this means giving experts clean ways to interact with models and programmatic verifiers before they begin writing questions. Predefined verifiers can limit some forms of expression, but they also make it possible to build difficult, reproducible tasks that reveal model behavior.

#### Public Resources

- [HARDMath2 paper](https://arxiv.org/abs/2505.11774)
- [HARDMath2 code and data](https://github.com/JamesRoggeveen/hardmath2_data)
- [CMT-Benchmark paper](https://arxiv.org/abs/2510.05228)
- [CMT-Benchmark code and data](https://github.com/JamesRoggeveen/cmt_benchmark_data)
- [Gemini 3 Deep Think release citing CMT-Benchmark](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-deep-think/)
