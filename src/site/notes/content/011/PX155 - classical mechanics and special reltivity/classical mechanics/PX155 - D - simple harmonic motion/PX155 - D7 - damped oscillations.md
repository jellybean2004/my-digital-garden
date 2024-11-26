---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-d-simple-harmonic-motion/px-155-d7-damped-oscillations/","created":"2024-10-01T18:27:09.663+01:00","updated":"2024-11-26T19:55:57.022+00:00"}
---

![Pasted image 20231030184750.png](/img/user/pics/Pasted%20image%2020231030184750.png)
- model motion of our oscillator through a viscous fluid with a drag force proportional to $\dot x$, ie:$-b\dot x$
	- [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]]: $m \ddot x = -kx - b\dot x$
	- dividing by m on both sides:$$\ddot x + \omega^{2}x + \gamma \dot x =0$$
			where, $\gamma = \frac{b}{m}$
	- switch to complex notation:
$$\ddot z + \omega ^{2}z + \gamma \dot z = 0 \, ...[1]$$
	- physically motivated:
$$z = ae^{pt}$$
			where, $p$ might be complex
		- $p$ is imaginary - oscillation
		- $p$ is real and negative - decay
			$z=ae^{pt}$
			$\dot z = pae^{pt}=pz$
			$\ddot z = p^{2}ae^{pt}=p^2z$
			- in $[1]$: $p^{2}z+\omega ^{2}z+\gamma pz =0$
				$z(p^{2} + \gamma p + \omega^{2})=0$
				$either \; z=0$ boring
				$or \; p^{2} + \gamma p + \omega^{2} = 0$
				
$$p = \frac{-\gamma\pm\sqrt{\gamma^{2}-4\omega^{2}}}{2}$$
				
$$p=- \frac{\gamma}{2} \pm \sqrt{\left(\frac{\gamma}{2}\right)^{2}-\omega^{2}}$$
				- $p$ can be complex, or real and negative *but* never real and positive