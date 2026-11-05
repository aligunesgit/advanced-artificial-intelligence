# Module 5: Sequence Models and Recurrent Networks

Week 5 · Graduate seminar and research lab

## Start with the idea: Learning from ordered data

In a sequence, order matters. A recurrent neural network (RNN) processes items in order and updates a hidden state that carries information from earlier items. GRU and LSTM models use gates to control this information.

## A concrete example

A next-character model reads “engin” and predicts what might follow. During prediction it must use only the available prefix. Future characters belong to the answer, not the input.

## Quick check

Why would using future tokens make a next-token evaluation misleading?

The sections below develop the mathematics and the practice experiment. For every experiment, record the data split, baseline, settings, result, and one limitation.

## Learning objectives

Derive backpropagation through time; compare recurrent gates; evaluate sequence models without temporal leakage.

## Core concepts

Autoregressive modeling, perplexity, RNNs, gradient clipping, LSTM, GRU, and encoder–decoder models.

## Mathematical preparation and derivation

Express the recurrent gradient as a product of Jacobians and explain vanishing and exploding gradients. Show why a bidirectional model cannot be used unchanged for causal next-token prediction.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Compare a compact RNN and GRU on a public-domain text corpus with a contiguous held-out segment. Fix vocabulary and context construction using training data. Measure held-out perplexity and runtime and ablate gradient clipping.

Prepare runnable code, environment details, one results table or figure, and a 500–800 word explanation. State what the result shows and one limitation. Use a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

Does lower perplexity imply useful long-range dependence?

Bring one claim, supporting evidence, and one alternative explanation. An **ablation** changes or removes one component to test its contribution.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_recurrent-neural-networks/index.html), sections 9.1–9.7; 10.1–10.2 and 10.6–10.7. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
