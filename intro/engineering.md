# 5. AI Across Engineering

## The idea

Start with a problem that someone needs to solve. Define the inputs, the expected output, and how success will be measured before choosing a model.

## Examples from different fields

| Field | Task | Input | Output |
|---|---|---|---|
| Mechanical | Predict a machine failure | Sensor measurements | Failure risk for the next day |
| Electrical | Forecast electricity demand | Past demand and weather forecast | Next-day demand |
| Civil | Find surface damage | Inspection photographs | Damage locations |
| Industrial | Detect defective products | Production images | Defective or acceptable |
| Computer | Identify suspicious traffic | Network records | An alert score |
| Materials | Estimate a material property | Composition and process settings | A predicted property value |

These are possible tasks. A simple rule or an established engineering model may already solve the problem well.

## Worked example: machine maintenance

“Use AI for maintenance” is too broad. A clearer task is: **use the previous hour's measurements to predict whether a machine will fail within the next day.**

We need measurements collected before the prediction and reliable failure records. Begin with a temperature-threshold rule as a **baseline**: a simple reference method that a new model should improve on.

If the model will be used on unfamiliar machines, test it on machines excluded from training. If it will predict future failures in the current fleet, use a later time period for testing.

Measure both missed failures and unnecessary inspections. If only one day in a hundred contains a failure, always predicting “no failure” gives 99% accuracy but misses every failure.

## A six-question worksheet

1. Who will use the result, and what will they do with it?
2. What information is available when the prediction is needed?
3. What exactly is the output, and how will we obtain the correct answer?
4. Which simple method will serve as the baseline?
5. Which unseen cases represent the intended use?
6. Which errors are most costly?

## Try it

Choose one task from the table and answer the six questions in plain language. Ask a classmate to identify one missing input or an unclear target. You should be able to explain the task without naming a neural network architecture.

**Previous: [Learning from data](learning-from-data.md) · Next: [Modern AI systems →](current-developments.md)**
