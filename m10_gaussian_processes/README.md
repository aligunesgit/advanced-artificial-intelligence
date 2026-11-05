# Module 10: Gaussian Processes and Uncertainty-Aware Model Selection

Week 11 · Graduate seminar and research lab

## Start with the idea: Predicting with uncertainty

Gaussian process (GP) regression predicts a numerical value and represents uncertainty under a chosen model. A kernel describes how function values at different inputs are related. Observations update the prior to a posterior.

## A concrete example

Suppose a material property has been measured at a few temperatures. A GP predicts between those measurements. Predictions outside the measured region depend strongly on the kernel and noise assumptions.

## Quick check

Why can a narrow predictive interval still be misleading if the model assumptions are wrong?

The sections below develop the mathematics and the practice experiment. For every experiment, record the data split, baseline, settings, result, and one limitation.

## Learning objectives

Derive GP posterior predictions; distinguish uncertainty sources; evaluate calibration and selection cost.

## Core concepts

Kernels, Gaussian process priors and regression, observation noise, predictive intervals, and budgeted hyperparameter selection.

## Mathematical preparation and derivation

Derive the Gaussian posterior mean K_*X(K_XX + sigma_n^2 I)^(-1)y and covariance K_** - K_*X(K_XX + sigma_n^2 I)^(-1)K_X*. Distinguish latent-function uncertainty from noisy-observation uncertainty.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Fit a GP on small synthetic regression data and compare kernels and noise assumptions. Measure held-out error and predictive interval coverage, including an extrapolation region. Use a declared validation budget for kernel selection; compare with a simple regression baseline.

Prepare runnable code, environment details, one results table or figure, and a 500–800 word explanation. State what the result shows and one limitation. Use a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Why can credible intervals be narrow yet unreliable under model misspecification?

Bring one claim, supporting evidence, and one alternative explanation. An **ablation** changes or removes one component to test its contribution.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_gaussian-processes/index.html), sections 18.1–18.3; revisit 19.1 and 19.3–19.5 for selection budgets. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
