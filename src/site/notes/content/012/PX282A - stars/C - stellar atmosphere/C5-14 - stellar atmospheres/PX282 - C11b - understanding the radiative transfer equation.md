---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/c-stellar-atmosphere/c5-14-stellar-atmospheres/px-282-c11b-understanding-the-radiative-transfer-equation/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:38:56.333+00:00"}
---

- the radiative transfer equation (RTE): 
$$\frac{dI_{\lambda}}{d\tau_{\lambda}} = I_{\lambda}- S_{\lambda}$$
## local thermal equilibrium (LTE)
- LTE implies that in a region, the temperature is effectively constant, and the velocity distribution of particles follows [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C7 - maxwell-boltzmann distribution\|the maxwell-boltzmann distribution]]
- the photons mean free path is small, and they interact with particles
- any optically thick object with a non-zero temperature emits blackbody radiation
- hence, LTE equates to blackbody radiation and: 
$$S=B$$
	where, $B$ is the planck function
- in equilibrium, the absorption and the emission are equal: 
$$\implies F = constant = \sigma T^{4}$$
- using LTE, the RTE becomes analytically solvable

- consider an isothermal slab, with the top surface at $\tau = 0$, and the bottom surface at $\tau'$
- using LTE: 
$$\frac{dI_{\lambda}}{d\tau_{\lambda}} = I_{\lambda}- B_{\lambda}$$
- multiplying by $e^{-\tau}:$ 
$$\begin{align*}
	\frac{dI_{\lambda}}{d\tau_{\lambda}} e^{-\tau} &= (I_{\lambda}- S_{\lambda}) e^{-\tau} \\
	\frac{d}{d\tau}(I_{\lambda} e^{-\tau}) &= \frac{dI_{\lambda}}{d\tau} e^{-\tau} - I_{\lambda}e^{-\tau} = -Be^{-\tau}\\
	[I_{\lambda} e^{-\tau}]_{\tau'}^{0} &=  -\int_{o}^{\tau'} Be^{-\tau}\,d\tau \\
	I(0) - I(\tau') e^{-\tau'} &= -B [e^{-\tau}]_{0}^{\tau'} \\
	\therefore I(0) &= B(1-e^{-\tau'})
 \end{align*}$$
- for a dense gas, $\tau'$ is large, so $I(0)\to B$ 
- this explains the emission lines as hot gases are not dense enough for pure blackbodies
- absorption lines: dense blackbody emitter, with cold gas in front of it
