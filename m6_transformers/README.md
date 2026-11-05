# Module 6: Attention and Transformer Architectures

Week 7 · Graduate seminar and research lab

## Start with the idea: Connecting relevant parts of a sequence

Attention forms a weighted combination of representations. Queries describe what a position is looking for; keys help determine relevance; values provide the information being combined. A Transformer builds on attention and other layers.

## A concrete example

In “The motor stopped because it overheated,” attention can connect positions across the sentence. Positional information represents order. A causal mask prevents a next-token model from using future positions.

## Quick check

What should happen to an earlier prediction if only a future token changes?

The sections below develop the mathematics and the practice experiment. For every experiment, record the data split, baseline, settings, result, and one limitation.

## Learning objectives

Derive attention; implement causal masking; compare recurrence and self-attention.

## Core concepts

Queries, keys, values, multi-head attention, positional encoding, encoder–decoder structure, and computational cost.

## Mathematical preparation and derivation

Derive tensor shapes in softmax(QK^T / sqrt(d_k))V and explain the scale factor. Compare attention score memory with recurrent computation as sequence length increases.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Implement a tiny causal Transformer for the M5 corpus. Verify that changing a future token cannot change earlier logits. Compare with the recurrent baseline under a declared parameter and compute budget; ablate positional information.

Prepare runnable code, environment details, one results table or figure, and a 500–800 word explanation. State what the result shows and one limitation. Use a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

What can an attention visualization establish about model reasoning?

Bring one claim, supporting evidence, and one alternative explanation. An **ablation** changes or removes one component to test its contribution.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_attention-mechanisms-and-transformers/index.html), sections 11.1–11.7 required; 11.8–11.9 optional. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
