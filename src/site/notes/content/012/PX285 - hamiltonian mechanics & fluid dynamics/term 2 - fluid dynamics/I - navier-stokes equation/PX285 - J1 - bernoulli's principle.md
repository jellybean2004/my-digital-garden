---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-j1-bernoulli-s-principle/","noteIcon":"1","created":"2025-01-24T12:51:54.480+00:00","updated":"2025-01-31T12:30:34.221+00:00"}
---

- considering a stream lined flow, with $A_{1}$ and $A_{2}$ as the cross-sectional areas of the flow tube

![PX285 - I3 - bernoulli's principle-1.png|500](/img/user/pics/PX285%20-%20I3%20-%20bernoulli's%20principle-1.png) 

- the rate at which the fluid enters region 1: $\rho_{1}A_{1}u_{1}$
- the rate at which work is done on fluid by the pushing from behind (left to right in the sketch): $W = Fd$, where $d = u/t$
- For unit time: $P_{1}A_{1}u_{1}$
- the rate at which kinetic energy of the fluid enters region 1: $\rho_{1} (u_{1}^{2}/2 )A_{1}u_{1}$
- and likewise, the gravitational potential energy: $\rho_{1} A_{1} u_{1} g z_{1}$

- the expressions for region 2 will be identical

- from conservation of mass, if flow is incompressible:
$$\rho_{1} A_{1}u_{1} = \rho_{2}A_{2}u_{2}$$
- considering a constant internal energy, ie. no friction, so the flow is inviscid

- conservation of energy:
$$\rho A_{1}u_{1} \left(\frac{u_{1}^{2}}{2} + gz_{1} + \frac{P_{1}}{\rho}\right) = \rho A_{2}u_{2} \left(\frac{u_{2}^{2}}{2} + gz_{2} + \frac{P_{2}}{\rho}\right)$$
- therefore, the invariant of the flow along a stream line:
$$\rho \frac{u^{2}}{2} + \rho g z + P = \text{constant}$$
- this is called **bernoulli's principle**
- this requires: 
	- incompressible, ie: $\vec\nabla\cdot\vec u = 0$
	- inviscid, ie: $\mu=0$
	- steady, ie: $\frac{\partial }{\partial t} = 0$

## from navier-stokes equation

$$\begin{align*}
\rho ( \vec u \cdot \vec\nabla) \vec u &= - \vec\nabla P- \rho g \hbar k \\
\rho g\hat k &= \vec\nabla(\rho g z) \\
\rho (\vec u \cdot \vec\nabla)\vec u &= -\vec\nabla (P + \rho gz)
\end{align*}$$

- projecting the NS equation on a streamline:
$$\begin{gather}
\rho \vec u \cdot (\vec u \cdot \vec\nabla )\vec u = - \vec u \cdot \vec\nabla (P = \rho gz) \\
\vec u \cdot \vec\nabla  \left( P + \rho gz + \rho \frac{u^{2}}{2}\right)= 0 \\
P + \rho gz + \rho \frac{u^{2}}{2} = \text{ constant}
\end{gather}$$
	where $(\vec u \cdot \vec\nabla) \vec u = \vec\nabla u^{2}/2$


- eg: **hydrostatic limit**
- bernoulli's principle can be applied between any two points in the fluid:
$$P + \rho gz = \text{constant}$$
- considering an object submerged in water
- the depth of water is $z_{1}$
- air above the water exerts atmospheric pressure, $P_{atm}$
- from bernoulli's principle:
$$P(z) = P_{atm} + \rho g (z_{1}- z)$$
- the total upward force on the object, which is the projection of the force on the z-axis
$$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}
\vec F \cdot \hat k = - \oiint_{S} P(z) \hat k \cdot d\vec s = - \iiint_{V} \vec\nabla\cdot ( P(z) \hat k) \, dV$$
	where, $S$ is the surface of the object, and $d\vec s$ is pointed outwards; $V$ is the volume of the object
- using bernoulli's principle:
$$\iiint \vec\nabla \cdot (\rho gz \hat k ) dV = \iiint_{V}\rho g \, dV = g \iiint_{V}\rho\, dV = Mg$$
- therefore the vertical force is the weight of the fluid if it fills up the object
- this is **archimedes' principle**
