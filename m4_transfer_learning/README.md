# Module 4: Transfer Learning and Computer Vision

Week 4 · Graduate seminar and research lab

## Learning objectives

Design augmentation controls; distinguish frozen-feature and full fine-tuning protocols; analyze domain shift.

## Core concepts

Image augmentation, pretrained representations, fine-tuning, detection and segmentation task formulations.

## Mathematical preparation and derivation

For a frozen encoder followed by a linear classifier, derive the trainable parameter count and explain which gradients are suppressed. Contrast the classification objective with pixelwise segmentation.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Compare training a small model from scratch, frozen features, and limited fine-tuning on a small image dataset. Use identical splits and account for pretraining data provenance. A CPU-scale substitute may use an instructor-provided small checkpoint; report its origin.

For practice and feedback, prepare code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

When can transfer improve sample efficiency while introducing evaluation contamination?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_computer-vision/index.html), sections 14.1–14.2 required; 14.3 and 14.9–14.11 provide an optional task survey. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
