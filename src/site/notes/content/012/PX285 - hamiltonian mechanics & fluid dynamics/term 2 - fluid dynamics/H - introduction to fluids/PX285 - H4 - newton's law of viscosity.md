---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h4-newton-s-law-of-viscosity/","noteIcon":"1","created":"2025-08-27T13:15:24.130+01:00","updated":"2025-01-10T12:36:22.000+00:00"}
---

- considering a flow between two parallel plates, where the upper plate is moving at a constant velocity, $\vec u$, and the bottom plate is stationary

![PX285 - H4 - newton's law of viscosity.png|500](/img/user/pics/PX285%20-%20H4%20-%20newton's%20law%20of%20viscosity.png)

- considering a 1D case of a **laminar flow**, so $\vec u = u_{x}(y) \hat i$, and $u_{y} = u_{z} = 0$
- when **steady motion** is obtained, ie. no dependence on time, so, $\cfrac{\partial }{\partial t} = 0$
- a constant force is needed to maintain the flow
$$F \propto \frac{u_{x}A}{ h}$$
	where, $A$ is the area of the plate perpendicular to $\hat j$, ie. parallel to $\vec u$
$$\frac{u_{x}}{h} \propto \frac{\partial u_{x}}{\partial y}$$
- therefore, the force is given by:
$$F = \mu A \frac{\partial u_{x}}{\partial y}$$
	where, $\mu$ is the **viscosity**

- for air at $20\degree$C, $\mu \simeq 1.8\times10^{-5}$ Pa s
- for water at $20\degree$C, $\mu \simeq$

- in the neighbourhood of the moving plate, $y = h$, the fluid acquires a certain amount of mechanical momentum
- this momentum is transferred trough flow in the direction perpendicular to $\vec u$, in y-direction
- this is the effect of viscosity, ie. internal friction in the fluid

- forces that should be considered in fluid mechanics:
	- viscous force
	- gravity
	- negative gradient of pressure $(- \vec\nabla p)$
	- coriolis force
	- lorentz force, for electrically conductive fluids

- if viscosity does not depend on speed, such fluids are known as **newtonian fluids**
	- eg: air, water, plasmas
- if viscosity does depend on speed, such fluids are known as **non-newtonian fluids**
	- eg: oil, blood, emulsions
- only newtonian fluids are discussed in this module
