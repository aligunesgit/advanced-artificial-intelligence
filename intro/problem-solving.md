# 3. Search, Reasoning, and Planning

## The idea

Some problems have clear rules and possible actions. We can solve them by exploring choices, checking conditions, and building a sequence of steps.

## Search: finding a route

Suppose a robot can take these directed routes. Numbers are travel costs.

```text
S --1--> A --8--> G
S --2--> B --2--> C --2--> G
```

A **state** is the robot's current location. An **action** follows an outgoing route. S is the start and G is the goal.

- **Breadth-first search (BFS)** explores by number of steps. It finds S–A–G with two steps, but cost 9.
- **Depth-first search (DFS)** follows one branch before trying another. Its result depends on exploration order; it does not guarantee the cheapest route.
- **Uniform-cost search** explores the lowest accumulated cost first. With nonnegative costs, it finds S–B–C–G with cost 6.
- **A\*** adds an estimate of remaining cost to the cost already paid. With an admissible estimate and correct handling of repeated states, it can find an optimal route. A zero estimate gives uniform-cost search.

Fewer steps and lower cost are different objectives.

## Local search: improving a candidate

For a repair schedule, start with a complete assignment and try small changes, such as swapping two jobs. **Hill climbing** keeps improvements but can get stuck at a solution that is only locally good. **Simulated annealing** sometimes accepts worse changes to explore further.

## Constraints: checking what is allowed

Two repairs need the same technician. Each takes one hour, so they cannot start together. A **constraint satisfaction problem** specifies variables, allowed values, and restrictions. Here the variables are start times and the restriction prevents overlap.

**Backtracking** tries an assignment and undoes it when a restriction is violated. Finding an allowed schedule and finding the cheapest schedule are separate questions.

## Reasoning and planning

**Knowledge representation** stores facts and rules in a usable form. For example: “Repair A requires the power to be off.” From “the power is on,” a reasoning system concludes that repair A cannot start yet.

**Planning** finds an action sequence: stop the machine, isolate power, repair, inspect, restart. Each action has conditions that must hold and effects that change the state.

In a competitive game, an action also depends on an opponent's response. **Minimax** chooses a move by considering the opponent's best reply; alpha–beta pruning avoids exploring branches that cannot affect the result.

## Try it

1. In the route example, which path uses fewer edges? Which costs less?
2. Add a direct edge S–G with cost 20. What does BFS now prefer?
3. Write two constraints for a university exam timetable.

**Previous: [AI approaches](approaches.md) · Next: [Learning from data →](learning-from-data.md)**
