# 1. What Is Artificial Intelligence?

## The idea

Artificial intelligence (AI) studies how computers can perform tasks such as recognizing objects, finding solutions, learning from examples, and choosing actions.

Consider a robot delivering a package. It needs to detect a wall, find a route around it, and move toward its destination. Recognizing the wall and choosing a route are different tasks. They may use different AI methods.

## Describe a system in four parts

| Part | Delivery robot | Spam filter |
|---|---|---|
| Input | Camera image and position | Email text |
| Task | Deliver a package | Identify unwanted messages |
| Output | Next movement | Spam or normal |
| Success measure | Delivery time and collisions | Missed spam and incorrectly blocked messages |

An **agent** observes its surroundings and chooses actions. The robot is an agent; its surroundings are its **environment**. A prediction model can be one component inside an agent.

## AI, machine learning, and deep learning

- **AI** is the broad field. Finding a route with a search algorithm belongs here.
- **Machine learning (ML)** is part of AI. A model learns patterns from examples, such as emails labeled spam or normal.
- **Deep learning (DL)** is part of ML. It uses neural networks with multiple layers to learn representations of data.

The relationship is: **AI contains ML; ML contains DL.** An AI system does not always need a neural network.

## Narrow and general capability

A spam filter solves a specific task. This is an example of narrow AI. General AI refers to broader ability across tasks; the term has varying definitions. In this course, we describe what a system can do using specific tasks and measurements.

A model can produce a fluent answer and still give incorrect information. Judge the result against the task, using evidence.

## Check your understanding

1. What are the input and output of a system that detects cracks in concrete?
2. Could a route-finding program work without learning from data?
3. Why is accuracy alone insufficient for a delivery robot?

**Next: [AI approaches →](approaches.md)**
