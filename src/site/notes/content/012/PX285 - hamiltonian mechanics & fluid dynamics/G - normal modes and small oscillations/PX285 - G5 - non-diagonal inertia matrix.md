---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g5-non-diagonal-inertia-matrix/","created":"2024-11-28T18:39:30.659+00:00","updated":"2024-11-29T06:32:05.376+00:00"}
---

![Pasted image 20241129063120.png|500](/img/user/pics/Pasted%20image%2020241129063120.png)
- the velocity of the first mass is $\dot l_1$, and of the second mass is $\dot l_{1 +}\dot l_2$
- the kinetic energy of the system:
$$T  = \frac{1}{2} m\dot l_{1}^{2} + \frac{1}{2} m(\dot l_{1}  + \dot l_{2})^{2} = m\dot l_{1}^{2}  + \frac{1}{2}m \dot l_{2}^{2}  + \frac{1}{2}m \dot l_{1} \dot l_{2}$$
- $\dot l_{1} \dot l_{2}$ is an off-diagonal term
- the inertia matrix: 
$$M = \begin{pmatrix}m & \frac{m}{2} \\ \frac{m}{2} & \frac{m}{2}\end{pmatrix}$$

- the generalized force:
$$F_{k} = \frac{\partial L}{\partial x_{k}} = - \frac{\partial V}{\partial x_{k}}$$
- normal modes represent small displacements from the equilibrium when response is linear
 ![Pasted image 20241129063140.png|500](/img/user/pics/Pasted%20image%2020241129063140.png)
 - considering the case where the displacements are a small distance from an equilibrium point
 - **equilibrium** is defined to be when there is no force, or the potential is at the minimum:
$$F = -  \frac{dV}{dx} = 0$$
- at equilibrium in more than one dimension, all components of the force must vanish:
$$F_{i} = - \frac{\partial V}{\partial x_{i}} = 0 \;\forall i$$
- a change of variables (shift of the coordinate axes)can be made  to engineer the equilibrium point of interest to be at $x=0$
![Pasted image 20241129063200.png|500](/img/user/pics/Pasted%20image%2020241129063200.png)
- potential might have a minimum at $q_{i} = q_{i}^{(0)} \neq 0$
- so, a new coordinate can be defined such that: $x_{i} = q_{i}- q_{i}^{(0)}$
- this makes calculations convenient
- the potential: $V(x_{1},x_{2},\dots) = V(\vec x)$
- [[content/011/PX153 - mathematics for physicists/term 1/PX153 - G - functions of many variables, calculus/PX153 - G4 - taylor expansion of a function of two variables\|taylor expansion]] about the equilibrium:
$$\begin{align*}
	 V(\vec x) &= V(0) + \sum\limits_{i}  \underbrace{\frac{\partial V}{\partial x_{i}} \bigg|_{\vec x=0} }_{=0}x_{i} + \frac{1}{2} \sum\limits_{i}\sum\limits_{j}\frac{\partial^{2} V}{\partial x_{i}x_{j}} \big|_{\vec x = 0} + \dots \\
	 &= V(0) +  \frac{1}{2} \sum\limits_{i}\sum\limits_{j}\frac{\partial^{2} V}{\partial x_{i}x_{j}} \big|_{\vec x = 0} + \dots
\end{align*}$$
- writing the second derivative as the [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/G - normal modes and small oscillations/PX285 - G2 - stiffness matrix\|stiffness matrix]], $K_{ij}$
$$F_{k} = \frac{\partial L}{\partial x_{k}} = - \frac{\partial V}{\partial x_{k}}$$
	where,  $F_{k}$ is the $k^{th}$ element of $\vec F$
$$\begin{align*}
	F_{k} &\approx - \frac{\partial V}{\partial x_{k}} = - \frac{\partial }{\partial x_{k}} \left[V\left(0\right) + \frac{1}{2}\sum\limits_{ij} K_{ij} x_{i}x_{j}\right] \\
	&= - \frac{1}{2} \sum\limits_{ij}K_{ij} \left[ \frac{\partial x_{i}}{\partial x_{j}} x_{k} + x_{i} \frac{\partial x_j}{\partial x_{k}}\right] \\
	&= - \frac{1}{2} \sum\limits_{ij}K_{ij} \left[ \delta_{ik} x_{j} + x_{i} \delta_{jk}\right] \\
	&= -\frac{1}{2} \left[\sum\limits_{j} K_{kj}x_{j} + \sum\limits_{i} K_{ik}x_{i}\right] \\
	\therefore F_{k}&= -\sum\limits_{ik} K_{ik} x_{i}
\end{align*}$$
$$\implies \frac{d}{dt} \sum\limits_{i} M_{ik} \dot x_{i} = \sum\limits_{i} M_{ik} \ddot x_{i} = - \sum\limits_{i} K_{ik}x_{i}$$
- this can be written as:
$$M \ddot {\vec x}  = - k \vec x$$
	where $M$ is the inertia matrix, and $K$ is the stiffness matrix
$$\begin{align*}
M_{ij} = \frac{\partial^{2} {T}}{\partial {\dot x_{i}}\partial \dot x_{j}} \\
K_{ij} = \frac{\partial^{2} {V}}{\partial {x_{i}}\partial x_{j}}
\end{align*}$$
