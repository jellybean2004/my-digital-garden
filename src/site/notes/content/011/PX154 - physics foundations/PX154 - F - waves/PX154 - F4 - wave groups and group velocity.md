---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-f-waves/px-154-f4-wave-groups-and-group-velocity/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:51:31.479+00:00"}
---

 - from [[content/011/PX154 - physics foundations/PX154 - F - waves/PX154 - F3a - principle of superposition#^d12c0f\|PX154 - F3a - principle of superposition#^d12c0f]]: $$u_{total} = 2A\cos(kx-\omega t)\cos(\Delta kx -\Delta \omega t)$$
	- where, 
		$\cos(kx-\omega t)= \frac{\omega}{k} =$ wave speed, 
		$\cos(\Delta kx -\Delta \omega t)= \frac{\Delta \omega}{\Delta k}=$ "*group velocity*"
	- keeping $|\Delta k|<<|k|$, and then, taking $\frac{\Delta\omega}{\Delta k} \to \frac{d\omega}{dk} \to group \; velocity (v_{g})$

- if any amplitude is considered maximum between two minima, this is the speed of this group of waves. $\frac{\omega}{k}$ is the "*phase velocity*", $v_{p}$
## dispersion
- this is the relationship between $\omega$ and $k$ for our wave: $\omega(k)$
	- waves of different wavelengths travelling at different speeds
- eg: gravity waves on deep water (dimensional analysis}: 
$$v_{p} \propto \sqrt{g\lambda}$$
	- we have, $k = \frac{2\pi}{\lambda}$, $v_{p}= \frac{\omega}{k}$
	$$v_{p}= \frac{\omega}{k} \propto \sqrt{g .\frac{2\pi}{k}} \implies v_{p}= constant \times \sqrt{\frac{g}{k}}$$
	- or, the "*dispersion relation*": 
	$$\omega(k) = constant \times \sqrt{gk}$$
	- also, $v_{g} = \frac{d\omega}{dk} = \frac{constant}{2} \sqrt{\frac{g}{k}}$
	- so, $v_{g}= \frac{v_{p}}{2}$
	- these waves are *dispersive*:
		- wave speed($v_{p}$) depends on $k$, hence wavelength
		- $v_{g}\neq v_{p}$

- eg: capillary waves on water: 
$$\omega^{2} = \frac{\sigma}{\rho}k^{3}$$
		where, $\sigma=$ surface tension, $\rho=$ density 
			$2\omega \frac{d\omega}{dk}= 3\frac{\sigma}{\rho}k^{2}$
			$v_{g} = \frac{d\omega}{dk} = \frac{3}{2}\sqrt{\frac{\sigma}{\rho}k}$
			$v_{p} = \frac{\omega}{k} = \sqrt{\frac{\sigma}{\rho}k}$
			$\therefore v_{g}= \frac{3}{2} v_{p}$
	- waves are dispersive:
		- $v_{p} \propto \sqrt{k}$
		- $v_{g}\neq v_{p}$

- eg: sound waves in air
	- for sound: 
	$$\omega(k) = k \sqrt\frac{B}{\rho}$$
		where, $B=$ bulk radius, $\rho=$ density of air
		$v_{p}= \frac{\omega}{k} = \sqrt{\frac{B}{\rho}}$
		$v_{g} = \frac{d\omega}{dk} = \sqrt{\frac{B}{\rho}}$
	- these are *non-dispersive* waves:
		- $v_{p}$ doesn't depend on $k$
		- $v_{g} = v_{p}$

- also important for light:
	- speed of light in vacuum is $c = 3 \times 10^{8} ms^{-1}$
	- now, snell's law: 
	$$n_{1}\sin\theta_{1} = n_{2} \sin\theta_{2}$$
		where, $n =\frac{c}{v}$ is the refractive index, $\theta$ is the angle with normal
	- for glass: $n_{1}= 1, n_{2}= 1.5$; $v = \frac{c}{n}$
		$\sin\theta_{2} = \frac{v_{2}}{c}\sin\theta_{1}$
	- light travelling through materials exhibits dispersion (eg: a prism)
	
 - eg: EM waves in the ionosphere: 
 $$(\omega(k))^{2} = c^{2}k^{2}+\omega_{p}^{2}$$
		 where, $w_p=$ cyclotron frequency (a constant)
	- find $v_{p}$ and $v_{g}$
			$v_{p} = \frac{\omega}{k} = \sqrt{c^{2} + \frac{\omega_{p}^{2}}{k^{2}}}$
			$v_{g} = \frac{d\omega}{dk} = \frac{2c^{2}k}{\sqrt{c^{2}k^{2}+\omega_{p}^{2}}}$
		- the waves are *dispersive*:
			$v_{p}\neq v_{g}$
			$v_{p}$ depends on $k$
		- any thing strange about $v_{p}$?
			- faster than the speed of light