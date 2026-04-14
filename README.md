# Traceline — Modeling AI Behavior in Constrained Environments

## Motivation

Modern AI systems are often trained on large-scale human data, which may contain implicit behavioral patterns such as conformity, bias, or limited exploration.

This project explores a simplified version of this question:

> If agents follow different behavioral assumptions — majority-driven, goal-driven, or exploratory — how does their behavior differ?

The goal is not to replicate real AI systems, but to study how **design choices influence behavior**.

---

## Experiment Overview

Agents are placed in a grid-based maze environment and evaluated based on their movement and decision patterns.

### Agents

- **Human-like**  
  Goal-oriented with limited repetition

- **Conditioned**  
  Follows a predefined majority path (social conformity)

- **Exploratory**  
  Prioritizes novelty while maintaining a soft goal bias

---

## Metrics

- Goal achievement  
- Novelty score  
- Repetition count  
- Distance to goal  

---

## Key Observations

- The conditioned agent exhibits high repetition and often fails to reach the goal  
- The exploratory agent achieves higher novelty and successfully reaches the goal  
- The human-like agent reaches the goal with moderate repetition  

---

## Insight

Behavior is strongly influenced by **decision rules (design)**, not just the environment.

This suggests that systems trained on majority-driven patterns may exhibit limited exploration, while alternative design choices can lead to more effective behavior.

---

## Structure

- `traceline_experiment.ipynb` — main experimental notebook with results and observations  

---

## Status

Initial experimental prototype. Further extensions and validation planned.