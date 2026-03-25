# Reading Note — Day 1
**Date:** March 2, 2025
**Sources:** Sutton & Barto Ch.1 | Géron Ch.1 | Stanford CS221

---

## The Five MDP Components

**State:** 
My definition: The situation or environment AI is looking at to make the decision.
My factory example: The current anomaly signal, where the severity, frequency, sensor location and time of the day etc. This shows that an anomaly exists. 

**Action:** 
My definition: The response to the state by AI.
My factory example: Trigger maintenance immediately or contiue monitoring, here action = 1 (act) or no action = 0 (wait)

**Reward:** 
My definition: the numerical signal environment gives to the agent after it takes the action.
My factory example: +2 for correct maintenance trigger, -1 for false alarm and 0 for waiting.

**Transition:** 
My definition: How the world changes after the aent takes an action.
My factory example: After triggering the maintenance, the equipment is repaired (if anomaly exists) or unchanged (false alarm). 
Either way a new anomaly arrives and the cycle continues.

**Policy:** 
My definition: the rule that maps state to actions. 
My factory example: In this simulation, naive policy = always act. Smart policy = act only if confidence > threshold

---

## Supervised Learning vs. Reinforcement Learning
Supervised learning, someone labels every example. "Teh animaly is real". " The anomaly is not real".
Reinforcement learning, no labels needed. The agent acts, receives a reward and then learns from that signal.

---

## The Multi-Armed Bandit
[2 sentences. What is it and how is your factory 
simulation specifically a bandit problem?]

---

## Where My Simulation Sits in the ML Taxonomy
[2 sentences. Reinforcement learning — why specifically?]

---

## One Thing I Want to Understand Better
[1-2 honest sentences]

---

## PMM Bridge — Day 1
[3 sentences positioning "AI that evaluates outcomes 
before acting" for a factory operations manager.
Value only. No jargon. No algorithms.]
```

Fill every field. Commit with message:
```
Add Day 1 reading note
