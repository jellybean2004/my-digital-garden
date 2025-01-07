---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g2-functions-of-a-multiple-variables/","noteIcon":"1","created":"2025-01-07T12:27:42.976+00:00","updated":"2025-01-07T12:40:43.878+00:00"}
---

- in physics, a common pairing is a spatially varying quantity, with a spatial dimension, $x$, and time, $t$
- eg: density of particles:
	- $c(x,t)$ is the concentration of particles
	- $Q(x,t)$ is the heat energy density
	- $u(x,t)$ is the displacement of a string

- partial derivatives are defined as:
$$\frac{\partial u(x,t)}{\partial x} \; \text{and}\; \frac{\partial u(x,t)}{\partial t}$$
- this leads to **partial differential equations (PDES)**
- it can be extended to an arbitrary combination of independent variables; eg: multiple spatial dimensions: $f(\vec r, t)$, where $\vec r = (x,y,z)$ or $\vec r = (r,\theta,\varphi)$, or, ant set of independent variables: $f(x_{1}, x_{2}, \dots, x_{N}) \implies \frac{\partial f}{\partial x_{i}}$, where, $i \in [1,N]$

- the wave equation is an example of a PDE:
$$\frac{\partial^{2} {u(x,t)}}{\partial {t}^{2}} = c^{2} \frac{\partial^{2} {u(x,t)}}{\partial {x}^{2}}$$

- **note:** the notation may differ:
	- $\dot u$ is often associated with the time derivative, ${} \cfrac{\partial }{\partial t} {}$
	- $u'$ is often associated with the$\cfrac{\partial }{\partial x}$
	- or subscripts: ${} u_{t} = \cfrac{\partial u}{\partial t} {}$ and $u_{x} = \cfrac{\partial u}{\partial x}$
- the wave equation can also be written as:
$$\begin{align*}
u_{tt} &=  c^{2}u_{xx} \\
\ddot u &= c^{2}u''
\end{align*}$$
