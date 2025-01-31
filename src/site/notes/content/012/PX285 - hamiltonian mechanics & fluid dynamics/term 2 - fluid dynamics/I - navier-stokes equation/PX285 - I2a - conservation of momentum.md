---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i2a-conservation-of-momentum/","noteIcon":"1","created":"2025-01-31T13:44:21.284+00:00","updated":"2025-01-31T14:21:04.257+00:00"}
---

- considering a *lagrangian* fluid element of volume, $V$, that moves at the fluid velocity, ${} \vec u {}$
	- *lagrangian*: its mass is constant, ie: $\rho\,dV =$ constant
- the rate of change of momentum:
$$\frac{d}{dt} (\rho\, dV\, \vec u) = \rho \, dV \frac{d\vec{u}}{dt}$$
	where, $\cfrac{d\vec{u}}{dt} = \cfrac{\partial \vec u}{\partial t} + (\vec u \cdot \nabla) \vec u$
[[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/I - navier-stokes equation/PX285 - I2b - advective derivative\|PX285 - I2b - advective derivative]]
- momentum conservation is newton's second law:
$$\vec F = m \vec a  = \rho\, dV \, \frac{D\vec u}{Dt}$$
- $dV$ can be dropped to calculate the force per unit volume/force density, that can be called force in shorthand

- the pressure force is $-\vec\nabla P$
- the force due to gravity is $\rho \vec g$

- combining the above, and the viscous force:
$$\implies \rho \frac{d \vec u}{dt} = \sum\limits \frac{\vec F}{dV} = - \vec\nabla P + \vec F_{v} + \rho \vec g + \dots$$
- the viscous force:
$$\vec F_{v} = \mu \nabla^{2}\vec u + \lambda \vec\nabla (\vec\nabla \cdot \vec u)$$
	where, $\mu$ and $\lambda$ arise from the shear and volume viscosities, respectively
- often, $\lambda \approx \mu/3$

- hence, the **navier-stokes equation** for incompressible fluids ${} (\vec\nabla\cdot\vec u = 0): {}$
$$\rho \frac{\partial \vec u}{\partial t} + \rho (\vec u \cdot \vec\nabla) \vec u = - \vec\nabla P + \mu \nabla^{2} \vec u - \rho g \hat k $$
- **note:**
	- the full continuity equation for $\rho$ involves ${} \vec u$
	- the NS for $\vec u$ involves $P$, so additional equation for $P$ is needed, which comes from the conservation of energy
