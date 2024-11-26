---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-the-solar-system/c-stellar-atmosphere/c2-14-stellar-atmospheres/px-282-c10b-line-broadening-from-bound-bound-absorption/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:38:38.956+00:00"}
---

## bound-bound absorption
- discrete wavelengths would be absorbed, so a $\delta$ function is expected in a $\kappa_{\lambda}-\lambda$ plot, but in reality, there is a '**broadening**' in the line: 
$$\kappa_{\lambda}^{bb} \propto g_{m} N_{n} \psi(\lambda)$$
	where, 
		$g_{m}=$ statistical weight,
		$N_{m}=$ number density in state,
		$\psi(\lambda)=$ line profile
- the energy of the line: 
$$E_{m}-E_{n} = \Delta E = h\nu \implies \lambda = \frac{hc}{\Delta E}$$

## natural broadening
- this arises from [[content/012/PX262 - quantum mechanics/A - recap/PX262 - A7 - the uncertainty principle\|the uncertainty principle]]: 
$$\Delta E \Delta t = \hbar$$
- the electron is in an excited state for a finite time, so the energy can only have an uncertain value: 
$$\begin{gather*}
	\Delta E = \frac{h}{2\pi \Delta t} \\
	\frac{hc}{\lambda}- \frac{hc}{\lambda+\Delta \lambda} = \frac{h}{2\pi\Delta t} \\\\
	\text{multipy by } \lambda(\lambda+\Delta \lambda): \\\\
	\Delta \lambda =\frac{\lambda^{2}}{2\pi c} \left( \frac{1}{\Delta t_{n}} + \frac{1}{\Delta t_{m}}\right)
\end{gather*}$$
- eg: $\lambda = 656\,nm$, for a $H_{\alpha}$ line:
		$n=2$, $m=3$
		$\Delta t_{2}\approx \Delta t_{3}= 10^{-8}\,s$
		$\implies \Delta \lambda = 4.6\times10^{-5}\,nm$
## doppler broadening
- arises from the motion of the absorbing atom
- assume atoms follow the maxwell-boltzmann distribution: 
	- the most probable velocity: 
	$$v = \sqrt{\frac{2kT}{m}}$$
	- the doppler shift: 
	$$\frac{\Delta\lambda}{\lambda} = \pm \frac{v}{c}$$
	- since it could be in either direction, there is a $2\times:$  
	$$\implies \Delta\lambda = \frac{2\lambda}{c}\sqrt{\frac{2kT}{m}}$$
- eg: for $H_{\alpha}$ line in the sun, $T=5700\,K$, $m_{H} = 1.67\times10^-27\,kg$
		$\implies \Delta\lambda = 0.043\,nm$
## pressure broadening
- arises from the uncertainty principle again
- collisions cause shorter lifetime of electrons in a state
$$\Delta E \sim \frac{h}{2\pi\Delta t}$$
- if $\Delta t \downarrow: \Delta E \uparrow \; \Delta\lambda \uparrow$ 
- estimate for $\Delta t:$ 
$$\Delta t \sim \frac{l}{v}$$
	where, $l=$ mean free path, $v=$ atom velocity
$$\Delta \lambda \sim \frac{\lambda^{2}}{\pi c\Delta t} = \frac{\lambda^{2}}{c} \frac{n\sigma}{\pi} \sqrt{\frac{2kT}{m}}$$
	where, $n =$ number density, $\sigma=$ collision cross-section
- eg: $n_{\odot} \sim 1.5\times10^23\,m^{-3}$, $\sigma \approx 2\pi r^{2}= 2\pi a_{0}^{2} = 1.8\times10^{-20}\,m^{2}$
	$\implies \Delta \lambda \approx 2\times10^{-5}\,nm$

- $\Delta \lambda \propto n\sqrt{T} \implies$ higher $p$, higher $\Delta\lambda$
## stellar rotation
- there will be constant doppler shifts from a rotating star: 
$$\frac{\Delta\lambda}{\lambda} = \frac{v_{rot}}{c}$$
- eg: for the sun, $P_{rot} = 27\,days$, $R_{\odot}= 7\times10^8\,m$, $v_{rot} \sim 2\times10^3\,ms^{-1}$
	$\implies \Delta\lambda \approx 0.004\,nm$
