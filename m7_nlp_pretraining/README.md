# Module 7: Representation Pretraining and NLP Adaptation

Week 8 · Graduate seminar and research lab

## Learning objectives

Compare embedding and contextual pretraining objectives; distinguish pretraining from fine-tuning; evaluate transfer.

## Core concepts

Word embeddings, negative sampling, subword representations, BERT objectives, sentiment analysis, and natural language inference.

## Mathematical preparation and derivation

Derive the skip-gram negative-sampling objective. Explain how masked-token prediction differs from causal next-token likelihood and why their losses are not directly comparable.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Compare a TF-IDF linear baseline with a compact pretrained-embedding classifier on sentiment data. Keep preprocessing and tuning leakage-free. Optional extension: fine-tune a small contextual encoder and report pretraining source, resource use, and test contamination risks.

For practice and feedback, prepare code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

How can one separate gains from pretraining data, architecture, and downstream tuning?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_natural-language-processing-pretraining/index.html), sections 15.1–15.4, 15.6, 15.8; 16.1–16.2. Sections 16.6–16.7 are an optional extension. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
