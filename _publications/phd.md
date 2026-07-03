---
title: "Learning to solve repeated combinatorial optimization problems exactly"
collection: publications
permalink: /publication/phd
excerpt: 'PhD dissertation'
date: 2026-05-28
venue: 'Ecole doctorale des sciences des métiers et de l''ingénieur'
paperurl: #
citation: 'Strang, P. (2026). Learning to solve repeated combinatorial optimization problems exactly (Doctoral dissertation, HESAM Université).'
---

**Keywords**

<ul class="keyword-list">
  <li>Repeated combinatorial optimization problems</li>
  <li>Mixed-integer linear programming</li>
  <li>Branch-and-bound</li>
  <li>Branching heuristics</li>
  <li>Graph neural networks</li>
  <li>Reinforcement learning</li>
  <li>Model-based reinforcement learning</li>
  <li>Interior-point methods</li>
  <li>Flow matching</li>
</ul>

**Abstract**

Mixed-integer linear programming (MILP) plays a central role in combinatorial optimization (CO), a discipline concerned with finding optimal solutions over typically large but finite sets. Specifically, MILPs offer a general modelling framework for NP-hard problems, and have become indispensable in tackling complex decision-making tasks across fields as diverse as operations research, quantitative finance, and computational biology. Modern MILP solvers are built upon the branch-and-bound (B&B) paradigm, which systematically explores the solution space by recursively partitioning the original problem into smaller subproblems, while maintaining provable optimality guarantees. Since the 1980s, considerable research and engineering effort have gone into refining these solvers, resulting in highly optimized systems driven by expert-designed heuristics tuned over large benchmarks. 

Nevertheless, in operational settings where structurally similar problems are solved repeatedly, adapting solver heuristics to the distribution of encountered MILPs can lead to substantial gains in efficiency, beyond what static, hand-crafted heuristics can offer. Recent research has thus turned to machine learning to design efficient, data-driven B&B heuristics tailored to specific instance distributions. The variable selection heuristic, or branching heuristic, plays a particularly critical role in B&B computational efficiency, as it governs the selection of variables along which the search space is recursively split. A key milestone was achieved by Gasse et al. (2019), who showed that learning to replicate the decisions of a greedy branching expert via imitation learning (IL) could outperform expert-designed branching heuristics. While subsequent works succeeded in learning effective branching strategies by reinforcement, none have yet matched the performance achieved by IL approaches. This trend extends beyond MILPs, as reinforcement learning (RL) baselines consistently underperform both handcrafted heuristics and IL methods across various combinatorial optimization benchmarks. 

Yet, if the performance of IL heuristics is capped by that of the experts they learn from, the performance of RL agents is, in theory, only bounded by the maximum score achievable. To cope with the credit assignment difficulties induced by sparse rewards, prior works have shifted away from the standard Markov decision process (MDP) framework, finding it impractical for learning efficient branching strategies. In this thesis, we show that these alternative formulations, despite improving the empirical performance of RL baselines, introduce approximations of the B&B dynamics that compromise the asymptotic guarantees of generic RL algorithms. To address this issue, we propose reverting to a principled MDP formulation of the branch-and-bound process, which preserves the convergence properties established by previous contributions without sacrificing optimality. Unlike prior formulations, our framework accommodates the full spectrum of modern RL algorithms, including planning-based approaches that leverage look-ahead search for robust policy improvement.

Inspired by the success of AlphaZero in complex combinatorial board games, we explore extending the applicability of planning-based RL from board games to exact combinatorial optimization. To that end, we introduce PlanB&B, a model-based reinforcement learning agent that leverages a learned internal model of the B&B dynamics to discover improved variable selection strategies. Our computational results across both synthetic and real-world industrial benchmarks indicate that the branching dynamics in B&B can be approximated with sufficient fidelity in latent space to enable policy improvement through planning over a learned model, opening the door to broader applications of model-based reinforcement learning to mixed-integer linear programming in the future.


[Access the manuscript](/files/manuscript.pdf)

**Jury**
- Dr. Riad Akrour, Inria, France (reviewer)
- Prof. Thibaut Vidal, Polytechnique Montréal, Canada (reviewer)
- Prof. Sourour Elloumi, ENSTA IP Paris, France (president)
- Dr. Mathieu Besançon, Inria, France (examiner)
- Prof. Axel Parmentier, ENPC, France (examiner)
- Prof. Safia Kedad-Sidhoum, Cnam, France (supervisor)
- Prof. Emmanuel Rachelson, ISAE-Supaero, France (co-supervisor)
- Prof. Zacharie Alès, ENSTA IP Paris, France (advisor)