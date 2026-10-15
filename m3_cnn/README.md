# Module 3: Convolutional Architectures and Residual Learning

Week 3 · Graduate seminar and research lab

## Learning objectives

Analyze convolution shapes and receptive fields; explain residual learning; design architecture ablations.

## Core concepts

Convolutions, pooling, parameter sharing, normalization, residual blocks, and architecture trade-offs.

## Mathematical preparation and derivation

Derive output dimensions and parameter counts for a convolutional layer. Derive the gradient through a residual block and discuss its limitations.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Compare a compact plain CNN and a residual CNN on the same image split. Match parameter counts approximately and disclose remaining differences. Ablate normalization or skip connections and report accuracy, runtime, and learning curves.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Does a deeper model improve because of capacity, optimization, or a larger training budget?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_convolutional-neural-networks/index.html), sections 7.1–7.6; 8.5–8.6. Other architectures in chapter 8 are optional comparisons. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
