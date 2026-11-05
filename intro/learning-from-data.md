# 4. Learning from Data

## The idea

A model learns a relationship from examples. To know whether that relationship is useful, test it on examples that were not used to build or select the model.

## Example: predicting electricity demand

Each row describes one day. Inputs might include the day of the week, forecast temperature, and previous demand. The target is the next day's demand.

A **feature** is an input variable. A **label** or **target** is the answer used for supervised training. Only include information available when the prediction will be made.

## A simple workflow

1. **Define the task.** Predict next-day demand for one building.
2. **Inspect the data.** Check missing readings, duplicate rows, units, and unusual values.
3. **Split the data.** Use earlier periods for training, a later period for validation, and the latest period for testing.
4. **Prepare inputs.** Learn replacements for missing values and scaling settings from training data only. Apply those settings to the other splits.
5. **Build a baseline.** Predict the same demand as the previous day.
6. **Train and select.** Fit a model on training data; use validation data to choose settings.
7. **Evaluate once.** Report final performance on the test period and compare with the baseline.

For time-dependent records, a random split can put future information into training. For repeated measurements from machines or people, consider holding out entire machines or people.

## Start with a small model

| Task | Simple starting model | Example measure |
|---|---|---|
| Predict a number | Linear regression | Mean absolute error |
| Predict a category | Logistic regression or decision tree | Precision and recall |
| Find similar groups | K-means | Inspect cluster structure and usefulness |

K-means needs a chosen number of clusters and is sensitive to feature scale. A cluster is a pattern to investigate, not proof of a real-world category.

For a classifier, **precision** asks how many predicted positives are correct; **recall** asks how many actual positives are found. Choose measures that reflect the consequences of errors.

## Two common mistakes

**Overfitting:** the model performs well on training examples but poorly on new ones. Compare training and validation performance; consider a simpler model, regularization, or better data.

**Data leakage:** training or model selection uses information that would be unavailable in real use. Examples include scaling with the entire dataset or repeatedly tuning against the test set.

## Python preparation

Before the technical modules, practise lists, loops, functions, NumPy arrays, and pandas tables. You should be able to load a small table, inspect missing values, and explain each column. See the [preparation checklist](../pages/before.md).

## Try it

A building uses about 100 units of electricity each day. Your model's average absolute error is 12 units; predicting yesterday's demand gives 8. Which method should be your current reference, and what would you investigate next?

**Previous: [Search and reasoning](problem-solving.md) · Next: [AI in engineering →](engineering.md)**
