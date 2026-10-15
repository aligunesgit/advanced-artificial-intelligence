# Module 5: Sequence Models and Recurrent Networks

Week 5 · Graduate seminar and research lab

## Learning objectives

Derive backpropagation through time; compare recurrent gates; evaluate sequence models without temporal leakage.

## Core concepts

Autoregressive modeling, perplexity, RNNs, gradient clipping, LSTM, GRU, and encoder–decoder models.

## Mathematical preparation and derivation

Express the recurrent gradient as a product of Jacobians and explain vanishing and exploding gradients. Show why a bidirectional model cannot be used unchanged for causal next-token prediction.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Compare a compact RNN and GRU on a public-domain text corpus with a contiguous held-out segment. Fix vocabulary and context construction using training data. Measure held-out perplexity and runtime and ablate gradient clipping.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Does lower perplexity imply useful long-range dependence?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_recurrent-neural-networks/index.html), sections 9.1–9.7; 10.1–10.2 and 10.6–10.7. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
