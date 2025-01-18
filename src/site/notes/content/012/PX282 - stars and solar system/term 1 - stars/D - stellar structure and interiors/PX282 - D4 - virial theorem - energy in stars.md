---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-1-stars/d-stellar-structure-and-interiors/px-282-d4-virial-theorem-energy-in-stars/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-10T11:41:40.914+00:00"}
---

- the **virial theorem** relates thermal $(U)$ and gravitational potential $(\Omega):$ 
$$\Omega = -2U$$

## derivation
- considering a shell of thickness, $dr$, at a radius, $r:$ 
$$d\Omega_{shell} = - \frac{GM_{r}dm_{shell}}{r}$$
- the mass of the shell: 
$$dm_{shell} = 4 \pi r^{2} \rho \,dr $$
$$\begin{align*}
	\int_{V} d\Omega_{shell} &= - \int_{0}^{R} 4\pi r^{2} \rho \frac{GM_{r}}{r}\,dr \\
	\int_{V} \Omega\,dV &= -4\pi \int_{0}^{R} GM_{r}\rho r\,dr \tag{1}
\end{align*}$$

- from [[content/012/PX282 - stars and solar system/term 1 - stars/A - introduction/PX282 - A0 - hydrostatic equilibrium\|hydrostatic equilibrium]]: 
$$\frac{dP}{dr} = - \frac{GM_{r}\rho}{r^{2}}$$
- by volume: 
$$\begin{align*}
	\frac{4}{3}\pi r^{3} \frac{dP}{dr} &= - \frac{4}{3}\pi r^{3} \frac{GM_{r}\rho}{r^{2}} \\
	4\pi \int_{0}^{R }r^{3} \frac{dP}{dr} dr  &= -4\pi \int_{0}^{R }GM_{r}\rho r\,dr \tag{2}
\end{align*}$$

- equations $(1)$ and $(2)$ have the same $RHS$
- using integration by parts on the $LHS$ of equation $(2):$ 
$$\begin{gather}
	4\pi \left[P r^{3} - 3 \int Pr^{2}\,dr \right]_{0}^{R} 
	= 4\pi \left(0 - 3\int_{0}^{R} Pr^{2}\,dr \right) && [\because P(r=R) = 0] \\
	= -3\int P\,dV
\end{gather}$$
$$\therefore \int_{V}\Omega\,dV = - 3\int P\,dV \implies \Omega = -3P$$
- considering thermal energy from the equations of state: 
$$P = nk_{B}T\;;\; U  = \frac{3}{2}k_{B}T \; (\text{per particle})$$
- for $n$ particles: 
$$U = \frac{3}{2}nk_{B}T  = \frac{3}{2}P$$
- therefore the **virial theorem** is obtained: 
$$\therefore \Omega = -2U$$
- the total energy of a star: 
$$E = \Omega+U $$
- using the virial theorem: 
$$E = -U = \frac{\Omega}{2}$$
- $U$ cannot be negative $\implies E<0:$ star is gravitationally bound

## relativistic case
- for a relativistic gas, $P \neq n k_{B} T$, so: $\Omega = -U$ and $E=0$
- if $E$ increases (ie: from nuclear fusion): 
	- $\Omega$ increases, and star expands 
	- $U$ decreases, and temperature drops
	- if the temperature drops, the fusion decreases, therefore it is self-regulating
- if $E$ decreases (ie: from radiation): 
	- $\Omega$ decreases, and star gets smaller
	- $U$ increases, and temperature increases
	- again, it is self-regulating
- self-regulation does not apply to degenerate matter
