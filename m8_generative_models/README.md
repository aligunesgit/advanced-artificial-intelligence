# Module 8: Generative Adversarial Learning

Week 9 · Graduate seminar and research lab

## Learning objectives

Analyze the adversarial objective; diagnose instability; assess sample diversity and coverage.

## Core concepts

Generator–discriminator games, minimax and non-saturating objectives, DCGAN, mode collapse, and evaluation limitations.

## Mathematical preparation and derivation

Derive the optimal discriminator D*(x) = p_data(x)/(p_data(x)+p_g(x)) for fixed generator where the denominator is nonzero. Explain why this idealized result does not ensure stable finite-network training.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Train a small GAN on a two-dimensional multimodal synthetic distribution. Compare minimax and non-saturating generator losses across seeds. Plot samples, mode coverage, and learning traces. A small image DCGAN is optional.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Can visually convincing samples coexist with severe mode collapse?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_generative-adversarial-networks/index.html), sections 20.1–20.2. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
