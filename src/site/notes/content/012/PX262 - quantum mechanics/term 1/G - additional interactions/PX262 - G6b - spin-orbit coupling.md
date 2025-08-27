---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/g-additional-interactions/px-262-g6b-spin-orbit-coupling/","noteIcon":"1","created":"2025-08-27T13:15:23.115+01:00","updated":"2024-12-21T13:22:32.000+00:00"}
---

- in the reference frame of an electron orbiting a nucleus, the nucleus is 'seen' to be orbiting it
- the electron is at the centre of a current carrying loop , so it is subject to magnetic field given by [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C3b - the biot-savart law applied to a wire\|the biot-savart law]]:
$$B = \frac{\mu_{0}Ze\omega}{4\pi r} = \frac{\mu_{0}Ze}{4\pi mr^{3}}l$$
	where, $\frac{Ze\omega}{2\pi}$ corresponds to the current
- the energy of the interaction is:
$$W = - \frac{1}{2} \vec \mu_{s} \cdot \vec B = \frac{\mu_{0}Ze^{2}}{8\pi m^{2}r^{3}} \vec l \cdot \vec s$$
	where, the factor of $1/2$ comes from a relativistic effect known as **thomas precession**
- $\vec l \cdot \vec s$ can be expressed through the total angular momentum: 
$$\begin{align*}
 \vec j &= \vec l + \vec s \\
 \implies j^{2} &= l^{2}+ s^{2} + 2 \,\vec l \cdot \vec s \\
 \therefore \vec l \cdot \vec s &= \frac{1}{2} (j^{2} - l^{2} - s^{2})
\end{align*}$$
- therefore, the interaction energy is: 
$$W = \frac{\mu_{0}Ze^{2}}{16\pi m^{2}r^{3}} (j^{2}-l^{2}- s^{2})$$
- using [[content/012/PX262 - quantum mechanics/term 1/C - the basic postulates/PX262 - C2c - postulates 2 & 3\|postulate 3]], the interaction energy operator can be written as: 

$$\hat H_{LS} = f(r) (\hat J^{2} - \hat L^{2} - \hat S^{2})$$
	where, $f(r) = \frac{\mu_{0}Ze^{2}}{4\pi m^{2}r^{3}}$
	
- this is called **spin-orbit (LS) coupling**

- additional note:
	- if $s = \frac{1}{2 :}j = l \pm \frac{1}{2}\to$ 2 states, splits into $2$
	- but, if $s=1/2$ and $l=0: j = \frac{1}{2}\to 1$ state, no splits
	- therefore, each state with a given value of $j$ consists of $(2j + 1)$ degenerate components
	- these can be separated by an applied magnetic field
- 