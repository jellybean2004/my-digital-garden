---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h6a-stream-line/","noteIcon":"1","created":"2025-01-10T12:52:24.907+00:00","updated":"2025-01-16T14:51:47.442+00:00"}
---

- a **stream line** is a curve, generally in 3D, which at a fixed time at each location is tangential to the fluid velocity, $\vec u$
- let $d\vec r$ be parallel to a stream line, ie: $d\vec r \parallel \vec u$ , or, $d\vec r = d\lambda \vec u$, where $d\lambda$ is a small scalar
	$dx = d\lambda u_x$
	$dy = d\lambda u_y$
	$dz = d\lambda u_z$
$$d\lambda = \frac{dx}{u_{x}}= \frac{dy}{u_{y}} = \frac{dz}{u_{z}}$$
- the solution to the above differential equations describe stream lines

- eg: considering a velocity: $\vec u = u_{0}(-2y, x ,0)$

$$\frac{dx}{u_{x}} = \frac{dx}{-2y} = \frac{dy}{x} = \frac{dy}{du_{y}}$$
- separating the variables:
$$\int x\,dx = \int-2y \,dy \implies \frac{x^{2}}{2} = - y^{2} + c$$
- the solution belongs to a family of ellipses, with different ellipses for different $c$ values
- therefore, it is a deformed vortex

![PX285 - H6 - stream line.png|500](/img/user/pics/PX285%20-%20H6%20-%20stream%20line.png)
