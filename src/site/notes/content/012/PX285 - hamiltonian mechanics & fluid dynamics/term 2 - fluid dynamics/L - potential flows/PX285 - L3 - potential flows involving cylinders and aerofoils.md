---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l3-potential-flows-involving-cylinders-and-aerofoils/","noteIcon":"1","created":"2025-08-27T13:15:24.465+01:00","updated":"2025-03-07T13:18:24.000+00:00"}
---

- neglecting vorticity, and considering an irrotational and incompressible flow, with potential given by: $\nabla^{2} \phi = 0$
- $\nabla^{2}\phi$ is linear, with linear boundary conditions
- a sum of solutions is also a solution
- considering a sum of uniform flow and potential dipole
$$\phi = U_{0} x + \frac{a\cos\theta}{r}$$
- considering cylindrical coordinates are used, with the origin at the dipole:
$$\phi = U_{0} r \left(l + \frac{R^{2}}{r^{2}}\right) \cos\theta$$
	where, $R^{2} = a/u_{0}$, $u_{0}$ is the speed at a large distance from dipole

$$\begin{gather}
\vec u : u_{r} = \frac{\partial \phi}{\partial r} = U_{0} (1 - R^{2}/r^{2})\cos\theta \\
u_{\theta} = \frac{1}{r} \frac{\partial \phi}{\partial \theta} = - U_{0} r ( 1 + R^{2}/r^{2})\sin\theta
\end{gather}$$
- the stagnation points: $u_{r}(r,\theta) = 0$ and $u_\theta(r,\theta) = 0$ at $r =R$ and $\theta = 0,\pi$

![PX285 - K5a - potential flows involving cylinders and aerofoils.png|500](/img/user/pics/PX285%20-%20K5a%20-%20potential%20flows%20involving%20cylinders%20and%20aerofoils.png)

- there is no flow through the surface
- hence, it can be considered rigid, ie: $u_{\perp} = 0$
- instead of the dipole, a cylinder of radius, R, can be put

![PX285 - K5a - potential flows involving cylinders and aerofoils-1.png|500](/img/user/pics/PX285%20-%20K5a%20-%20potential%20flows%20involving%20cylinders%20and%20aerofoils-1.png)

- at the surface of the cylinder, ie: $r = R$
$$\begin{gather}
u_{r} = 0 \\
u_{\theta} = - 2U_{0}\sin\theta \\
u_{\theta, max} = 2U_{0} \; \text{ at } \theta = \frac{\pi}{2}, - \frac{\pi}{2}
\end{gather}$$

- $u_{\theta}\neq 0$ is not consistent with the condition that $\vec u = 0$ at $r = R$
- this will be revisited when viscosity is considered

![PX285 - K5a - potential flows involving cylinders and aerofoils-2.png|500](/img/user/pics/PX285%20-%20K5a%20-%20potential%20flows%20involving%20cylinders%20and%20aerofoils-2.png)

- calculating the force experienced by the cylinder from the flow
- determining the pressure on the surface of the cylinder using [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/J - some approximate solutions/PX285 - J1a - bernoulli's principle from conservation of energy\|bernoulli's principle]] at a large distance, $x\to -\infty$:
$$\begin{gather}
P_{0} + \frac{\rho}{2} U_{0}^{2}  = P_{s} + \frac{\rho}{2} u_{\theta}^{2} (R) \\
P_{s} = P_{0} + \frac{1}{2} \rho U_{0} ^{2} (1 - 4 \sin^{2} \theta)
\end{gather}$$

![PX285 - K5a - potential flows involving cylinders and aerofoils-3.png](/img/user/pics/PX285%20-%20K5a%20-%20potential%20flows%20involving%20cylinders%20and%20aerofoils-3.png)

- the net force from the flow on the cylinder:
$$d\vec S = (\cos\theta, \sin\theta) R\,d\theta$$
$$\begin{align*}
F_{x} &= -\int P (d\vec S)_{x} \\
&= - \int_{0}^{2\pi} P_{s}(\theta ) R\cos\theta\, d\theta \\
&= \left(P_{0} + \rho \frac{U_{0}^{2}}{2}\right)R \int_{0}^{2\pi} \cos\theta \, d\theta\\
&= 0
\end{align*}$$

- similarly, the force in $\hat y:$
$$F_{y} = \int_{0}^{2\pi} P_{s} R\sin \theta \, d\theta = 0$$

- therefore, the  cylinder does not experience any net force:
$$|\vec F| = 0$$
- the failure to satisfy the boundary condition and the net force at the boundary being zero is called the **d'Alembert paradox**, which is resolved by accounting for viscosity and turbulence
