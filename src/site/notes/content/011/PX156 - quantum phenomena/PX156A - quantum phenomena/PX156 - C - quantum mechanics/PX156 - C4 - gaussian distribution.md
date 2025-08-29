---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-a-quantum-phenomena/px-156-c-quantum-mechanics/px-156-c4-gaussian-distribution/","noteIcon":"1","created":"2025-08-27T13:14:00.850+01:00","updated":"2024-11-26T20:02:02.000+00:00"}
---


- **the gaussian distribution**: 
$$a(k) = A\, \exp(-\frac{(k-k_{0})^{2}}{2\sigma^{2}})$$
	where, $\sigma=$ standard deviation
- let $k' = k-k_{0} = \Delta k:$ 
$$\begin{align*}
	f(s) = f(x-v_{g}t) &= A \int_{-\infty}^{\infty} dk' \, \exp(- \frac{k'^{2}}{2\sigma^{2}})\,\exp(ik's) \\
	&= A \int_{-\infty}^{\infty} dk' \, \exp\left(- \frac{1}{2}\left(\frac{k'}{\sigma}-is\sigma\right)^{2} - \frac{s^{2}\sigma^{2}}{2}\right) \\
	&= A \,\exp\left(- \frac{s^{2}\sigma^{2}}{2}\right)\,\sigma \int_{-\infty}^{\infty} \frac{dk'}{\sigma} \, \exp\left(- \frac{1}{2}\left(\frac{k'}{\sigma}-is\sigma\right)^{2}\right) \\
	&= A\, \exp\left(- \frac{s^{2}\sigma^{2}}{2}\right)\sigma\sqrt{2\pi} \\\\
	\therefore |f(s)|^{2}&= 2A^{2}\sigma^{2}\pi \exp(-s^{2}\sigma^{2})
\end{align*}$$
	- also a gaussian
- $s=0 \implies |f(0)|^{2}= 2A^{2}\sigma^{2}\pi$

- RMS: 
$$w^{2}= \frac{\int |a(k)|^{2}(k-k_{0})^{2}\,dk}{\int dk|a(k)|^{2}}$$
- $a(k_{0})=A$, $w=2\Delta k:$ 
$$\begin{align*}
	\frac{1}{2}A &= A\exp\left(- \frac{\Delta{k^{2}}}{2\sigma^{2}}\right) \\
	-\ln{2} &= - \frac{\Delta{k^{2}}}{2\sigma^{2}} \\
	\Delta k^{2}&= 2\sigma^{2}\ln{2},\; \sigma\sqrt{2\ln{2}} \\
	w &= 2\sigma\sqrt{2\ln{2}} \approx 23556
\end{align*})$$
- width in $x:$ 
$$w'= 2\Delta s = 2 \frac{\sqrt{\ln 2}}{\sigma}\sim \frac{1}{w}$$
$$\begin{align*}
	\omega &= \frac{\hbar k^{2}}{2m} \\
	\frac{d\omega}{dk} &= \frac{\hbar k}{m} \\\\
	v_{g} &= \frac{d}{dk}\omega(k_{0}) \\
	&= \frac{\hbar k}{m} \\
	&= \frac{p}{m}
\end{align*}$$
