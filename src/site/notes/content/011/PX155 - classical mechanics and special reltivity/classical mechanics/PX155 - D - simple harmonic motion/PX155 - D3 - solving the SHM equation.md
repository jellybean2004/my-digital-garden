---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-d-simple-harmonic-motion/px-155-d3-solving-the-shm-equation/","created":"2024-10-01T18:27:09.641+01:00","updated":"2024-11-26T19:55:41.141+00:00"}
---

- try: $x=A\cos{\lambda t}$ 
		$\dot x = -A\lambda\sin{\lambda t}$
		$\ddot x = -A\lambda ^{2}\cos{x} = -\lambda ^{2}x$
			if $\lambda = \omega$, we have a solution
		similarly, $x=B\sin{\omega t}$ is a solution
	- general solution:
$$x=A\cos{\omega t}+B\sin{\omega t}$$
		- $\omega t$ plays the role of an angle in trig functions, so, $\omega$ *acts* like an *angular velocity*
			- argument $\theta = \omega t \implies \omega = \frac{\theta}{t} = angular \;velocity$
		- solutions repeat every $\omega t=2\pi$ because $\cos(\omega t +2\pi)=\cos(\omega t)$, and $\sin{(\omega t +2\pi)}=\sin{(\omega t)}$
			- $T= \frac{1}{f} = \frac{2\pi}{\omega}$
	- alternate form of the solution:
$$x=A' \cos(\omega t+\phi)$$
				$A'=$ amplitude
				$\phi =$ phase angle
		- comes from:
			  $cos(a+b)=cos(a)cos(b)-sin(a)sin(b)$
			  $A' cos(\omega t +\phi)= A'cos(\phi)cos(\omega t)-A' sin(\phi)sin(\omega t)$
		- ![Pasted image 20231024151059.png](/img/user/pics/Pasted%20image%2020231024151059.png)
		- peaks at $\omega t + \phi \pm 2n\pi =0$
			- so, peak at $t= -\frac{\phi}{\omega}\pm 2n\pi$ 

- eg: calculate the oscillation period when a mass of $0.1kg$ is attached to aspring with $k=100Nm^{-1}$
	- $\omega =\sqrt{\frac{k}{m}}, T= \frac{2\pi}{\omega}$
	- $T = 2n/\sqrt{\frac{k}{m}}=0.199s$