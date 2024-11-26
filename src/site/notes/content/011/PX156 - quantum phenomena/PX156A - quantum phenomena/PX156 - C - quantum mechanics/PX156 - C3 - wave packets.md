---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-a-quantum-phenomena/px-156-c-quantum-mechanics/px-156-c3-wave-packets/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T20:02:01.133+00:00"}
---


## idea
- consider two plane waves:
	$\psi_{1}= A\exp (ikx-i\omega(-k)t)$
	$\psi_{2}= A\exp -(ikx-i\omega(-k)t)$
	$$\hbar \omega(-k) = \frac{\hbar^{2}k^{2}}{2m}= h \omega(k) \implies \omega(k)=\omega(-k)$$
	$$\begin{align*}
		\psi &= \psi_{1}+\psi_{2} \\
		&= A\exp(-i\omega(k)t) (\exp(ikx)+ \exp(-ikx)) \\
		&= 2A \exp(-i\omega(k)t)\cos(kx)
		\end{align*}$$
	- standing wave  with amplitude, $2A\cos(kx)$
	$$|\psi|^{2} = 4A^{2}\cos^{2}(kx) = 2A^{2}(1+\cos(2kx))$$

- consider two plane waves:
	$\psi_{1}= A\exp (ikx-i\omega(k_{1})t)$
	$\psi_{2}= A\exp -(ikx-i\omega(k_{2})t)$
	
	$\psi = \psi_{1}+\psi_{2}$
	- choosing $k_{1}= k_{0}+\Delta k$, $k_{2}= k_{0}-\Delta k$, $\Delta k << k_{0}$
	- expanding $\omega(k_{1})$ and $\omega(k_{2})$ as a [[content/011/PX153 - mathematics for physicists/term 1/PX153 - F - series/PX153 - F1 - taylor series\|taylor series]]:
		$\omega(k_{1})\approx \omega(k_{0}) +\Delta k \frac{d\omega(k_{0})}{dk}+\dots = \omega_{0} + \Delta k\, \omega_{0}' + \dots$
		$\omega(k_{2})\approx \omega(k_{0}) -\Delta k \frac{d\omega(k_{0})}{dk}+\dots  = \omega_{0} - \Delta k\, \omega_{0}' + \dots$
	$$\begin{align*}
		\psi &= A \exp(i(k_{0}x-\omega_{0}t + \Delta kx - \Delta k \omega_{0}'t)) + A \exp(i(k_{0}x-\omega_{0}t - \Delta kx + \Delta k \omega_{0}'t)) \\
		&= A \exp(i(k_{0}x-\omega_{0}t)) ( \exp(i\Delta k(x-\omega_{0}'t)) + \exp(-i\Delta k(x-\omega_{0}'t))) \\
		&= 2A \exp(i(k_{0}x-\omega_{0}t)) \cos (\Delta k (x-\omega_{0}'t)) \\\\
		|\psi|^{2} &= 4 A^{2} \exp(i(k_{0}x-\omega_{0}t)) (1+ \cos(2\Delta k(x-\omega_{0}'t)))
	\end{align*}$$
	- this is a travelling wave, moving at speed, $v_{g}= \omega_{0}'$
		- $\frac{d\omega}{dk}= \omega' =$ group velocity
	- $\hbar \omega(k) = \frac{\hbar^{2}k^{2}}{2m}$, and $\omega' = \frac{d}{dk}\left(\frac{\hbar k^{2}}{2m}\right)= \frac{\hbar k}{m}$ 
	- $\omega_{0}' = \frac{\hbar k_{0}}{m} = \frac{p_{0}}{m}$

	$$\int_{-\infty}^{+\infty} |\psi|^{2}\,dx = \int_{-\infty}^{+\infty} A^{2}\,dx = \infty \neq 1 \;unless\; A\equiv 0$$
	- consider a box of size $\pm L:$ $$\int_{-L}^{+L} A^{2}\,dx = 2LA^{2}= 1 \implies A= \frac{1}{\sqrt{2L}}$$
## a particle as a wave packet
- super position of many plane waves with wave numbers grouped around an average value, $k_{0}:$ 
$$\psi = \int dk\, a(k)\exp(ikx-i\omega(k)t)$$
	- where, $a(k)$ is the $k$-dependent amplitude
- a particle is represented by a combination that is grouped around a particular wavenumber, $k_{0}$, with gaussian distribution of amplitudes of waves around $k_0$

- $\omega<<k_{0}:$ 
$$\omega(k) \approx \omega(k_{0}) + \omega_{0}' (k-k_{0})+\dots = \omega_{0}+ \omega_{0}'\Delta k+\dots$$
- for a wave packet where the distribution is narrow around $k_{0}$, the wavefunction, $\psi$, is given by the integral: 
$$\begin{align*}
	\psi &= \int dk\, a(k)\exp(ik_{0}x+ i\Delta kx - i\omega_{0}t - i\omega_{0}'\Delta k t) \\
	&= \exp(ik_{0}x-i\omega_{0}t) \int dk \, a(k) \exp(i\Delta k(x-\omega_{0}'t))
\end{align*}$$
- let $s= z-\omega_{0}' t: |\psi|^{2}=|f(s)|^{2}$ 
- $\psi$ is a function in the form $f(s)=f(x-\omega_{0}'t)$, which represents the travelling wave packet moving along at group velocity, $\omega_{0}'$
- the shape of the wave packet is determined by the form of the distribution, $a(k)$
