# 2. AI Approaches and Key Concepts

AI methods are easier to understand when we separate how knowledge is represented, how a solution is found, and how a system is evaluated. The categories below overlap; they are tools to combine rather than competing labels for every system.

## Rules, search, probability, and learning

| Approach | Central idea | Engineering example | Key question |
|---|---|---|---|
| Rule-based and symbolic methods | Represent explicit facts, rules, or constraints | Check whether a design satisfies specified logical conditions | Are the rules complete and consistent? |
| Search and planning | Explore possible states or action sequences | Find a route or maintenance schedule | How large is the search space, and what constraints apply? |
| Probabilistic methods | Represent and update uncertainty | Infer a possible fault from noisy observations | What assumptions connect the variables? |
| Machine learning | Fit a model using examples or experience | Predict demand or classify defects | Does the learned relationship generalize? |
| Hybrid systems | Combine learned components with other methods | Use a learned detector inside a constrained planning pipeline | How do component errors affect the complete system? |

For example, recognizing a part in a camera image may use a neural network, while selecting a safe grasp can also involve geometric constraints and a controller. Calling the complete robot “AI” does not imply every component uses the same method.

## AI, machine learning, and deep learning

**AI** is the broader field. **Machine learning** is a family of approaches that use data or experience to fit models or policies. **Deep learning** uses neural networks with multiple representation stages. **Generative AI** describes systems that generate content or samples; it is a capability category, not a synonym for all AI.

A **large language model** models token sequences, commonly using a Transformer. A **Transformer** is an architecture, not the definition of AI. A **foundation model** is pretrained broadly and can be adapted to multiple downstream tasks. An **agentic system** combines a model with observations, tools, state, and an action loop; the surrounding system matters as much as an isolated answer.

## Ways to learn

- **Supervised learning:** use labeled examples to predict a target, such as a defect category.
- **Unsupervised learning:** examine structure without a task-specific target label, such as grouping operating regimes.
- **Self-supervised learning:** construct a learning signal from the data itself, such as predicting missing content.
- **Reinforcement learning:** learn behavior through actions, rewards, and interaction over time.

Self-supervision does not eliminate the need to evaluate a downstream task. Reinforcement learning is not simply supervised classification with a different name: actions can change future observations and outcomes.

## Four distinctions to keep clear

A **model** is a parameterized component; a **system** also includes data collection, interfaces, rules, tools, and monitoring. **Training** changes model parameters; **inference** uses a fitted model to produce outputs. A **prediction** estimates something; a **decision** also depends on goals and costs. **Fluent output** is an observable behavior; **correctness** requires evidence appropriate to the task.

## Classroom discussion

A system reads inspection reports, retrieves a maintenance manual, proposes a repair schedule, and checks resource constraints. Identify the components. Which might use learning, retrieval, search, or explicit rules? How would you test the system beyond checking whether the final paragraph reads well?

For the technical learning track, see [Dive into Deep Learning](https://d2l.ai/index.html). For the broader AI perspective, see [Artificial Intelligence: A Modern Approach](https://aima.cs.berkeley.edu/).

**Previous: [What Is AI?](what-is-ai.md) · Next: [AI Across Engineering →](engineering.md)**
