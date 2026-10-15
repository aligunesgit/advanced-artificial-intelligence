# 3. AI Across Engineering

The starting point for an AI project is a decision or scientific question. The choice of model follows from the data, objective, constraints, and evidence needed to support that question.

## Different disciplines, shared questions

The examples below are possible project directions, not claims that AI is always the best solution.

| Discipline | Possible task | Observations | Important evaluation concern |
|---|---|---|---|
| Mechanical engineering | Predict machine failure | Sensor time series and operating conditions | Hold out machines or future periods, not overlapping windows alone |
| Electrical engineering | Forecast electricity demand | Historical demand, weather, calendar variables | Use only information available at forecast time |
| Civil engineering | Detect surface damage | Images and inspection records | Check transfer to new structures and imaging conditions |
| Industrial engineering | Detect defects or forecast demand | Production images or operational records | Compare errors using operational costs and class balance |
| Computer engineering | Classify network events | Traffic or event logs | Account for changing attacks, duplicates, and future information |
| Chemical or materials engineering | Predict a property or prioritize experiments | Composition, process settings, measurements | Test unfamiliar compositions and quantify uncertainty |

Domain knowledge helps define realistic targets and recognize meaningless shortcuts. For example, a fault model might identify a machine from its sensor signature instead of learning a fault mechanism. A random observation-level split could hide this problem.

## A problem formulation worksheet

Before selecting an architecture, answer these questions in plain language:

1. **Decision:** who uses the result, and what action does it support?
2. **Input:** what information is actually available at that moment?
3. **Target:** what outcome are we predicting, and how is it measured?
4. **Baseline:** what simple rule, statistical method, or current practice should we compare against?
5. **Evidence:** what held-out cases resemble the intended use?
6. **Costs:** which errors matter, and what are the runtime or resource constraints?

A broad interest such as “AI for maintenance” becomes a testable question when the prediction horizon, machines, measurements, baseline, and evaluation protocol are specified.

## Worked example: maintenance

Suppose the question is whether measurements from the previous hour help identify failures within the next day. Inputs must precede the prediction time. Labels need reliable failure records. A temperature threshold or a linear model provides a baseline. If we want the system to work on new machines, we should evaluate on held-out machines. If we want future performance on a known fleet, we need a time-aware evaluation.

Report missed failures and unnecessary inspections, not accuracy alone. A rare failure class can make a model look accurate even when it misses the cases that matter. A risk estimate also needs a decision rule reflecting inspection capacity and error costs.

## When another approach may fit better

Known physical relationships, explicit constraints, limited data, and strict latency can favor established models or a combination of methods. A simulator, a mathematical optimizer, a rule-based check, and a learned estimator can contribute to one solution. Compare them against the actual engineering objective.

## Classroom activity

In pairs from different departments, complete the worksheet for one problem. Your partner should challenge the target definition and ask, “What observation would show that your proposed approach has failed?” Keep the question for later project planning; this is ungraded practice.

**Previous: [AI Approaches](approaches.md) · Next: [Current Developments in AI →](current-developments.md)**
