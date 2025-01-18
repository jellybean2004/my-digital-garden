---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h7-quantifying-the-effects-of-viscousity/","noteIcon":"1","created":"2025-01-17T12:34:59.151+00:00","updated":"2025-01-17T14:09:43.247+00:00"}
---

- the stress:
$$\tau = \mu \frac{\partial u_{x}}{\partial y}$$
- it is expressed in the units of pressure
#review
$$[\tau] = \frac{[\mu][L]}{[T^{2}][L^{2}]} = \frac{[M]}{[T][L]} $$
$$[\mu] = [M][L]^{-1}[T]^{-1}$$
- typical scales in a fluid:
	- density: $\rho_{0} = [M]/[L]^{3}$
	- characteristic speed: $u_{0}= [L]/[T]$
	- characteristic spatial scale: $L_{0} = [L]$

- constructing a combination of those typical scales of the same dimensions as viscosity:
$$\rho_{0}u_{0}L_{0} \sim \mu$$
- to assess whether $mu$ is big or small, compare it with $\rho_{0}u_{0}L_{0}$ in a specific problem
- $\rho_{0}u_{0}L_{0}/\mu$ is a dimensionless quantity
- if the fraction is big, ${} \mu$ can be neglected

- **reynold's number:**
$$R_{e} = \frac{\rho_{0}u_{0}L_{0}}{\mu}$$
- a small $R_{e}$ means the flow is viscous dominant (laminar)
- a large $R_{e}$ means the flow is turbulent
- specific values of $R_{e}$ comes from experiments

- **note:** this estimation is rough

- eg: 
	- in the flow in a cylinder, $L_{0}$ could be either $a$ or $2a$
	- furthermore, $u_0$ could be the ${} u_{max} {}$, or $u_{max}/2$, or the average speed $\langle{u}\rangle$

$$\langle{u}\rangle = \frac{1}{\pi a^{2}} \int_{0}^{2\pi} \int_{0}^{a} u_{z}(r) \,r\, dr\,d\phi = \frac{Qa^{2}}{a\mu}$$
$$R_{e}= \frac{Qd_{0}^{3}\rho_{0}}{32\mu^{2}}$$
- flows in this case are laminar, $R_{e} < 3200$

- a pipe of $5$ cm in diameter, $\rho_{water} = 10^{3}$ kg m$^{-3}$, $\mu_{water} = 10^{-3}$ N s m$^{-2}$
	- $u_{0}\approx 5$ cm s$^{-1}$ is the threshold
	- if $u>u_{0}$, the flow is turbulent
	- if $u < u_{0}$, the flow is laminar

