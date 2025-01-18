---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/c-calculus-of-variations/px-285-c6d-two-particles-in-3-d/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:26.824+00:00"}
---

## basic case
- consider two particles with the same mass, $m$, in positions, $(x_{1},y_{1},z_{1})$ and ${} (x_{2},y_{2},z_{2}) {}$, so $d=6$
- the lagrangian: 
$$L =-= \frac{1}{2} m(v_{1}^{2}+v_{2}^{2}) - V(x_{1},\dots z_{2})$$
	where, $v_{d}^{2}=\dot x_{d}^{2}+\dot y_{d}^{2}+\dot z_{d}^{2}$
- expect six euler-lagrange equations: 
$$\begin{gather}
	-\frac{\partial V}{\partial x_{1}} = \frac{d}{dt}m\dot x_{1} = \frac{d}{dt}p_{x_{1}} \\
	\vdots
\end{gather}$$
## special case
- now, consider if the potential was a function of only the separation, ie: $V(r)$, where $r = \sqrt{(x_{2}-x_{1})^{2}+(y_{2}-y_{1})^{2}+(z_{2}-z_{1})^{2}}$
- redefine:
	$q_{1}=x_{2}-x_{1}$
	${} q_{2}=y_{2}-y_{1} {}$
	$q_{3}=y_{2}-y_{1}$
	$q_{4}=x_{2}+x_{1}$
	${} q_{5}=y_{2}+y_{1} {}$
	$q_{6}=z_{1}+z_{2}$
- there s a one-to-one mapping: $q_{1}\leftrightarrow x/y/z_{i}$, eg: $z_{1} = \frac{q_{6}-q_{3}}{2}$ 
- there will be three non-trivial equations of motion with a non-zero $LHS:$ 
$$\frac{\partial L}{\partial q_{1}} = \frac{d}{dt} \frac{\partial L}{\partial \dot q_{1}} = \frac{d}{dt}p_{1}$$
	and so on for $q_{2}$ and $q_{3}$
- there will be three trivial equations: 
$$\frac{\partial L}{\partial q_{4}} = \frac{d}{dt} \frac{\partial L}{\partial \dot q_{4}} = \frac{d}{dt}p_{4}=0$$
	and so on for $q_{5}$ and $q_{6}$
- this is because $V$ has no dependence on them, so the corresponding momenta are constant, and conserved