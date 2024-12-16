---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/c-calculus-of-variations/px-285-c6c-two-particles-in-1-d/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:25.815+00:00"}
---

## basic case
- consider two particles with the same mass, $m$, in positions, $x_{1}$ and $x_{2}$, so $d=4$
- the lagrangian: 
$$L =-= \frac{1}{2} m(\dot x_{1}^{2}+\dot x_{2}^{2}) - V(x,y)$$
- the euler-lagrange equations: 
$$\begin{gather}
	-\frac{\partial V}{\partial x_{1}} = \frac{d}{dt}m\dot x_{1} = \frac{d}{dt}p_{1} = F_{1} \\
	-\frac{\partial V}{\partial x_{2}} = \frac{d}{dt}m\dot x_{2} = \frac{d}{dt}p_{2} = F_{2}
\end{gather}$$
- define $\vec p = \begin{pmatrix}p_{x} \\ p_{y}\end{pmatrix}$, and $\vec F = \begin{pmatrix}F_{1} \\ F_{2}\end{pmatrix}$
- therefore, newton's law is obtained again: 
$$\vec F = \frac{d}{dt}\vec p$$
## special case
- now, consider $V(x_{1}, x_{2}) = U(x_{1}-x_{2}) = U(z)$
$$\begin{gather}
-\frac{\partial V}{\partial x_{1}} = - \frac{\partial U}{\partial z}\frac{\partial z}{\partial x_{1}} = -U'(z) \\
-\frac{\partial V}{\partial x_{1}} = F_{1} = - U'(z)
\end{gather}$$
$$\begin{gather}
-\frac{\partial V}{\partial x_{2}} = - \frac{\partial U}{\partial z}\frac{\partial z}{\partial x_{2}} = +U'(z) \\ 
-\frac{\partial V}{\partial x_{2}} = F_{2} = +U'(z)
\end{gather}$$
- newton's third law can be seen: 
$$F_{1}= - F_{2}$$
- there is also no time-dependence in momentum: 
$$\frac{d}{dt}(m(\dot x_{1}^{2} + \dot x_{1}^{2})) = \frac{d}{dt}(p_{1}+p_{2}) = F_{1}+F_{2}=0$$
