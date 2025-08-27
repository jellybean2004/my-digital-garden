---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/b-variational-principles/px-285-b1-variational-principles/","noteIcon":"1","created":"2025-08-27T13:14:16.098+01:00","updated":"2024-12-09T10:31:05.000+00:00"}
---

- allows quantities such as path lengths, and functions to be extremized 

![Pasted image 20241209103049.png|500](/img/user/pics/Pasted%20image%2020241209103049.png)

- considering a person taking different paths through strips of tarmac, beach and sea
- the time taken is: 
$$\tau = \sum\limits \frac{\text{distances}}{\text{velocities}}$$
## variational principles in physics:
- **optics**: fermat's law, $l(x)$ is extremal
- **waves**: destructive interference is small for paths that interfere constructively (ie: are at the same phase), such that their phase difference is minimized
- **relativity:** trajectories in free space, in a gravitational field for general relativity, are those that extremize (maximize here) elapsed proper time: 
$$\tau = \int_{t_{1}}^{t_{2}} \frac{dt}{\gamma} = \int dt\sqrt{1- \frac{v^{2}}{c^{2}}}$$
	- classical paths in flat space minimize velocity
	- straight line paths give lower velocities, and hence higher values of $\tau$
- **newtonian mechanics:** trajectories extremize the action
- **electromagnetism:** 
$$L = \frac{1}{2} \int dV \left(\epsilon_{0}E^{2}- \frac{1}{\mu_{0}} B^{2}\right)$$
- **path integrals:**
	- **quantum mechanics:** (non-examinable) 
	$$\psi(x,t) = \sum\limits_{paths} \exp\left(\frac{1}{\hbar}\int_{t_{0}}^{t_{1}} L\,dt\right)$$
	- equivalent to finding the solutions of schrödinger's equation
	- $\exp(i\phi)$ is a quantum mechanical phase, with phase angle 
	$$\phi = \frac{1}{\hbar} A = \frac{1}{\hbar} \int_{t_{0}}^{t_{1}} L\,dt$$
	- paths, $x(t)$, that minimize the action are paths for which the quantum mechanical phase is nearly the same for nearby paths $\implies$ constructive interference
	- in the limit of macroscopic particles, $N\sim10^{20}\,T$, interference is very strong $implies$ only this 'classical' trajectory is realized
