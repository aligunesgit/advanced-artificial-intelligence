# Module 9: Sequential Decision Making and Reinforcement Learning

Week 10 · Graduate seminar and research lab

## Learning objectives

Derive Bellman equations; compare planning and learning; evaluate exploration across seeds.

## Core concepts

Finite MDPs, value iteration, Q-learning, exploration, reward specification, and policy evaluation.

## Mathematical preparation and derivation

Derive the Bellman optimality equation and contraction for a finite discounted MDP. State conditions for tabular Q-learning convergence and distinguish them from a finite-run guarantee.

Prepare a written derivation before the seminar. State assumptions and dimensions, and identify one case in which the conclusion fails.

## Practice lab (ungraded)

Implement value iteration and Q-learning on the same small finite MDP. Compare returns against an optimal reference across at least five seeds. Separate exploration during training from policy evaluation and ablate an exploration schedule.

For practice and feedback, prepare code, an environment specification, a reproducible run command, a results table or figure, and a 500–800 word analysis. Explain limitations and distinguish observations from proposed explanations. Work within a declared compute budget; a CPU-scale experiment is sufficient.

## Seminar discussion

How can a reward-maximizing policy fail to satisfy the intended task?

Bring one claim, the evidence supporting it, and one alternative explanation. For paper sessions, identify a missing ablation or an assumption that limits the result.

## Reading

[Dive into Deep Learning](https://d2l.ai/chapter_reinforcement-learning/index.html), sections 17.1–17.3. Use the PyTorch implementation where available. These selections are assigned reading, not a requirement to reproduce every book experiment.

## Completion criteria

- Derivation is correct and assumptions are explicit.
- Experiment includes a suitable baseline and a fair comparison.
- Results can be reproduced from the submitted instructions.
- Conclusions follow from measured evidence, including negative results.

Lab instructions and submission layout: [exercise files](exercise_files/README.md).
