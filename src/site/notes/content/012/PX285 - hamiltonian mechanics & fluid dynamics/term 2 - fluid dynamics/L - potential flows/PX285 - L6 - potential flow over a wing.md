---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l6-potential-flow-over-a-wing/","noteIcon":"1","created":"2025-03-06T14:35:10.624+00:00","updated":"2025-03-07T14:22:53.142+00:00"}
---

![PX285 - L6 - potential flow over a wing.png|500](/img/user/pics/PX285%20-%20L6%20-%20potential%20flow%20over%20a%20wing.png)

- everywhere except the transition region, the flow is irrotational, incompressible, and follows the laplace equation
- since the shape is complex, it is not analytically tractable
- numerically solving the laplace equation  around the aerofoil: $\nabla^{2} \phi = 0$
- the boundary conditions: $u_{\perp} = 0$ at the surface, ie: $\hat n \cdot u = 0$ ; $u = u_{0} \hat i$, far from the aerofoil
- at $A$, since it is incompressible: $\vec\nabla \times \vec u = 0  \implies K = 0$, so the net lift by magnus effect is zero
- using a wind tunnel to measure the flow once it has reached a steady state, it is found that the stagnation point, $B$, lies on the trailing edge

![PX285 - L6 - potential flow over a wing-1.png|500](/img/user/pics/PX285%20-%20L6%20-%20potential%20flow%20over%20a%20wing-1.png)

- since there are differences in speeds, and hence pressure, there will be a lift force
- this mismatch is caused by the need for considering the transition region
- the transition (or boundary) region (or layer) near an object:
$$\frac{\delta}{d} = \frac{1}{\sqrt{Re}} = \left(\frac{\mu}{\rho u_{0}d} \right)^{1/2}$$

- $B$ can be moved from the potential flow pattern to the trailing edge by adding a circulation to the flow around the wing:

![PX285 - L6 - potential flow over a wing-2.png|500](/img/user/pics/PX285%20-%20L6%20-%20potential%20flow%20over%20a%20wing-2.png)

- equivalently, a circulation of the opposite sign can be subtracted
- this is called **vortex shedding**
