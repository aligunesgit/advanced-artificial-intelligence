# 6. Modern AI Systems

## The idea

An AI application often combines several components. Separate what each component does before deciding how to evaluate the whole system.

## Example: answering a maintenance question

A technician asks, “How should I inspect this pump?” A useful application might follow these steps:

1. **Retrieve** relevant passages from the correct pump manual.
2. **Generate** an explanation using a language model and those passages.
3. **Call a tool** to check available inspection times.
4. Ask the technician to review the proposed inspection.

Retrieval selects existing information. Generation produces an output. Tool use interacts with another system. Each step can fail independently.

## Generative AI

Generative models produce text, images, audio, or other outputs. A language model predicts tokens from context; tokens are pieces of text. A **prompt** supplies instructions and context to a model.

A GAN trains a generator alongside a discriminator. A diffusion model learns a denoising process. These are different approaches to generation; [M8](../m8_generative_models/README.md) studies GANs in detail.

## RAG and agents

**Retrieval-augmented generation (RAG)** supplies retrieved material as context for generation. It can help answer questions about a manual, but a relevant passage does not guarantee a correct answer. Check that the cited passage actually supports the answer.

An **agent** selects actions based on observations and a goal. A language-model agent may call a search tool, inspect the result, and choose another action. Define which actions it may take and how completion is checked.

## Language, images, and applications

**Natural language processing (NLP)** includes tasks such as text classification and translation. **Computer vision** includes image classification, object detection, and segmentation. A **multimodal** system uses more than one type of input or output, such as a photo and a written question.

For a pump photo, classification asks which kind of pump it is; detection locates pumps in the image; segmentation assigns a label to individual pixels.

## How to check the result

For the maintenance assistant, ask four concrete questions:

- Did retrieval find the manual for the correct model?
- Does the answer match the manual, including important conditions?
- Did the scheduling tool return a valid available time?
- Did the technician receive a clear proposal they can review?

A polished paragraph does not answer these questions. Measure the behavior needed by the application.

## Try it

Design an assistant for your department. Name its inputs, one information source, one possible tool, and one check that demonstrates success.

**Previous: [AI in engineering](engineering.md) · Next: [M1: Deep learning foundations →](../m1_foundations/README.md)**
