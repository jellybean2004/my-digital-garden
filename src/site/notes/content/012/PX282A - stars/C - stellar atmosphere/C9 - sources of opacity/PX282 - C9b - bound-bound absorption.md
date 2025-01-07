---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/c-stellar-atmosphere/c9-sources-of-opacity/px-282-c9b-bound-bound-absorption/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-06T18:15:15.444+00:00"}
---

## bound-bound absorption
- discrete wavelengths would be absorbed, so a [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2b - dirac delta\|delta function]] is expected in a $\kappa_{\lambda}$-$\lambda$ plot
- in reality, there is a '**broadening**' in the line: 
$$\kappa_{\lambda}^{bb} \propto g_{m} N_{n} \psi(\lambda)$$
	where, 
		$g_{m}=$ statistical weight,
		$N_{m}=$ number density in state,
		$\psi(\lambda)=$ line profile
- the energy of the line: 
$$E_{m}-E_{n} = \Delta E = h\nu \implies \lambda = \frac{hc}{\Delta E}$$
- line broadening can occur due to several reasons
## natural broadening
- it arises from [[content/012/PX262 - quantum mechanics/term 1/A - recap/PX262 - A7 - the uncertainty principle\|the uncertainty principle]]: 
$$\Delta E \Delta t \geq \hbar \tag{1}$$
- the electron is in an excited state for a finite time, so the energy can only have an uncertain value: 
$$\begin{gather*}
	\Delta E = \frac{hc}{\lambda^{2}}\Delta\lambda =  \frac{\hbar}{\Delta t}  \; [ \text{from }(1)]\\
	\frac{hc}{\lambda}- \frac{hc}{\lambda+\Delta \lambda} = \frac{h}{2\pi\Delta t} \\
	\Delta \lambda = \frac{\lambda^{2} + \lambda\Delta\lambda}{2\pi c \Delta t}
\end{gather*}$$
- since $\Delta\lambda \ll \lambda:$ 
$$\Delta \lambda \approx \frac{\lambda^{2}}{2\pi c \Delta t} =\frac{\lambda^{2}}{2\pi c} \left( \frac{1}{\Delta t_{n}} + \frac{1}{\Delta t_{m}}\right)$$
- eg: $\lambda = 656\,nm$, for a $H_{\alpha}$ line:
		$n=2$, $m=3$
		$\Delta t_{2}\approx \Delta t_{3}= 10^{-8}\,s$
		$\implies \Delta \lambda = 4.6\times10^{-5}\,nm$
## doppler broadening
- it arises from the motion of the absorbing atom
- assuming atoms follow the [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C7 - maxwell-boltzmann distribution\|maxwell-boltzmann distribution]]
- the most probable velocity: 
$$v = \sqrt{\frac{2kT}{m}}$$
- the [[content/011/PX154 - physics foundations/PX154 - G - mechanical waves/PX154 - G6 - the doppler effect\|doppler shift]]: 
$$\frac{\Delta\lambda}{\lambda} = \pm \frac{v}{c}$$
- since it could be in either direction, there is a factor of $2:$  
$$\Delta\lambda = \frac{2\lambda}{c}\sqrt{\frac{2kT}{m}}$$
- eg: for $H_{\alpha}$ line in the sun, $T=5700\,K$, $m_{H} = 1.67\times10^-27\,kg:$
$$\therefore \Delta\lambda = 0.043\,nm$$
## pressure broadening
- it arises from the uncertainty principle again
- collisions shorten the lifetime of electron in a state
- from the [[content/012/PX262 - quantum mechanics/term 1/A - recap/PX262 - A7 - the uncertainty principle\|uncertainty principle]]:
$$\Delta E \sim \frac{\hbar}{\Delta t}$$
- if $\Delta t \downarrow: \Delta E \uparrow \; \implies \Delta\lambda \uparrow$ 
- estimate for $\Delta t:$ 
$$\Delta t \sim \frac{l}{v} = \frac{{1}/{n\sigma}}{v}$$
	where, ${} l= 1/n\sigma= {}$ [[content/012/PX282A - stars/C - stellar atmosphere/C5-8 - stellar atmospheres/PX282 - C7 - mean free path\|mean free path]], $v=$ velocity of atom, $n =$ number density, $\sigma=$ collision cross-section
$$\Delta \lambda \sim \frac{\lambda^{2}}{\pi c\Delta t} = \frac{\lambda^{2}}{\pi c} n\sigma \sqrt{\frac{2kT}{m}}$$
- here, $\Delta \lambda \propto n\sqrt{T} \implies$ higher $p$, higher $\Delta\lambda$

- eg: 
	- $n_{\odot} \sim 1.5\times10^{23}\,m^{-3}$ 
	- $\sigma \approx 2\pi r^{2}= 2\pi a_{0}^{2} = 1.8\times10^{-20}\,m^{2}$, where, $a_0=$ bohr radius
$$\therefore \Delta \lambda \approx 2\times10^{-5}\,nm$$

![line broadening.png|500](/img/user/pics/line%20broadening.png)
*image: K. N. Liou, An Introduction to Atmospheric Radiation*

- natural and pressure broadening form the lorentzian in the $\kappa-\lambda$ plot
## stellar rotation
- there will be constant doppler shifts from a rotating star: 
$$\frac{\Delta\lambda}{\lambda} = \frac{v_{rot}}{c}$$
- eg: for the sun, $P_{rot} = 27\,days$, $R_{\odot}= 7\times10^8\,m$, $v_{rot} \sim 2\times10^3\,ms^{-1}$
	$\therefore \Delta\lambda \approx 0.004\,nm$
