---
dg-publish: true
---
- in $A\cos{(\omega t)+ B\sin{(\omega t)}}$
	- $A'\cos(\omega t+\phi)$
	- 2 constants to find which specify the problem, ie: particular harmonic oscillation, usually from initial conditions
- eg: a mass $m=2kg$ on a spring with $k=8Nm^{-1}$. at $t=0s$, $x=2m$, and $\dot x=6ms^{-1}$
	- to find: $x(t)$
			$x=A\cos(\omega t)+B\sin(\omega t)$
			$\dot x = -\omega A\sin(\omega t) + B\omega \cos(\omega t)$
		- at $t=0$:
			$x=A+=2m$
			$\dot x=B\omega = 6ms^{-1}$
				$\omega = \sqrt{\frac{k}{m}}=\sqrt{\frac{8}{2}}=2s^{-1}$
				so, $B=3m$
			$\therefore x(t)=(2\cos{2t}+3\sin{2t})m$