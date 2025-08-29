---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l4a-lift-and-circulation-magnus-effect/","noteIcon":"1","created":"2025-08-27T13:15:24.475+01:00","updated":"2025-03-07T13:26:07.000+00:00"}
---

![PX285 - K5b - potential flow with rotating cylinder.png|500](/img/user/pics/PX285%20-%20K5b%20-%20potential%20flow%20with%20rotating%20cylinder.png)

- considering that the cylinder is rotating around its axis, which would drag the fluid in the direction of rotation due to viscosity
- modelling it as:
$$\phi = U_{0}r \left(1 + \frac{R^{2}}{r^{2}}\right) \cos\theta  - \frac{K}{2\pi} \theta$$
	where, the negative term is the free vortex due to clockwise rotation
$$\begin{gather}
u_{r} = \frac{\partial \phi}{\partial r} = U_{0} \left( 1 - \frac{R^{2}}{r^{2}}\right) \cos\theta \\
u_{\theta} = \frac{1}{r}\frac{\partial \phi}{\partial \theta} = - U_{0} \left( 1 + \frac{R^{2}}{r^{2}}\right) \sin\theta - \frac{K}{2\pi r} 
\end{gather}$$

- at the surface of the cylinder, $r = R:$
$$\begin{gather}
u_{r}(r = R) = 0 \implies \text{rigid wall} \\
u_{\theta} (r = R) = - 2 U_{0} \sin\theta  - \frac{K}{2\pi R}
\end{gather}$$
- the pressure around the cylinder, $P_{s}(\theta):$
$$\begin{gather}
P_{0} + \frac{1}{2} \rho U_{0} ^{2}= P_{s} + \frac{1}{2}\rho U_{\theta}^{2} \\
P_{s}(\theta) = P_{0} + \frac{\rho U_{0}^{2}}{2}  - \frac{\rho}{2} \left[ \frac{K^{2}}{4\pi R^{2}} + 4U_{0}^{2}\sin^{2}\theta  + \frac{4}{2}  \frac{U_{0}K}{\pi R} \sin\theta\right]
\end{gather}$$
- the force:
$$\begin{gather}
\vec F = - \int P_{s}(\theta)  \,d\vec S \\
F_{x} = - \int_{0}^{2\pi} P_{s}(\theta ) \cos\theta \, R\,d\theta = 0 \\
F_{y} = - \int_{0}^{2\pi} P_{s}(\theta ) \sin\theta \, R\,d\theta = \rho U_{0}K
\end{gather}$$
- there is no drag (ie. force in the $x$ direction)
- the force is perpendicular to the velocity, which can be the lift force:
$$\vec L = \rho \vec U_{0} \times \vec K$$
	where, $\vec K$ is the circulation vector

- this is called the **magnus effect**

- in the fluid's frame of reference:
$$\vec L = \rho \vec K \times\vec U_{obj}$$
	where, $\vec U_{obj}$ is the velocity of a moving object with respect to the stationary fluid

- in the vicinity of the boundary, the no-slip condition applies as a boundary condition
- the flow moves with the cylinder
- from bernoulli's principle: $u_{t} > u_{b}$, and if $P_{s}^{(t)}> P_{s}^{(b)}$, then there is lift
