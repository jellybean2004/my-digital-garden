---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-the-solar-system/c-stellar-atmosphere/c10-13-radiative-transfer/px-282-c12-temperature-structure/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-22T16:32:36.664+00:00"}
---

- the [[content/012/PX282 - stars and the solar system/C - stellar atmosphere/C10-13 -  radiative transfer/PX282 - C11 - radiation pressure\|radiation pressure]]: 
$$P_{rad}= \frac{4\pi}{3c}\langle{I}\rangle$$
- this concept of $P_{rad}$ can be linked to the flux, $F$, to relate $T$ with $z$ and $\tau$

- considering a small block of material with flux coming out of a star
- the block has a thickness. $dz$
- $P_{rad}(z)$ and $P_{rad}(z+dz)$ on the surfaces
- incoming flux: $F$, outgoing flux: $F-dF$
- over a distance, $z$:
	- $F$ decreases
	- $P_{rad}$ decreases
- the change in $P_{rad}$ can be related to the change in $F$
- for the photon: $E=pc$ and $F = \frac{dE}{dt}$ 
$$\frac{dp}{dt}= \frac{dF}{c} = Force$$
- the force, ie: the difference in $P_{rad}$, is: $Force = \frac{dP_{rad}}{dz}\,dz$: 
$$\frac{dP_{rad}}{dz}dz = \frac{1}{c}dF$$

- considering only absorption for the change in $F:$ 
$$\frac{dF}{F}= -\rho\kappa\,dz$$
 where, $\frac{dI}{dz}= -\rho\kappa I$, and $F = \int I\cos\theta\,d\Omega$
$$\frac{dP_{rad}}{dz}dz = - \frac{1}{c}F\rho\kappa\,dz$$
$$\frac{dP_{rad}}{d\tau} = \frac{F}{c}$$
- integrating: 
$$P_{rad} = \frac{1}{c}F\tau+A$$
	- where, $A$ is the constant of integration
$$\frac{4\pi}{3c}\langle{I}\rangle = \frac{1}{c}F\tau + A$$
- solving for $T$ structure near the surface
- using boundary conditions:
	- at the top of the atmosphere: $\tau=0$, $\langle{I}\rangle = \frac{I_{out}}{2}$ (no $I$  heading inwards)
$$\frac{2\pi I_{out}}{3c} = A = \frac{2F}{3c}$$
$$\therefore \frac{4\pi}{3c} \langle{I}\rangle= \frac{F\tau}{c} + \frac{2F}{3c}$$
$$\frac{4\pi}{3}\langle{I}\rangle = F\left(\tau+\frac{2}{3}\right)$$
- near the surface (photosphere): 
	$F = \sigma T_{eff}^{4}$
	$\langle{I}\rangle = S = B = \frac{\sigma T^{4}}{\pi}$
$$\frac{4\pi}{3}B = \sigma T_{eff}^{4} \left(\tau + \frac{2}{3}\right)$$
$$\therefore T^{4} = \frac{3}{4} T_{eff}^{4}\left(\tau + \frac{2}{3}\right)$$
- **key points:**
	- $T = T_{eff}$ when $\tau=\frac{2}{3}$
	- the 'surface' that is seen is at $\tau \approx \frac{2}{3}$
