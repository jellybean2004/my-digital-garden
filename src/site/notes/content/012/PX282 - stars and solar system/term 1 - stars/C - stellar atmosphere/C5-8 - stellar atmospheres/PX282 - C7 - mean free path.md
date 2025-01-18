---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-1-stars/c-stellar-atmosphere/c5-8-stellar-atmospheres/px-282-c7-mean-free-path/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-22T12:55:13.576+00:00"}
---

- the [[content/012/PX282 - stars and solar system/term 1 - stars/C - stellar atmosphere/C5-8 - stellar atmospheres/PX282 - C6b - intensity after absorption\|intensity after absorption]] is given by:
$${\frac{I_{\lambda}}{I_{\lambda,0}} = \exp\left(-\int_{0}^{z} \kappa_{\lambda} \rho\,dz\right)}$$
- using this to define the **mean free path** for a photon, $l$, which is the characteristic distance a photon travels: 
$$\begin{gather}
l = \frac{1}{\kappa_{\lambda}\rho} \\\\
\implies \frac{I_{\lambda}}{I_{\lambda,0}} = e^{-1} \\ 
\end{gather}$$

- taking a typical stellar opacity, $\kappa\sim0.1\,m^{2}kg^{-1}$, and density, $\rho\sim 1.5\times10^{5}\,kg\,m^{-3}$ (core), $\sim 1.4\times10^{3}\,kg\,m^{-3}$ (average), $\sim 10^{-6}\,kg\,m^{-3}$ (photosphere), gives the mean free paths:

| mean free path     |            |          value           |
| ------------------ | ---------- | :----------------------: |
| in the core        | $l_{core}$ | $\sim 7\times10^{-5}\,m$ |
| average            | $l_{avg}$  | $\sim 7\times10^{-3}\,m$ |
| in the photosphere | $l_{ps}$   |     $\sim 10^{7}\,m$     |
- therefore, photons observed come from the photosphere
## example
- calculating the absorption coefficient for ozone
- taking a $9.5\,\mu m$ line of ozone $(z)$, with $\sim30\%$ transmission, ie:
$$\frac{I}{I_{0}}= e^{-\kappa\rho z} = 0.3 \implies k\rho z \approx 1.2$$
- considering the density, $\rho(\text{O}_{3}) = 0.3~$ppm, and assuming it is all in the stratosphere $(0-50\,km)$ 
- the mass in the air column is $\simeq 6.4\times10^{-3}\,kg\,m^{-2}$
- the average density of ozone $\simeq 1.3\times10^{-7}\,kg\,m^{-3}$
- therefore, the absorption coefficient is: 
$$\kappa \approx 185\,m^{2}kg^{-1}$$
