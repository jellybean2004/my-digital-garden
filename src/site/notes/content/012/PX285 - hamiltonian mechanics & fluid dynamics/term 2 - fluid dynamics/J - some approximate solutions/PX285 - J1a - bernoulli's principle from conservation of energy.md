---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/j-some-approximate-solutions/px-285-j1a-bernoulli-s-principle-from-conservation-of-energy/","noteIcon":"1","created":"2025-01-24T12:51:54.480+00:00","updated":"2025-04-16T07:52:46.388+01:00"}
---

- considering a stream lined flow, with $A_{1}$ and $A_{2}$ as the cross-sectional areas of the flow tube

![PX285 - I3 - bernoulli's principle-1.png|500](/img/user/pics/PX285%20-%20I3%20-%20bernoulli's%20principle-1.png) 

- the rate at which the fluid enters region 1: 
$$\rho_{1}A_{1}u_{1}$$
- work is done on fluid by the pushing from behind (left to right in the sketch): 
$$W = Fd = \frac{Fu}{t}$$
- the rate at which work is done is: 
$$P_{1}A_{1}u_{1}$$
- the rate at which kinetic energy of the fluid enters region 1: 
$$\frac{1}{2} \rho_{1}A_{1}u_{1} (u_{1})^{2}$$
- and likewise, the gravitational potential energy: 
$$\rho_{1} A_{1} u_{1} g z_{1}$$

- the expressions for region 2 will be identical

- from conservation of mass, if flow is incompressible:
$$\rho_{1} A_{1}u_{1} = \rho_{2}A_{2}u_{2}$$

- considering a constant internal energy, ie. no friction, so the flow is inviscid
- from conservation of energy:
$$\rho A_{1}u_{1} \left(\frac{u_{1}^{2}}{2} + gz_{1} + \frac{P_{1}}{\rho}\right) = \rho A_{2}u_{2} \left(\frac{u_{2}^{2}}{2} + gz_{2} + \frac{P_{2}}{\rho}\right)$$
- the pre-factors cancel out from conservation of mass

- therefore, the invariant of the flow along a stream line:
$$\rho \frac{u^{2}}{2} + \rho g z + P = \text{constant}$$
- this is called **bernoulli's principle**
- required conditions: 
	- incompressible, ie: $\vec\nabla\cdot\vec u = 0$
	- inviscid, ie: $\mu=0$
	- steady, ie: $\frac{\partial }{\partial t} = 0$
