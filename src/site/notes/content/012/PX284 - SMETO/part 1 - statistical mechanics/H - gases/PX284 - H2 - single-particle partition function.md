---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/h-gases/px-284-h2-single-particle-partition-function/","noteIcon":"1","created":"2025-08-27T13:15:24.633+01:00","updated":"2025-04-22T10:34:25.000+01:00"}
---

- the sum is now written as an integral:
$$Z_{1} = \int_{0}^{\infty} e^{-\beta E(k)}g(k)\,dk$$
	where, $e^{-\beta E(k)}$ is the boltzmann factor, and ${} g(k)$ is DOS

- for a particle with a wavevector, $k$, and mass, $m$, the momentum, $p = \hbar k$, and the energy, $E \left(=\cfrac{p^{2}}{2m}\right)  = \cfrac{\hbar^{2}k^{2}}{2m}$

- so,
$$Z = \int_{0}^{\infty}\exp\left( -\beta \frac{\hbar^{2}k^{2}}{2m} \right) \frac{Vk^{2}}{2\pi^{2}} \,dk$$
- using the standard integral:
$$\int_{\infty}^{\infty} x^{2}e^{-\alpha x^{2}} dx = \frac{1}{2}\sqrt{\frac{\pi}{\alpha^{3}}}$$ 
$$\begin{align*}
Z &= V \left(\frac{mk_{B}T}{2\pi \hbar^{2}}\right)^{3/2} \\
&= Vn_{Q} \\
&= \frac{V}{\lambda_{th}^{3}}
\end{align*}$$
	where, 
		$n_{Q} = \left(\cfrac{mk_{B}T}{2\pi\hbar^{2}}\right)^{3/2}$ is the **quantum concentration**,
		$\lambda_{th} = \cfrac{h}{\sqrt{2\pi mk_{B}T}}$  is the **thermal wavelength**

- $\lambda_{th}$ is the de broglie wavelength of a particle at temperature, $T$, ie. it is the characteristic size of the particle's wavefunction
- $n_{Q} = \cfrac{1}{\lambda_{th}^{3}}$ is the concentration at which the particles are separated by $\lambda_{th}$

- if the actual concentration, $n \ll n_{Q}$, the particles are dilute with no wavefunction overlap, and there are no quantum effects
- this is known as a **'classical gas'**

- if $n \gg n_{Q}$, the particles are concentrated, there are wavefunction overlaps, giving rise to quantum effects
- this is known as a **'quantum gas'**

- eg: H$_{2}$ molecule at RTP
	- $n_{Q} \simeq 10^{30}$ m$^{-3}$
	- $n \simeq 10^{25}$ m$^{-3}$
	- no overlap, so classical

- eg: electrons in a metal at $300$ K
	- $n_{Q} \simeq 10^{25}$ m$^{-3}$
	- $n \simeq 10^{29}$ m$^{-3}$
	- significant overlap, so quantum
