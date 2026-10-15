# 4. Current Developments in AI

**Source review: 15 October 2026.** This page provides selected developments and discussion prompts, rather than a model ranking or an exhaustive news feed. Dates below refer to the cited announcements or publications. Revisit the sources as the field changes.

## From isolated predictions to multimodal systems

A growing area of AI combines information across modalities, such as images, language, audio, and video. The engineering question is how these observations are represented and connected to a useful output. A system that describes an image correctly can still fail at measurement, localization, or action selection.

A concrete example is the connection between visual observations, language instructions, and robot actions discussed in Google DeepMind’s [Gemini Robotics 2 announcement, 30 July 2026](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/). The authors describe whole-body control and manipulation, while reporting continuing difficulty with some dexterous tasks. This is a provider-reported development, not independent evidence of dependable operation in every environment.

**Engineering question:** what happens under unfamiliar lighting, objects, hardware, or physical disturbances? Later course connections: computer vision, representations, and sequential decision making.

## From answering questions to acting through tools

Agentic systems can combine a model with tool calls and repeated observation–action steps. Such systems may inspect files, run code, query information, or revise a plan. Success depends on the entire interaction, including tool behavior and the environment, rather than the text of a final answer alone.

Anthropic’s [Demystifying evals for AI agents, 9 January 2026](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents) discusses evaluating agents through tasks, trials, and grading approaches. It is a developer-authored methodology source, not a guarantee about a particular product.

**Engineering question:** did the system reach the correct final state, and how often does it succeed across repeated trials? Later course connections: reproducibility, experimental design, and project evaluation.

## AI as a tool for scientific investigation

AI is also being used to predict scientific quantities and prioritize investigation. Google DeepMind announced [AlphaGenome Atlas on 8 September 2026](https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/), a resource containing predicted molecular effects of single-nucleotide changes. This illustrates the use of learned models to organize a large scientific prediction space.

Predictions are not experimental confirmation or proof of causation. A useful scientific workflow asks which measurements validate a prediction and whether it transfers to the biological context of interest.

**Engineering question:** can a model help prioritize costly experiments while making its uncertainty and assumptions visible? Later course connections: representations, Gaussian processes, and evaluation.

## Reliability and evaluation are part of progress

New capabilities increase the importance of testing data quality, unsupported outputs, privacy, and behavior under changing conditions. NIST’s [Generative AI Profile, published 26 July 2024](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence) provides a cross-sector reference for generative-AI risk management. It is a framework for analysis, not a certification that a system is reliable.

For this course, translate broad concerns into measurable questions: how often are answers supported by evidence, which groups or operating regimes have higher error, and what changes when the data distribution shifts?

## How to read an AI announcement

For each development, separate the claimed capability, the test conditions, the source of the evidence, and the remaining limitation. A provider demonstration, a research paper, an independently reproduced experiment, and field performance supply different kinds of evidence.

Ask: compared with what baseline, on which tasks, at what cost, with how many trials, and under which assumptions? Avoid interpreting one benchmark improvement as universal intelligence or universal engineering readiness.

## Discussion and transition to the technical track

Choose one development above. State its contribution in one sentence, identify a limitation, and propose a small experiment that would test a narrower claim. No paid service or hardware purchase is required.

We now have a map of AI, examples from engineering, and questions for evaluating new systems. The next step is to understand one important family of methods in detail: learning from data. Begin [M1: Deep Learning Foundations and Research Practice](../m1_foundations/README.md), then follow the [D2L reading map](../pages/reading-map.md).

**Previous: [AI Across Engineering](engineering.md) · Next: [Course Guide](../pages/course-guide.md) or [M1 →](../m1_foundations/README.md)**
