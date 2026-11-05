# Module 1: Deep Learning Foundations and Research Practice

Week 1 · Graduate seminar and research lab

Begin with the [AI introductory sequence](../intro/what-is-ai.md): what AI is, its approaches, engineering applications, and current developments. This module follows that shared introduction and starts the technical learning track.

## Start with the idea: Learning a prediction rule

A neural network turns inputs into a prediction. During training, a loss measures the prediction error, and backpropagation computes how each parameter affects that loss. An optimizer then updates the parameters.

## A concrete example

For a clothing image, the input is a grid of pixel values and the output is a score for each clothing category. A softmax classifier is a simple starting point; a multilayer perceptron (MLP) adds hidden layers.

## Quick check

A model gets 99% training accuracy and 75% validation accuracy. What might explain the gap?

The sections below develop the mathematics and the practice experiment. For every experiment, record the data split, baseline, settings, result, and one limitation.

## Learning objectives

Analyze generalization; derive backpropagation; construct leakage-resistant baselines.

## Core concepts

Risk minimization, automatic differentiation, initialization, regularization, and experimental controls.

## Mathematical preparation and derivation

Derive softmax cross-entropy gradients and explain how validation-based model selection differs from final test evaluation.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Compare softmax regression and an MLP on Fashion-MNIST using fixed splits. Add one regularization ablation, repeat stochastic runs, and report uncertainty and compute.

Prepare runnable code, environment details, one results table or figure, and a 500–800 word explanation. State what the result shows and one limitation. Use a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Which changes improve generalization rather than merely training fit?

Bring one claim, supporting evidence, and one alternative explanation. An **ablation** changes or removes one component to test its contribution.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_multilayer-perceptrons/index.html), sections 3.6–3.7, 4.6–4.7, 5.3–5.6; review chapters 2–6 as needed. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
