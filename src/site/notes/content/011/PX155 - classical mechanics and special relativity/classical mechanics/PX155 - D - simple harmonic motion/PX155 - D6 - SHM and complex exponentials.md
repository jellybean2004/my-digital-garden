---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-d-simple-harmonic-motion/px-155-d6-shm-and-complex-exponentials/","noteIcon":"1","created":"2024-10-01T18:27:09.660+01:00","updated":"2024-11-26T19:55:55.165+00:00"}
---

using [[content/011/PX153 - mathematics for physicists/term 1/PX153 - B - complex numbers/PX153 - B2 - polar representation#euler's formula\|euler's formula]]
$$e^{i\theta}=\cos\theta+i\sin\theta$$
- so, $$x=A' \cos{(\omega t+\phi)}= \mathbb Re(A'e^{i(\omega t + \phi)})$$
$$x=\mathbb{R}e(A'e^{i\theta}e^{i\omega t})$$
- let complex amplitude $a=A'e^{i\phi}$
$$x=\mathbb{R}e(ae^{i\omega t})$$
	- $a$ encodes both amplitude and the phase $\phi$ in one complex number
- the complex number $z=ae^{i\omega t}$ is a solution of ${} \ddot z +\omega^{2} z = 0 {}$
	- ie: $\dot z =  i \omega ae^{i\omega t}=i\omega z$
		$\ddot z = -\omega^{2} ae^{i\omega t}=-\omega^{2} z$
	- so, $\ddot z + \omega ^{2}z = 0$
- so, can solve $SHM$ equation for complex variables $z$ and take the real part of the solution