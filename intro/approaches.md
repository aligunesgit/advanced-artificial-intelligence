# 2. AI Approaches and Key Concepts

## The idea

Choose a method based on the problem. A written rule, a search algorithm, and a learned model solve problems in different ways.

## One example: maintaining a machine

| Method | How it works | Example |
|---|---|---|
| Rules | Apply conditions written by a person | Request inspection if temperature exceeds a limit |
| Search | Explore possible choices | Find a repair schedule that fits available staff |
| Probability | Represent uncertainty | Estimate failure risk given a sensor reading |
| Machine learning | Learn relationships from examples | Predict failure from historical sensor records |

These methods can work together. A learned model estimates risk, a rule identifies urgent cases, and a search procedure assigns inspection times.

## Three ways to learn

**Supervised learning:** examples include a target answer. Given measurements and known failures, learn to predict failure. Predicting a category is **classification**; predicting a number is **regression**.

**Unsupervised learning:** examples have no target answer. Group machines with similar operating patterns. The groups are not automatically meaningful fault categories.

**Reinforcement learning:** an agent tries actions and receives rewards. A robot can learn a movement policy through repeated interaction. A reward must reflect the intended behavior.

## Where deep learning fits

A neural network transforms inputs through layers to produce an output. Training changes its numerical parameters to reduce an error measure called the **loss**. Deep networks are useful for many image, language, and audio tasks, but need suitable data and evaluation.

**Training** updates parameters. **Inference** uses the trained model to produce an output. A deployed model does not necessarily keep learning.

## Check your understanding

1. Is predicting tomorrow's demand classification or regression?
2. How does clustering maintenance records differ from predicting known failure labels?
3. Which methods could help schedule repairs after a model predicts failure?

**Previous: [What is AI?](what-is-ai.md) · Next: [Search, reasoning, and planning →](problem-solving.md)**
