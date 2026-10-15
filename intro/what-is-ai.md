# 1. What Is Artificial Intelligence?

## From an engineering problem to intelligent behavior

Imagine a robot navigating a warehouse. It must estimate where it is, recognize obstacles, select a route, and adapt if an aisle is blocked. These are connected but distinct problems: perception, state estimation, planning, and decision making. Learning from experience may help several of them, but learning is not the only possible mechanism.

For this course, we use AI as an umbrella for computational approaches to perception, reasoning, learning, communication, planning, and action. We study the methods and the evidence that a system performs the intended task. This perspective connects with the agent-centered treatment in [Russell and Norvig’s Artificial Intelligence: A Modern Approach](https://aima.cs.berkeley.edu/).

## The agent–environment view

An **agent** receives observations from an environment and selects actions. Its behavior is assessed against an objective under constraints.

| Element | Warehouse robot example | Predictive maintenance example |
|---|---|---|
| Environment | A warehouse with people and shelves | Machines operating under changing loads |
| Observations | Camera images, range measurements | Vibration, temperature, current |
| Action or output | Movement or a route | A risk estimate or inspection recommendation |
| Objective | Deliver items reliably | Reduce failures and unnecessary inspections |
| Constraints | Collision avoidance, battery, time | Staff, downtime, sensor availability |

An objective needs careful definition. Maximizing the number of deliveries without accounting for collisions would describe an incomplete engineering goal. Similarly, maximizing classification accuracy may ignore costly missed faults.

## Core capabilities

- **Perception:** extract useful information from observations, such as detecting cracks in an image.
- **Reasoning:** derive conclusions from information and assumptions, such as checking whether constraints can be satisfied.
- **Planning:** choose a sequence of actions, such as scheduling repairs.
- **Learning:** adjust a model or policy using experience or data.
- **Language:** interpret or generate text and other linguistic signals.
- **Decision making under uncertainty:** choose an action when information or outcomes are uncertain.

A working system may combine several capabilities. Strong performance on one benchmark does not establish competence across all of them. Humanlike language alone does not demonstrate reliable planning or physical understanding.

## Task-specific systems and general intelligence

A system can perform a narrow task extremely well without being generally capable. “Artificial general intelligence” refers to broader capability across tasks, but definitions and proposed tests differ. We will make specific, measurable claims about systems rather than infer general intelligence from a single demonstration.

Also distinguish automation from adaptation. A fixed rule can automate a useful task; it need not learn. A learned model can adapt through training, but it still operates under assumptions and may fail when conditions change.

## Classroom discussion

Choose an AI application from your department. Identify its observations, outputs or actions, objective, and constraints. Which capabilities does it need? Which part could be solved with a simple rule or established engineering method?

**Next: [AI Approaches and Key Concepts →](approaches.md)**
