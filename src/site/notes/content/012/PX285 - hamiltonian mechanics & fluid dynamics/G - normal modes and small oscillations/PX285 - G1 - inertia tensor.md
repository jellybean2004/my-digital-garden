---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g1-inertia-tensor/","noteIcon":"1","created":"2024-11-26T12:37:58.111+00:00","updated":"2024-11-26T12:59:07.569+00:00"}
---

- **note:** from typed notes

- the kinetic energy in the most general quadratic form:
$$T = \frac{1}{2} \sum\limits_{ij}M_{ij}\dot q_{i} \dot q_{j}$$
	where, $M_{ij}$ are a number of arbitrary coefficients, a set of which can be thought of as a square matrix
- as $\dot q_{i}\dot q_{j} = \dot q_{j}\dot q_{i}$, there is not distinction between $M_{ij}$ and $M_{ji}$, and they can be thought of as a symmetric matrices with commuting indices:
$$M_{ij} = M_{ji}$$
- the canonical momenta: 
$$\begin{align*}
p_{k} &= \frac{\partial L}{\partial \dot q_{k}} \\
&= \frac{\partial }{\partial \dot q_{k}} \frac{1}{2}\sum\limits_{ij}M_{ij}\dot q_{i}\dot q_{j} \\
&= \frac{1}{2}\sum\limits_{ij}(M_{ij} \dot q_{i} \frac{\partial \dot q_{j}}{\partial \dot q_{k}} + M_{ij} \dot q_{j} \frac{\partial \dot q_{i}}{\partial \dot q_{k}}) \\
&= \frac{1}{2}\sum\limits_{ij} M_{ij} (\dot q_{i}\delta_{jk} + \dot q_{j}\delta_{ik}) \\
\therefore p_{k} &= \sum\limits_{j}M_{jk} \dot q_{j}
\end{align*}$$
- $M_{ij}$ is the **inertia tensor** (or matrix), which relates the conical momenta to the generalised velocities
- this can be used to calculate the hamiltonian
$$\sum\limits_{i}p _{i}\dot q_{i} = \sum\limits_{i}\sum\limits_{j} M_{ij} \dot q_{j} \dot q_{i} = 2T$$
- the hamiltonian:
$$H = \sum\limits_{i} p_i \dot q_{i} - L = 2T - (T-V) = T + V$$
	which is as required
