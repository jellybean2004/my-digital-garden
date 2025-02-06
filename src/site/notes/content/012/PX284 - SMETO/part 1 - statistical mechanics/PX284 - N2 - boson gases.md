---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/px-284-n2-boson-gases/","noteIcon":"1","created":"2025-02-06T15:22:47.225+00:00","updated":"2025-02-06T15:33:11.387+00:00"}
---

## photon gas
- massless bosons
- $\mu = 0$, $s = 1\implies 2s+1 = 3$ , but one of those states is forbidden
$$\begin{gather}
E = \hbar \omega \\
\omega = ck \\
g(\omega )\,d\omega = 2 \frac{V\omega^{2}}{2\pi^{2} c^{3}}\,d\omega \\
U = \int_{0}^{\infty} \hbar\omega g(\omega ) f_{BE}(\omega)\,d\omega = \int_{0}^{\infty} \frac{\hbar V}{\pi^{2}c^{3}} \frac{\omega^{3}}{\exp(\beta\hbar\omega)-1}\,d\omega
\end{gather}$$

## phonon gas
- massless, spinless boson
- $\mu = 0$, $2s+1 = 1$ and $\omega = v_{s}q$
$$\begin{gather}
g(\omega)\,d\omega = 3 \times \frac{V\omega^{2}}{2\pi^{2}v_{s}^{3}} \, d\omega  \\
U = \int_{0}^{\infty} \frac{9N\hbar}{\omega_{D}^{3}} \frac{\omega^{3}}{\exp(\beta\hbar\omega)-1} \,d\omega \\
\omega_{D} = \left(\frac{6N\pi^{2}v_{s}^{3}}{V}\right)^{1/3}
\end{gather}$$
## general massive boson gas in 3D

$$N = \int_{0}^{\infty} (2s+1) \frac{V}{(2\pi)^{2}} \left(\frac{2m}{\hbar}\right)^{3/2}\frac{E^{1/2}}{\exp(\beta(E-\mu))-1}\,dE$$
where, $\mu<0$
- this integral is hard, but doable
