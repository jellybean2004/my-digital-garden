---
dg-publish: true
---

- virial theorem relates thermal $(U)$ and gravitational potential $(\Omega):$ 
$$\Omega = -2U$$
{ #b7947e}

- considering a shell of thickness, $dr$, at a radius, $r:$ 
$$d\Omega_{shell} = - \frac{GM_{r}dm_{shell}}{r}$$
- from previous notes: 
$$dm_{shell} = 4 \pi r^{2} \rho \,dr $$
$$\begin{align*}
	\int_{V} d\Omega_{shell} &= - \int_{0}^{R} 4\pi r^{2} \rho \frac{GM_{r}}{r}\,dr \\
	\int_{V} \Omega\,dV &= -4\pi \int_{0}^{R} GM_{r}\rho r\,dr \tag{1}
\end{align*}$$
- *hydrostatic equilibrium*: 
$$dP = - \frac{GM_{r}\rho}{r^{2}}$$
- by volume: 
$$\begin{align*}
	\frac{4}{3}\pi r^{3} \frac{dP}{dr} &= - \frac{4}{3}\pi r^{3} \frac{GM_{r}\rho}{r^{2}} \\
	4\pi \int_{0}^{R }r^{3} \frac{dP}{dr} dr  &= -4\pi \int_{0}^{R }GM_{r}\rho r\,dr \tag{2}
\end{align*}$$
- equations $(1)$ and $(2)$ have the same $RHS$
- using integration by parts on the $LHS$ of $(2):$ 
$$\begin{gather}
	4\pi \left[P r^{3} - 3 \int Pr^{2}\,dr \right]_{0}^{R} \\
	= 4\pi \left(0 - 3\int_{0}^{R} Pr^{2}\,dr \right) && [\because P(r=R) = 0] \\
	= -3\int P\,dV
\end{gather}$$
$$\therefore \int_{V}\Omega\,dV = - 3\int P\,dV \implies \Omega = -3P$$
- considering thermal energy from the equations of state: 
$$P = nk_{B}T\;;\; U  = \frac{3}{2}k_{B}T \; (\text{per particle})$$
- for $n$ particles: 
$$U = \frac{3}{2}nk_{B}T  = \frac{3}{2}P$$
- therefore the virial theorem is obtained: 
$$\therefore \Omega = -2U$$
- the total energy of a star: 
$$E = \Omega+U $$
- with the virial theorem: 
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
