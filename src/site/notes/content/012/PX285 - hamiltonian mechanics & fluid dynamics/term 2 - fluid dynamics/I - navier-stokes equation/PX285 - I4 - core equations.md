---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i4-core-equations/","noteIcon":"1","created":"2025-01-24T12:09:51.045+00:00","updated":"2025-01-31T14:25:47.046+00:00"}
---


- the continuity equation:
$$\frac{\partial \rho}{\partial t} + \vec\nabla\cdot (\rho \vec u) = 0 $$
- this reduces to $\vec\nabla\cdot\vec u = 0$ for incompressible fluids

- the momentum equation:
$$\rho \left(\frac{\partial \vec u}{\partial t} + (\vec u \cdot\vec\nabla) \vec u \right) = - \vec\nabla P - \rho g \hat k  + \mu \nabla^{2} \vec u + \lambda \nabla (\vec\nabla\cdot\vec u)$$
- for incompressible fluids:
$$\rho \left(\frac{\partial \vec u}{\partial t} + (\vec u \cdot\vec\nabla) \vec u \right) = - \vec\nabla P - \rho g \hat k  + \mu \nabla^{2} \vec u $$
- $(\vec u \cdot \vec\nabla) \vec u$ is called the **inertial term**

- the pressure equation, for adiabatic processes:
$$\frac{d}{dt}\left(\frac{P}{\rho^{\gamma}}\right) = 0$$
## simplifications
- if $\mu, \; \lambda = 0$, it is an inviscid fluid
- if $\frac{\partial }{\partial t} = 0$, it is a steady flow
- if $\vec\nabla\cdot\vec u = 0$, it is an incompressible flow, or $\rho =$ constant

