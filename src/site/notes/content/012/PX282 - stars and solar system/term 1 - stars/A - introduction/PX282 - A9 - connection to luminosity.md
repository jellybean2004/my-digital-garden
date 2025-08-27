---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-1-stars/a-introduction/px-282-a9-connection-to-luminosity/","noteIcon":"1","created":"2025-08-27T13:14:15.742+01:00","updated":"2024-11-26T09:33:55.000+00:00"}
---

- luminosity is the total energy emitted: 
$$\begin{align*}
	L &= \int d\Omega \int_{star} dA \int_{0}^{\infty}B_{\lambda}\,d\lambda \\
	&= \int_{0}^{2\pi} \int_{0}^{\pi} \cos\theta\, \sin\theta\, d\theta\, d\phi\, \left(4\pi R_{*}^{2}\right) \left(\sigma \frac{T^{4}}	{\pi}\right)
\end{align*}$$
	where, 
		$d\Omega = \sin\theta\, d\theta\, d\phi$ ,
		$\int_{star} dA = 4\pi R_{*}^{2}$ ,
		$\int_{0}^{\infty}B_{\lambda}\,d\lambda  = \left(\sigma \frac{T^{4}}{\pi}\right)$
	- $\cos\theta$ arises from the angular profile of the emitting area
- only looking at light coming out of the star limits in $\theta$ half: 
$$\begin{align*}
	L &= 2\pi \left[- \frac{1}{2}\cos^{2}\theta\right]_{0}^{\frac{\pi}{2}} 4 R_{*}^{2}\sigma T^{4} \\\\
	\therefore L &= 4\,\pi \, R_{*}^{2}\,\sigma\, T_{eff}^{4}
\end{align*}$$
- this is the luminosity-radius-temperature relation of a star
- the flux: 
$$f = \sigma T_{eff}^{4}$$
- **notes:**
	- $T^{4}$ makes errors inflate rapidly
	- real spectra are not perfect blackbodies
	- $T_{eff}$ is very effective for classifying stars
