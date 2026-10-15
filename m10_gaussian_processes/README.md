# Module 10: Gaussian Processes and Uncertainty-Aware Model Selection

Week 11 · Graduate seminar and research lab

## Learning objectives

Derive GP posterior predictions; distinguish uncertainty sources; evaluate calibration and selection cost.

## Core concepts

Kernels, Gaussian process priors and regression, observation noise, predictive intervals, and budgeted hyperparameter selection.

## Mathematical preparation and derivation

Derive the Gaussian posterior mean K_*X(K_XX + sigma_n^2 I)^(-1)y and covariance K_** - K_*X(K_XX + sigma_n^2 I)^(-1)K_X*. Distinguish latent-function uncertainty from noisy-observation uncertainty.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Fit a GP on small synthetic regression data and compare kernels and noise assumptions. Measure held-out error and predictive interval coverage, including an extrapolation region. Use a declared validation budget for kernel selection; compare with a simple regression baseline.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Why can credible intervals be narrow yet unreliable under model misspecification?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_gaussian-processes/index.html), sections 18.1–18.3; revisit 19.1 and 19.3–19.5 for selection budgets. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
