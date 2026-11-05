# Module 8: Generative Adversarial Learning

Week 9 · Graduate seminar and research lab

## Start with the idea: Generating new examples

A generative adversarial network (GAN) has two models. The generator transforms random inputs into samples. The discriminator learns to distinguish generated samples from real examples; its feedback helps train the generator.

## A concrete example

Use data with three clusters in a two-dimensional plane. Generated points should cover all three clusters. If they cover only one, the generator has missed important variation, even if those points look realistic.

## Quick check

Can realistic individual samples still give poor coverage of the data?

The sections below develop the mathematics and the practice experiment. For every experiment, record the data split, baseline, settings, result, and one limitation.

## Learning objectives

Analyze the adversarial objective; diagnose instability; assess sample diversity and coverage.

## Core concepts

Generator–discriminator games, minimax and non-saturating objectives, DCGAN, mode collapse, and evaluation limitations.

## Mathematical preparation and derivation

Derive the optimal discriminator D*(x) = p_data(x)/(p_data(x)+p_g(x)) for fixed generator where the denominator is nonzero. Explain why this idealized result does not ensure stable finite-network training.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Train a small GAN on a two-dimensional multimodal synthetic distribution. Compare minimax and non-saturating generator losses across seeds. Plot samples, mode coverage, and learning traces. A small image DCGAN is optional.

Prepare runnable code, environment details, one results table or figure, and a 500–800 word explanation. State what the result shows and one limitation. Use a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Can visually convincing samples coexist with severe mode collapse?

Bring one claim, supporting evidence, and one alternative explanation. An **ablation** changes or removes one component to test its contribution.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_generative-adversarial-networks/index.html), sections 20.1–20.2. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
