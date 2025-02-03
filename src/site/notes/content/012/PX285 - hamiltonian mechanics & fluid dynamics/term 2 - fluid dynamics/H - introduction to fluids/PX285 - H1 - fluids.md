---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h1-fluids/","noteIcon":"1","created":"2025-01-09T14:14:03.983+00:00","updated":"2025-02-01T16:04:04.376+00:00"}
---

## definition
- fundamentally, fluid is a substance which fills up a vessel with no fixed shape
- the molecules in a fluid are not fixed in a lattice like in solids, and they are able to move freely relative to each other
## methods of describing fluids
### considering every molecule
- each molecule has a velocity, $\vec v_{i}$
- kinematic equations from the newton's second law give the trajectories of the molecules
- it works if there are a small number of molecules
### kinetic approach
- using a distribution function, $f(\vec r, \vec v, t)$, that gives the **number of molecules at a certain location** (a sufficiently small volume)  with a **certain velocity** (a small interval of velocities) at a **certain time**
- the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/C - entropy and temperature/PX284 - C3 - boltzmann distribution\|boltzmann equation]] such a function, but it is a 7D problem
### continuous matter approach - fluid/hydro-dynamics
- introducing density:
$$\rho = \frac{m}{V}$$
- more rigorously:
$$\rho = \lim_{\Delta V \to 0} \frac{\Delta m}{\Delta V}$$
- from quantum mechanics, it is known that $\Delta V$ cannot approach 0
- as ${} \Delta V \to 0$, there are fluctuations below a certain volume, $\Delta V^{*}$, in $\rho$ due to discrete nature

![PX285 - H1 - fluids.png|500](/img/user/pics/PX285%20-%20H1%20-%20fluids.png)

- for water, air, etc, in atmospheric pressure, $(\Delta V^{*})^{1/3} \simeq 10^{-9}$ mm
- for scales smaller than $10^{-9}$ mm, fluid mechanics works

- defining the **knudsen number**:
$$k_{n} \equiv \frac{\lambda}{L}$$
	where, $\lambda$  is the mean free path, and $L$ is the size of the system of interest
- **mean free path** is the average distance that a molecule travels between two collisions

- if $k_{n}\ll 1$, fluid approach is justified 

- at atmospheric pressure, $\lambda \simeq 0.1\,\mu$m
- at $100$ km height above the ground, $\lambda \simeq 1$ cm
