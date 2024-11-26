---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g2-stiffness-matrix/","created":"2024-11-26T12:40:36.599+00:00","updated":"2024-11-26T12:59:18.993+00:00"}
---

- **note:** from typed notes

## equilibrium conditions
- considering the equilibrium position:
$$\dot q_{i}=0 \; \forall \; q_{i} = constant$$
- this requires $\vec p =0$ and the system remains at equilibrium only if $\dot {\vec p} =0$
- from hamilton's equation, this is only possible id the generalized forces also vanish, ie: $-\frac{\partial H}{\partial q_{i}}=0$
- since all generalized momenta vanish at equilibrium, $T=0$
- thus:
$$\frac{\partial V}{\partial q_{i}}= 0 \tag{1}$$
- this corresponds to the newtonian condition of forces vanishing at equilibrium
## examining the motion
- the equilibrium position:
$$\vec q^{(o)} = \{ q_{1}^{(o)}, q_{2}^{(o)} \dots, q_{i}^{(o)} \dots \}$$
	where, $\frac{\partial V}{\partial q_{i}}\big|_{\vec q^{(o)}} = 0$
- changing the coordinate variables by the translation:
$$x = \vec q - \vec q^{(o)} \iff x_{i} = q_{i}- q_{i}^{(o)} \;\forall\;i$$
- here, $\dot{\vec x} = \dot{\vec q}$, so the definitions of momentum are unchanged
- the taylor expansion of the potential: 
$$ V(x) = V(0) + \sum\limits_{i}x_{i}\frac{\partial V}{\partial x_{i}}\bigg|_{0} + \frac{1}{2}\sum\limits_{ij}x_{i}x_{j} \frac{\partial^{2} {V}}{\partial {x_{i}} \partial x_{j}} \bigg|_{0} +\dots$$
	where, $V(0)$ is the constant value at equilibrium 
- from equation $(1)$, the first derivative is zero
- the generalized forces are given by:
$$\begin{align*}
	F_{i} &= - \frac{\partial V(\vec x)}{\partial x_{i}}\\
	&= - \sum\limits_{j}K_{ij} x_{j}
\end{align*}$$
- the **stiffness/force matrix** is defined as:
$$K_{ij} = \frac{\partial^{2}V }{\partial x_{i}\partial x_{j}}\bigg|_{0}$$
- considering a spring with $V = \frac{1}{2}kx^{2}$, with a restoring force, $F = -kx$, $K$ is a $1\times1$ matric with $K_{11} = k$, the **'stiffness'** of the spring