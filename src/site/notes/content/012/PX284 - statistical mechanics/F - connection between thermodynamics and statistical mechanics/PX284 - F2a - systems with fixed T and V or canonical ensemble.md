---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/f-connection-between-thermodynamics-and-statistical-mechanics/px-284-f2a-systems-with-fixed-t-and-v-or-canonical-ensemble/","noteIcon":"1","created":"2024-12-05T15:14:47.782+00:00","updated":"2024-12-05T15:42:36.211+00:00"}
---

- in thermodynamics, the hemholtz free energy:
$$F = U - T_{0}S$$
	where, $T = T_{0}$ is fixed
$$ dF  = dQ  + dW - T_{0}\,dS$$
- but, $dQ \leq T_{0}\, dS$
$$\therefore dF \leq dW \implies dF\leq 0$$
- for a mechanically isolated system, ie. $V$ is fixed
- $F$ decreases until a minimum is reached at equilibrium

- similarly, for fixed $S$ and $p$, the enthalpy:
$$dH \leq 0$$
- and, for fixed $T$ and $p:$
$$dG \leq 0$$

[[content/012/PX284 - statistical mechanics/F - connection between thermodynamics and statistical mechanics/PX284 - F2b - aside on lagrange multipliers\|PX284 - F2b - aside on lagrange multipliers]]

- minimizing $F = U - T\,S$ under the constraint $\sum\limits_{i} P_{i} = 1$, ie: 
$$\vec\nabla_{P_{i}}\bigg|U - TS + \lambda \sum\limits_{i}P_{i} \bigg| = 0$$
- trying a particular state with the probability, $P_{j}:$
$$\begin{gather}
\frac{\partial }{\partial P_{j}} \left( \sum\limits _{i} E_{i}P_{i} + k_{B}T \sum\limits_{i}P_{i}\ln P_{i} + \lambda \sum\limits_{i} P_{i} \right) = 0 \\
E_{j} + k_{B}T ( \ln P_{j} +1 ) + \lambda = 0 \\ 
\ln P_{j} = - \frac{E_{j}}{k_{B}T } - \frac{\lambda}{k_{B}T } -1 \\
P_{j} = A \exp\left(- \frac{E_{j}}{k_{B}T }\right)
\end{gather}$$
	where, $A = \frac{1}{Z}$
- this is the [[content/012/PX284 - statistical mechanics/C - entropy and temperature/PX284 - C3 - boltzmann distribution\|boltzmann distribution]]
- therefore, minimizing $F \equiv$ boltzmann distribution
- this is the definition of equilibrium in a canonical ensemble
- it shows that thermodynamics and statistical mechanics are consistent
