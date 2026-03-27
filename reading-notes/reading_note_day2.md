# Reading Note — Day 2
**Date:** 27 March, 2026
**Sources:** Sutton & Barto Ch.2 | Géron Ch.4 | 
Counterfactual Explainability article

---

## Exploration vs. Exploitation

**The tradeoff in my own words:**
An agent that only exploits gets stuck on the first good action it finds and never discovers better ones. 
An agent that only explores never uses what it has learned and wastes every experience. The tension is finding the right balance between the two.

---

## Why Pure Greed Fails

**In my own words:**
Pure greed fails for that exact reason, where the agent chooses the best known action over and over again leading to 
poor long term performance. The reason is that the agent never discovers whether other actions might be better. 
It locks in on an early assumption and never tests it.

**Factory floor example:**
The robot always triggers maintenance as it was rewarded once and this doesn't allow it learn different possibilities of 
maintenance as there are different anomalies that could occur in a factory.

---

## Upper Confidence Bound (UCB)

**Why UCB is smarter than epsilon-greedy:**
Unlike epsilon-greedy which explores randomly, UCB targets its exploration towards actions it is most uncertain about, 
making every exploration step count rather than wasting it on actions already well understood.

---

## Loss Functions and Regret

**The connection in my own words:**
Regret measures the cumulative gap between the best possible reward and the actual reward received. 
Loss function measures the gap between a model's predictions and the correct answers. 
Minimising both means finding the policy or parameters that make the least costly mistakes over time.

---

## One Thing I Want to Understand Better
I want to understand the different alogorithms that are part of bandit problem in depth and the use cases for them.

---

## PMM Bridge — Day 2
Every day your AI systems make hundreds of decisions that affect operations, safety, and costs and under EU AI Act you are legally 
required to explain each one to regulators on request. This system logs the reasoning behind every decision automatically, 
showing exactly what conditions led to each action and what would have changed that decision. When a regulator asks why the robot halted 
production Tuesday at 14:32, you have a complete audit trail ready in seconds rather than scrambling through logs.
```
