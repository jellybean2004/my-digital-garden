---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h3-mechanical-perspective-of-fluids/","noteIcon":"1","created":"2025-01-09T14:42:19.537+00:00","updated":"2025-02-27T12:59:22.256+00:00"}
---

- fluid is a substance which **cannot resist shear force without motion**, and **does not return to its initial state** when stress is removed

- **stress** can be defined similar to pressure, ie. force per unit area:
$$\tau = \frac{F}{A}$$
- considering a brick fixed on a surface, $x=0$, and an external force, $\vec F$ is applied to it
- the stress deforms this solid object, where $X$ is the deformation due to the stress

![PX285 - H3 - mechanical perspective of fluids.png|500](/img/user/pics/PX285%20-%20H3%20-%20mechanical%20perspective%20of%20fluids.png)

- defining **strain**, $e$:
$$\tau_{solid} = G e$$
	where, $G$ is a coefficient determined by the *binding forces* between molecules

- in a fluid, there are no *binding forces*, and the strain, caused by stress, builds up in time

![PX285 - H3 - mechanical perspective of fluids-1.png|500](/img/user/pics/PX285%20-%20H3%20-%20mechanical%20perspective%20of%20fluids-1.png)

- therefore, in fluids,
$$\tau_{fuild} = \mu \frac{de}{dt}$$
	where, $\mu$, the coefficient of proportionality is the viscosity

$$e = \frac{dX}{dy}$$
$$\tau_{fluid} = \mu \frac{d}{dt}\left(\frac{\partial X}{\partial y}\right) = \mu \frac{\partial }{\partial y}\left(\frac{dX}{dt}\right) = \mu \frac{\partial u_{x}}{\partial y}$$
	where, $\cfrac{dX}{dt} = u_{x}$ is the horizontal velocity
- in summary, as a response to shear forces, **a solid deforms whereas a fluid flows**

- the relaxation time indicates how quickly the stress adjusts to the new sheared state
- initially, ${} t' < t < t_{rel}$, the stress is like in a solid
- then, for $t>t_{rel}$, the fluid starts to flow, and the stress relaxes into a new sheared state
