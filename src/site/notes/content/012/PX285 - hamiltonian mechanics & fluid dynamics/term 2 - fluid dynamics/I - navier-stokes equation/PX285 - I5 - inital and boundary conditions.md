---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i5-inital-and-boundary-conditions/","noteIcon":"1","created":"2025-01-31T13:27:32.532+00:00","updated":"2025-01-31T14:52:17.632+00:00"}
---

- considering a rigid object in flow at the object's boundary, $u_{\perp} = 0$, locally normal to the boundary
- boundary conditions: 
	- 'rigid wall'
	- 'no flux', ie. nothing can flow into a solid, and on the surface of a moving object in a fluid, $\vec u$ matches the velocity of the object's boundary
	- 'no slip': $u_{\parallel} = 0 \implies \vec u = 0$ at the boundary

- rederiving the **reynold's number** from the navier-stokes equation

- considering flow over an obstacle

![PX285 - I2 - core equations.png|500](/img/user/pics/PX285%20-%20I2%20-%20core%20equations.png)

- comparing the inertial and the viscous terms:
$$\begin{gather}
|\rho(\vec u \cdot \vec\nabla) \vec u| \sim \frac{\rho_{0}u_{0}^{2}}{L_{0}} \\
|\mu\nabla^{2}\vec u| \sim \frac{\mu u_{0}}{L_{0}^{2}}
\end{gather}$$
	where, $\nabla \sim 1/L_0$

- the ratio of the inertial and the viscous terms:
$$\frac{\rho_{0}u^{2}}{L_{0}} \cdot\frac{L_{0}^{2}}{\mu u_{0}} = \frac{\rho_{0}u_{0}L_{0}}{\mu} = Re$$
- so, reynold's number estimates the relative importance of the inertial and he viscous terms
- if it is large, the flow is inviscid, $\mu = 0$
- if it is small, the inertial flow can be neglected, ${} \rho \frac{\partial \vec u}{\partial t} =$ force densities

- eg: the pousselle flow:
$$0 = \rho \frac{\partial \vec u}{\partial t} = - \vec\nabla P + \mu \nabla^{2} \vec u - \frac{\partial \rho}{\partial x} + \mu \frac{\partial^{2} {u_{x}}}{\partial {y}^{2}}$$

- since the navier-stokes equation is a second order PDE, there is a need for $u_{\parallel}$, $u_\perp$ at boundaries
- in the inviscid limit, terms with $\mu \to 0$ 
- this turns into a first order PDE - **euler equation**
- only one boundary condition is needed, eg. for $u_\perp$

![PX285 - I2 - core equations-1.png|500](/img/user/pics/PX285%20-%20I2%20-%20core%20equations-1.png)

- the velocity experiences a '*sharp*' gradient near the boundary
- euler and navier-stokes equations are similar except for a width, $\delta$, near the boundary - **transition region**
- hence, the inertial and viscous terms:
$$\begin{gather}
| \rho ( \vec u \cdot \vec\nabla) \vec u| \sim \frac{\rho_{0}u_{0}^{2}}{L_{0}} \\
|\mu \nabla^{2} \vec u | \sim \frac{\mu u_0}{\delta^{2}}
\end{gather}$$

- at the outer boundary of transition region:
$$\frac{\rho_{0}u_{0}^{2}}{L_{0}} \sim \frac{\mu u_{0}}{\delta^{2}}$$
$$\frac{\delta}{L_{0}}\approx \sqrt{\frac{\mu}{\rho_{0}u_{0}L_{0}}} = (Re)^{-1/2}$$

- for large reynolds number flows, thin layer near the boundary where viscosity **cannot** be ignored
- this is called the **boundary layer**
- outside this, $\mu = 0$ will be an accurate model
- 