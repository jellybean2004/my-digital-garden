---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/e-conservation-laws-and-symmetries/px-285-e2-translation-of-space/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-09T14:07:36.774+00:00"}
---

- space is homogenous if the motion of a particle is independent of its absolute position in space, ie: the lagrangian, $L(\vec r , \vec v) = L(q_{1},\dots, \dot q_{1},\dots)$, is unchanged under an arbitrary translation
- under a small translation of ${} \vec r \to \vec r + \delta\vec r {}$: 
$$L(\vec r , \vec v) \to L(\vec r + \delta\vec r, \vec v)  = L(x + \delta x, y + \delta y, z+\delta z, \vec v) $$
- using the taylor expansion: 
$$L(\vec r + \delta\vec r, \vec v)  = L(\vec r, \vec v) + \frac{\partial L}{\partial x}\delta x + \frac{\partial L}{\partial y}\delta y + \frac{\partial L}{\partial z}\delta z$$
$$\delta L = \frac{\partial L}{\partial x}\delta x + \frac{\partial L}{\partial y}\delta y + \frac{\partial L}{\partial z}\delta z = \vec\nabla L \cdot \delta\vec r$$
- if space is homogenous, there should be no change in the lagrangian under translations: 
$$\delta L = 0 \implies \frac{\partial L}{\partial x} = \frac{\partial L}{\partial y}= \frac{\partial L}{\partial z} = 0$$
- recalling the euler-lagrange equations: 
$$\begin{align*}
	\frac{d}{dt}\frac{\partial L}{\partial \dot x} &= \frac{\partial L}{\partial x} =0 \\
	\frac{d}{dt}\frac{\partial L}{\partial \dot y} &= \frac{\partial L}{\partial y} =0 \\
	\frac{d}{dt}\frac{\partial L}{\partial \dot z} &= \frac{\partial L}{\partial z} =0 \\\\
	\dot p_{x} = \dot p_{y} &=  \dot p_{z}=0
\end{align*}$$
- the canonical momenta remain constant during the motion
- for a single particle, this is also the total momentum of the system
## generalized
- for $N$ particles, each at position, $\vec r_{a}$, with velocity, $v_{a}:$ 
$$\delta L = \sum\limits_{a} \left(\frac{\partial L}{\partial x_{a}} \delta x + \frac{\partial L}{\partial y_{a}} \delta y + \frac{\partial L}{\partial z_{a}} \delta z\right) = \sum\limits_{a}\frac{\partial L}{\partial \vec r_{A}} \cdot \vec{\delta r}$$
- the condition of homogeneity of space is that $\delta L =0:$ 
$$\sum\limits_{a}\frac{\partial L}{\partial \vec r_{a}}=0 \implies \sum\limits_{a} \frac{d}{dt}\frac{\partial L}{\partial \vec v_{a}} =0$$
- for any closed system, the sum of the canonical vector momenta, $\vec P = \sum\limits_{a} \frac{\partial L}{\partial \vec v_{a}}$, remains constant
