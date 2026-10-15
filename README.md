# Advanced Artificial Intelligence

[View the course website](https://aligunesgit.github.io/advanced-artificial-intelligence/)

Graduate course · Proposed 12-week curriculum · English teaching materials

Primary textbook: Aston Zhang, Zachary C. Lipton, Mu Li, and Alexander J. Smola, [Dive into Deep Learning](https://d2l.ai/index.html), online edition 1.0.3 checked on 15 October 2026. The course follows its PyTorch track.

The course title remains Advanced Artificial Intelligence, with a focus on deep learning and selected advanced learning methods. Foundational chapters are prerequisite review; graduate depth comes from derivations, controlled ablations, paper critiques, and the research project. The book is used selectively rather than covered in full.

## Course information

- Instructor: Ali Gunes; institutional details to be confirmed.
- Level: graduate (MSc; adaptable for doctoral students).
- Format: 10 content modules and 2 research project sprint weeks.
- Suggested weekly contact: 2 hours of lecture/seminar and 2 hours of lab.
- Suggested independent study: 6–8 hours per week.
- Credits, official contact hours, semester dates, and institutional assessment rules: TBD.

This curriculum follows the folder and navigation structure of the existing MLOps and Software Design and Architecture courses. Duration, workload, and assessment weights are proposals pending instructor approval.

## Prerequisites

Undergraduate AI or equivalent; supervised learning and neural network basics; Python and NumPy; linear algebra, multivariable calculus, probability, and basic optimization. Review the [preparation checklist](pages/before.md) before starting.

## Learning outcomes

By the end of the course students should be able to:

1. Formulate an AI research question with a falsifiable hypothesis and appropriate baselines.
2. Derive and analyze algorithms for optimization, representation learning, attention, and sequential decisions.
3. Implement small-scale experiments and evaluate statistical and computational trade-offs.
4. Critically assess convolutional, recurrent, attention-based, generative, and Gaussian process approaches.
5. Diagnose leakage, distribution shift, unreliable uncertainty estimates, and unsupported scientific claims.
6. Produce and defend a reproducible research report with an ablation and a clear account of limitations.

## Course organization

| Week | Module | Topic |
|---|---|---|
| 1 | [M1](m1_foundations/README.md) | Deep Learning Foundations and Research Practice |
| 2 | [M2](m2_optimization/README.md) | Optimization and Hyperparameter Search |
| 3 | [M3](m3_cnn/README.md) | Convolutional Architectures and Residual Learning |
| 4 | [M4](m4_transfer_learning/README.md) | Transfer Learning and Computer Vision |
| 5 | [M5](m5_sequence_models/README.md) | Sequence Models and Recurrent Networks |
| 7 | [M6](m6_transformers/README.md) | Attention and Transformer Architectures |
| 8 | [M7](m7_nlp_pretraining/README.md) | Representation Pretraining and NLP Adaptation |
| 9 | [M8](m8_generative_models/README.md) | Generative Adversarial Learning |
| 10 | [M9](m9_reinforcement_learning/README.md) | Sequential Decision Making and Reinforcement Learning |
| 11 | [M10](m10_gaussian_processes/README.md) | Gaussian Processes and Uncertainty-Aware Model Selection |
| 6 | [Sprint A](sprint_a_project/README.md) | Research proposal and baseline reproduction |
| 12 | [Sprint B](sprint_b_final_project/README.md) | Final experiments, report, and oral defense |

Follow the chronological [time plan](pages/timeplan.md). Each module includes a mathematical task, a required experiment, reading, and seminar questions. These are teaching notes and assignment briefs; full lecture slides and reference solutions are not yet supplied.

## Proposed assessment

| Component | Weight |
|---|---|
| Four individual lab reports (M1, M3, M5, M7) | 30% |
| Individual paper critique and seminar presentation | 15% |
| Sprint A proposal and reproduced baseline | 15% |
| Sprint B research report and reproducibility package | 30% |
| Individual oral defense | 10% |

All module labs are formative learning activities; only the four named reports contribute to the 30% component. See [project requirements and rubrics](pages/projects.md). No publishable novelty is required; a rigorous replication with one justified extension is sufficient.

## Reading and navigation

- [Dive into Deep Learning](https://d2l.ai/index.html): required primary textbook; assigned sections are linked in every module.
- [Textbook-to-course reading map](pages/reading-map.md): required sections, review material, and optional extensions.
- Supplementary primary papers are selected with the instructor for the individual critique.

Textbook prose and code are linked rather than copied. Cite the relevant section and comply with the upstream license when adapting code. Textbook examples are starting points; submitting an unchanged example does not satisfy the experimental assignment.

See [preparation](pages/before.md), [projects](pages/projects.md), [FAQ](pages/faq.md), [concept map](pages/overview.md), and [slides status](pages/slides.md).
