---
title: "Model-based reinforcement learning for combinatorial optimization"
collection: teaching
type: "Summer school class"
permalink: /teaching/summer-school/
venue: "CEA-EDF-Inria Summer School on numerical analysis"
date: "2026-06-25"
location: "Le Bourget-du-Lac, France"
---

[Link to the summer school website](https://ecoles-cea-edf-inria.fr/en/schools/ecole-analyse-numerique-de-2026/).

**Abstract**

Modern mixed-integer linear programming (MILP) solvers are built upon the branch-and-bound (B&B) paradigm. Since the 1980s, considerable research and engineering effort has gone into refining these solvers, resulting in highly optimized systems driven by expert-designed heuristics tuned over large benchmarks. However, in operational settings where structurally similarproblems are solved repeatedly, adapting solver heuristics to the distribution of encountered MILPs can lead to substantial gains in efficiency, beyond what static, hand-crafted heuristics can offer. Recent research has thus turned to machine learning (ML) to design efficient, data-driven B&B heuristics tailored to specific instance distributions. Here, we propose adapting recent reinforcement learning (RL) approaches, known for having achieved breakthroughs in complex combinatorial games such as chess or go, to the setting of exact combinatorial optimization. Drawing on the MuZero architecture, we introduce Plan-and-Branch-and-Bound (PlanB&B), a model-based reinforcement learning (MBRL) agent that leverages an internal model of the B&B dynamics to learn improved variable selection strategies.