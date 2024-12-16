---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-e-second-order-inhomogeneous-od-es/px-153-e3-driven-damped-simple-harmonic-motion/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:17.498+00:00"}
---

*[[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - D - simple harmonic motion/PX155 - D9 - driven damped simple harmonic motion\|PX155 - D9 - driven damped simple harmonic motion]]*
- add a periodic driving force to our damped SHM. we'll write 
$$f(x) = A_{0}e^{i\omega t}$$
	- often written as $A_{0}\cos(\omega t)$
- the equation of motion becomes: 
$$\ddot x + 2\alpha\dot x + \omega_{0}^{2}x = A_{0}e^{i\omega t}$$
	- we'll assume underdamped, so the complementary function is 
	$$x_{c}= e^{-\alpha t} (Ce^{i\omega't}+De^{-i\omega't})$$
		- where, $\omega' = \sqrt{\omega_{0}^{2}-\alpha^{2}}$
	- for the particular integral, our trial function is $x_{p}(t) = a e^{i\omega t}$
		- $a$ could be a complex number
		$-\omega ^{2}ae^{i\omega t} + 2\alpha i \omega ae^{i\omega t}+ \omega_{0}^{2}ae^{i\omega t}= A_{0}e^{i\omega t}$
		$a(\omega_{0}^{2} -\omega^{2}+2\alpha i \omega) = A_{0}$
		$\therefore a = \frac{A_{0}}{(\omega_{0}^{2}-\omega^{2})+2\alpha i \omega}$
			- $a$ is a complex number
			$|a| = \sqrt{a^{*}a} = \sqrt{\frac{A_{0}}{(\omega_{0}^{2}-\omega^{2})+2\alpha i \omega}} = A$
			$arg(a) = \tan^{-1} \frac{Im(a)}{Re(a)}$
			$arg(a) = \phi = \tan^{-1} (\frac{-2\alpha\omega}{\omega_{0}^{2}-\omega^{2}})$
		- find maximum of $a$ and sketch 
		$$G.S. : x(t) = e^{-\alpha t} (Ce^{i\omega't} + De^{-i\omega't}) + Ae^{i(\omega t + \phi)}$$
			- where, $A=\sqrt{\frac{A_{0}}{(\omega_{0}^{2}-\omega^{2})+2\alpha i \omega}}$ and $\phi = \tan^{-1} (\frac{-2\alpha\omega}{\omega_{0}^{2}-\omega^{2}})$
