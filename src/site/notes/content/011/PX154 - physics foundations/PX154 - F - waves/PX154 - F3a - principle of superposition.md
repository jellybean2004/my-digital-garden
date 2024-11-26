---
dg-publish: true
---

- to add waves together
	- eg: diffraction experiment with a laser + diffraction grating
- to add waves of  different frequencies
## phase differenece
![Pasted image 20231121083811.png](/img/user/pics/Pasted%20image%2020231121083811.png)
- the wave function can be written as: 
$$\begin{align*}
	u_{1}(x,t) = A\cos(kx-\omega t) \; ... [1] \\
	u_{2}(x,t) = A\sin(kx-\omega t) \; ... [2]
\end{align*}$$
	- for $[2]$, $\sin$ is used instead of $\cos$, but they both behave similarly
- the *phase difference*, $\phi$, can be introduced as: 
$$u_{3}(x,t) = A \cos(kx-\omega t+ \phi)$$
	- typically, $(0 \leq \phi \leq 2\pi)$, or ($-2\pi \leq \phi \leq 2\pi)$
- if $\phi = \pi$: 
$$u_{3}(x,t) = A\cos(kx-\omega t + \pi) \equiv -A\cos(kx-\omega t)$$
- $u_{1} + u_{3} = 0$: *destructive interference*
## waves of the same frequency
- eg: two loudspeakers emitting *middle C* $(261.63Hz)$
		$u_{1}(x,t) = A \cos(kx-\omega t+ \phi_{1})$
		$u_{2}(x,t) = A \cos(kx-\omega t+ \phi_{2})$
	- let both have the same amplitude, $A$
		- helpful identity: $$\cos A + \cos B = 2\cos(\frac{A+B}{2})\cos(\frac{A-B}{2}) \;...[3]$$
	- adding the waves: 
	$$u_{1}+u_{2} = 2A \cos(kx-\omega t + \frac{\phi_{1}+\phi_{2}}{2})\cos(\frac{\phi_{1}-\phi_{2}}{2})$$
		- first $\cos$ is equation of a wave
		- second $\cos$ depends on the phase difference, and has no time or position dependence
	- if waves are *in phase*: $\Delta \phi = \phi_{1} - \phi_{2} = 0$
		- then, $u_{total} = u_{1}+u_{2} = 2u_{1}= 2u_{2}$
	- if waves are *out of phase*: $\Delta\phi = \pi$
		- then, $\cos(\frac{\phi_{1}-\phi_{2}}{2})= \cos(\frac{\pi}{2}) = 0$
			$\therefore u_{total} = 0$ 
