---
title: "Planning in Branch-and-Bound: Model-based Reinforcement Learning for Exact Combinatorial Optimization"
collection: publications
permalink: /publication/planbb
excerpt: "We introduce PlanB&B, a model-based reinforcement learning agent that learns an internal model of Branch & Bound dynamics to derive improved branching strategies for variable selection in B&B."
date: 2026-01-01
venue: AAAI
paperurl: https://arxiv.org/abs/2511.09219
citation: 'Strang, P., Alès, Z., Bissuel, C., Juan, O., Kedad-Sidhoum, S., Rachelson, E., (2026). Planning in Branch-and-Bound: Model-based Reinforcement Learning for Exact Combinatorial Optimization. <i>AAAI</i>.'
---
 Mixed-Integer Linear Programming (MILP) lies at the core of many real-world combinatorial optimization (CO) problems, traditionally solved by branch-and-bound (B&B). 
A key driver influencing B&B solvers efficiency is the variable selection heuristic that guides branching decisions. 
Looking to move beyond static, hand-crafted heuristics, recent work has explored adapting traditional reinforcement learning (RL) algorithms to the B&B setting, aiming to learn branching strategies tailored to specific MILP distributions. 
In parallel, RL agents have achieved remarkable success in board games, a very specific type of combinatorial problems, by leveraging environment simulators to plan via Monte Carlo Tree Search (MCTS).
Building on these developments, we introduce Plan-and-Branch-and-Bound (PlanB&B), a model-based reinforcement learning (MBRL) agent that leverages a learned internal model of the B&B dynamics to discover improved branching strategies. 
Computational experiments empirically validate our approach, with our MBRL branching agent outperforming previous state-of-the-art RL methods across four standard MILP benchmarks. 

[Download paper here](https://arxiv.org/abs/2511.09219)