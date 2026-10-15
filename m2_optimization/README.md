# Module 2: Optimization and Hyperparameter Search

Week 2 · Graduate seminar and research lab

## Learning objectives

Analyze optimizer updates; compare methods under a fixed budget; avoid tuning leakage.

## Core concepts

SGD, momentum, adaptive optimization, learning-rate schedules, random search, and successive halving.

## Mathematical preparation and derivation

Derive momentum and Adam updates, including bias correction. State what optimizer convergence claims require and why nonconvex neural training complicates them.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Compare SGD, momentum, and Adam on one compact MLP with equal tuning budgets. Compare random search with a simple successive-halving schedule. Keep test data sealed until selection is complete.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Is an optimizer comparison fair if learning rates are tuned for only one method?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_optimization/index.html), sections 12.1–12.6, 12.10–12.11; 19.1 and 19.3–19.5. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
