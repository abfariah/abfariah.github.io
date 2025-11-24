---
title: "A Markov decision process for variable selection in Branch & Bound"
collection: publications
permalink: /publication/bbmdp
excerpt: 'In this work, we introduce BBMDP, a principled vanilla MDP formulation for variable selection in B&B, allowing to leverage a broad range of RL algorithms for the purpose of learning optimal B&B heuristics.'
date: 2025-01-01
venue: 'Neural Information Processing Systems (NeurIPS)'
paperurl: # 'http://academicpages.github.io/files/paper2.pdf'
citation: 'Strang, P., Ales, Z., Bissuel, C., Juan, O., Kedad-Sidhoum, S., Rachelson, E., 2025. A Markov Decision Process for Variable Selection in Branch & Bound. Presented at the <i>The Thirty-ninth Annual Conference on Neural Information Processing Systems</i>.'
---
Mixed-Integer Linear Programming (MILP) is a powerful framework used to address a wide range of NP-hard combinatorial optimization problems, often solved by Branch and bound (B&B). A key factor influencing the performance of B&B solvers is the variable selection heuristic governing branching decisions. Recent contributions have sought to adapt reinforcement learning (RL) algorithms to the B&B setting to learn optimal branching policies, through Markov Decision Processes (MDP) inspired formulations, and ad hoc convergence theorems and algorithms. In this work, we introduce BBMDP, a principled vanilla MDP formulation for variable selection in B&B, allowing to leverage a broad range of RL algorithms for the purpose of learning optimal B&B heuristics. Computational experiments validate our model empirically, as our branching agent outperforms prior state-of-the-art RL agents on four standard MILP benchmarks.

[Download paper here](https://arxiv.org/abs/2510.19348)
