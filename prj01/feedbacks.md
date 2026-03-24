Kenta:
The scope is good if kept narrow: simple 2D geometry + COMSOL benchmark is a solid starting point. I would avoid expanding too early before showing that the PINN is accurate and stable on the baseline problem.
Since the reference paper already uses a PINN, it may help to explain what your novelty is beyond reproducing it. For example: better geometry handling, faster inference, stronger coupling to CFD, or inverse design of distributor layouts.

Farhad:
Good aspects:
The project has a clear objective: comparing KANs vs. MLPs within a PINN framework for solving PDEs.
Suggestions for improvement:
Maybe it's good to ensure fair comparison by matching model capacity (similar number of parameters or FLOPs).
Recommending to consider comparing training stability and gradient behavior, since PINNs can suffer from optimization issues.

Nick:
Alternative idea: Dummy edges
In standard GNNs, information propagates only one hop per layer.
Instead of introducing hierarchical levels, maybe you can add dummy edges connecting nodes that are k-hop neighbors.
These edges allow the model to directly exchange information between distant nodes without requiring many layers.
Maybe comparing that with your approach? Here is the paper I was talking about:
Bruel-Gabrielsson, Yurochkin, Solomon (2022), Rewiring with Positional Encodings for Graph Neural Networks.
https://arxiv.org/pdf/2201.12674
