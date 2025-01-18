---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-1-stars/c-stellar-atmosphere/c10-13-radiative-transfer/px-282-c10b-understanding-the-radiative-transfer-equation/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-22T21:35:46.028+00:00"}
---

- the radiative transfer equation (RTE): 
$$\frac{dI_{\lambda}}{d\tau_{\lambda}} = I_{\lambda}- S_{\lambda}$$
## local thermal equilibrium (LTE)
- LTE implies that in a region, the temperature is effectively constant, and the velocities of particles follow [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C7 - maxwell-boltzmann distribution\|the maxwell-boltzmann distribution]]

- at LTE, the photon mean free path is small, and they interact with particles, so, any optically thick object with a non-zero temperature emits blackbody radiation
- hence, LTE equates to blackbody radiation, therefore the source function equals the planck function: 
$$S_{\lambda} = B_{\lambda}$$
- in equilibrium, the absorption and the emission are equal, so the flux is constant, ie: $F = \sigma T^{4}$

- using LTE, RTE becomes analytically solvable

- considering an isothermal slab with its top surface at optical depth, $\tau = 0$, and its bottom surface at $\tau'$, such that $I(\tau') = 0$
- using LTE: 
$$\frac{dI_{\lambda}}{d\tau_{\lambda}} = I_{\lambda}- S_{\lambda}=  I_{\lambda}- B_{\lambda}$$
- multiplying by $e^{-\tau}:$ 
$$\begin{gather*}
	\frac{dI_{\lambda}}{d\tau_{\lambda}} e^{-\tau} = (I_{\lambda}- B_{\lambda}) e^{-\tau} \\
	\frac{dI_{\lambda}}{d\tau} e^{-\tau} - I_{\lambda}e^{-\tau} = \frac{d}{d\tau}(I_{\lambda} e^{-\tau}) = -Be^{-\tau}\\
	[I_{\lambda} e^{-\tau}]_{\tau'}^{0} =  -\int_{o}^{\tau'} Be^{-\tau}\,d\tau \\
	\therefore I(0) = -B [e^{-\tau}]_{0}^{\tau'}  = B(1-e^{-\tau'})
 \end{gather*}$$
- for a dense gas, $\tau'$ is large, so $I(0)\to B$ 
- this explains the emission lines as hot gases are not dense enough for pure blackbodies
- absorption lines: dense blackbody emitter, with cold gas in front of it
