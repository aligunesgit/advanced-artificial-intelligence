# Module 6: Attention and Transformer Architectures

Week 7 · Graduate seminar and research lab

## Learning objectives

Derive attention; implement causal masking; compare recurrence and self-attention.

## Core concepts

Queries, keys, values, multi-head attention, positional encoding, encoder–decoder structure, and computational cost.

## Mathematical preparation and derivation

Derive tensor shapes in softmax(QK^T / sqrt(d_k))V and explain the scale factor. Compare attention score memory with recurrent computation as sequence length increases.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Required lab

Implement a tiny causal Transformer for the M5 corpus. Verify that changing a future token cannot change earlier logits. Compare with the recurrent baseline under a declared parameter and compute budget; ablate positional information.

Submit code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

What can an attention visualization establish about model reasoning?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_attention-mechanisms-and-transformers/index.html), sections 11.1–11.7 required; 11.8–11.9 optional. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
