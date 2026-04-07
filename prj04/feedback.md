## Farhad
KANs use fewer parameters, so their representational capacity is lower compared to PINNs. As a result, a higher total loss (≈2×) is not surprising—especially since the loss includes both interior MSE and a heavily weighted boundary term (λ = 10). Despite this, achieving comparable performance with ~50% fewer parameters suggests that KANs are more parameter-efficient.

## Nick
This result suggests that the chosen L2-based objective is learnable, since both optimizers reduce the loss, but Adam is clearly more effective and reaches about 0.03 while SGD plateaus higher. The remaining oscillations likely come from training dynamics, such as no mini-batching or learning-rate effects, rather than from the PDE formulation itself. Maybe the following gating mechanism can be helpful, although the problem in the following paper is different from your problem (problem in both is spiky losses, but the reason behind that is different):
[text](https://arxiv.org/pdf/2505.06708)