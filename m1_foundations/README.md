# Module 1: Deep Learning Foundations and Research Practice

Week 1 · Graduate seminar and research lab

## Learning objectives

Analyze generalization; derive backpropagation; construct leakage-resistant baselines.

## Core concepts

Risk minimization, automatic differentiation, initialization, regularization, and experimental controls.

## Mathematical preparation and derivation

Derive softmax cross-entropy gradients and explain how validation-based model selection differs from final test evaluation.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Compare softmax regression and an MLP on Fashion-MNIST using fixed splits. Add one regularization ablation, repeat stochastic runs, and report uncertainty and compute.

For practice and feedback, prepare code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Which changes improve generalization rather than merely training fit?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_multilayer-perceptrons/index.html), sections 3.6–3.7, 4.6–4.7, 5.3–5.6; review chapters 2–6 as needed. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
