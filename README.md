# Awesome Graph Neural Networks for Reinforcement Learning

...and other forms of relational decision learning.

<picture>
  <img
    src="https://upload.wikimedia.org/wikipedia/commons/2/22/Solaris_grapes_in_Chateaux_Luna_vineyard_24.jpg"
    alt="Green Solaris grapes and leaves growing in Chateaux Luna vineyard, Lysekil, Sweden"
    width="100%"
    height="200"
    style="object-fit: cover;"
  >
</picture>

## Intro

This is a list of links to code associated with papers that combine graph representation learning and various forms of decision learning, along with references to an extended family of relational and factored decision problems.

### Why graphs?

Many decision problems can be modeled as a set of entities that the agent
should make decision about. Depending on what is known about the entities,
the data can either be represented as a set, a graph or a hypergraph.
Unfortunately, most of the common RL libraries do not support
relational data structures, leading to some works representing the
entity-relational state as a flat vector.  However, such a data modeling
approach leads to brittle and impractical agents. This repository is intended
to provide examples and guidance to aspiring researchers aiming to use
decision learning in an entity oriented envrionment to help them
avoid these issues.

## Papers with Code

...and some code without papers

### MDPs/Reinforcement Learning

- [SR-DRL](https://github.com/jaromiru/sr-drl)
  - Code used for _Symbolic Relational Deep Reinforcement Learning based on Graph Neural Networks and Autoregressive Policy Decomposition_.
  - Tested with _Blockworld_, _Sokoban_ and _SysAdmin_.
- [ORACLE Sage](https://github.com/AndrewPaulChester/oracle-sage)
  - Code used for _Oracle-SAGE: planning ahead in graph-based deep reinforcement learning_.
  - Tested with _Minihack_ and _Taxi_.
- [Vejde](https://github.com/kasanari/vejde/)
  - Code used for _Vejde: A Framework for Inductive Deep Reinforcement Learning Based on Factor Graph Color Refinement_.
  - Tested with various [RDDLRepository](https://github.com/pyrddlgym-project/rddlrepository) problems.
- [Symnet 3](https://github.com/dair-iitd/symnet3)
  - Code for _SymNet 3.0: Exploiting Long-Range Influences in Learning Generalized Neural Policies for Relational MDPs_.
- [Symnet 2](https://github.com/dair-iitd/symnet2)
  - Code for _SymNet 2.0: Effectively handling Non-Fluents and Actions in Generalized Neural Policies for RDDL Relational MDPs_.
- [Symnet](https://github.com/dair-iitd/symnet)
  - Code for _Symbolic Network: Generalized Neural Policies for Relational MDPs_.
- [ACD-With-GraphRL](https://github.com/cybermonic/ACD-With-GraphRL)
  - Code for _Generalizable Graph-based Reinforcement Learning Agents for Automated Cyber Defense_.
  - Implemented for _Yawning Titan_, _Cage 2_ and _Cage 4_.
- [incident-response-rl-gnn](https://github.com/kasanari/incident-response-rl-gnn)
  - Code for _Structural Generalization in Autonomous Cyber Incident Response with Message-Passing Neural Networks and Reinforcement Learning_.
  - Implemented for _Cage 2_.

### Automated Planning

- [Learning General Optimal Policies with Graph Neural Networks: Expressive Power, Transparency, and Limits](https://zenodo.org/records/6353141)
  - Code from the paper with the same name.
- [GOOSE](https://github.com/DillonZChen/goose)
  - Code for _Return to Tradition: Learning Reliable Heuristics with Classical Machine Learning_.

### Combinatorial Optimization

- [LaGCO-RL](https://github.com/terranovafr/LaGCO-RL)
  - Code for _Projecting Latent RL Actions: Towards Generalizable and Scalable Graph Combinatorial Optimization_.
- [RUN-CSP](https://github.com/RUNCSP/RUN-CSP)
  - Code for _Graph Neural Networks for Maximum Constraint Satisfaction_.
- [graph_comb_opt](https://github.com/Hanjun-Dai/graph_comb_opt)
  - Code for _Learning combinatorial optimization algorithms over graphs_.
- [GNN-Decision-TSP](https://github.com/Panichito/GNN-Decision-TSP)
  - Replication of _Learning to Solve NP-Complete Problems: A Graph Neural Network for Decision TSP_.

### Logic Programming

- [NUDGE](https://github.com/k4ntz/NUDGE)
  - Code for _Interpretable and Explainable Logical Policies via Neurally Guided Symbolic Abstraction_

### Entity-Relational Environments

- [Entity Gym](https://github.com/entity-neural-network/entity-gym)
  - [Motivation](https://clemenswinter.com/2023/04/14/entity-based-reinforcement-learning/)
  - Note: Does not support relations between entities.
- [PyRDDLGym](https://github.com/pyrddlgym-project)
  - "RDDL is a compact, easily modifiable representation language for discrete time control in dynamic stochastic environments."
- [OC Atari](https://github.com/k4ntz/OC_Atari)
  - Object Centric Atari games

## Related Lists

- [Awesome Graph Classification](https://github.com/benedekrozemberczki/awesome-graph-classification)

## Papers Without Code

| Name                                                                                                   | Year | Authors                                                                                                                                                                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------ | ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Decision-Theoretic Planning: Structural Assumptions and Computational Leverage                         | 1999 | Boutilier, C. and Dean, T. and Hanks, S.                                                                                                                                                                                                                                                                                   |
| Relational Reinforcement Learning                                                                      | 2001 | Džeroski, Sašo and De Raedt, Luc and Driessens, Kurt                                                                                                                                                                                                                                                                       |
| Efficient Solution Algorithms for Factored MDPs                                                        | 2003 | Guestrin, C. and Koller, D. and Parr, R. and Venkataraman, S.                                                                                                                                                                                                                                                              |
| Solving Relational MDPs with First-Order Machine Learning                                              | 2003 | Weld, Daniel S and Mausam                                                                                                                                                                                                                                                                                                  |
| Generalizing plans to new environments in relational MDPs                                              | 2003 | Guestrin, Carlos and Koller, Daphne and Gearhart, Chris and Kanodia, Neal                                                                                                                                                                                                                                                  |
| Bellman goes relational                                                                                | 2004 | Kersting, Kristian and Otterlo, Martijn Van and De Raedt, Luc                                                                                                                                                                                                                                                              |
| Approximate linear programming for first-order MDPs                                                    | 2005 | Sanner, Scott and Boutilier, Craig                                                                                                                                                                                                                                                                                         |
| Approximate Policy Iteration with a Policy Language Bias: Solving Relational Markov Decision Processes | 2006 | Fern, A. and Yoon, S. and Givan, R.                                                                                                                                                                                                                                                                                        |
| An object-oriented representation for efficient reinforcement learning                                 | 2008 | Diuk, Carlos and Cohen, Andre and Littman, Michael L.                                                                                                                                                                                                                                                                      |
| Symbolic Dynamic Programming for First-order POMDPs                                                    | 2010 | Sanner, Scott and Kersting, Kristian                                                                                                                                                                                                                                                                                       |
| Near-optimal Reinforcement Learning in Factored MDPs                                                   | 2014 | Osband, Ian and Roy, Benjamin Van                                                                                                                                                                                                                                                                                          |
| Interaction networks for learning about objects, relations and physics                                 | 2016 | Battaglia, Peter W. and Pascanu, Razvan and Lai, Matthew and Rezende, Danilo Jimenez and Kavukcuoglu, Koray                                                                                                                                                                                                                |
| Deep reinforcement learning with relational inductive biases                                           | 2018 | Zambaldi, Vinicius and Raposo, David and Santoro, Adam and Bapst, Victor and Li, Yujia and Babuschkin, Igor and Tuyls, Karl and Reichert, David and Lillicrap, Timothy and Lockhart, Edward and Shanahan, Murray and Langston, Victoria and Pascanu, Razvan and Botvinick, Matthew and Vinyals, Oriol and Battaglia, Peter |
| Structure in Deep Reinforcement Learning: A Survey and Open Problems                                   | 2024 | Mohan, Aditya and Zhang, Amy and Lindauer, Marius                                                                                                                                                                                                                                                                          |
| Transferable dynamics models for efficient object-oriented reinforcement learning                      | 2024 | Marom, Ofir and Rosman, Benjamin                                                                                                                                                                                                                                                                                           |
