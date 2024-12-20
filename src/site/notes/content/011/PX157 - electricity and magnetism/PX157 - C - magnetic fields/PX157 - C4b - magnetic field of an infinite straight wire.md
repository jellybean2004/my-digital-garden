---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-c-magnetic-fields/px-157-c4b-magnetic-field-of-an-infinite-straight-wire/","noteIcon":"1","created":"2024-10-01T18:27:10.197+01:00","updated":"2024-11-26T20:09:56.340+00:00"}
---

![Pasted image 20240219183357.png](/img/user/pics/Pasted%20image%2020240219183357.png)
- **step 1: symmetry arguments**
	- $|\vec B|$ is constant at fixed radius, $R$, independent of ${} \phi$ and $z$
	- [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C3a - the biot-savart law\|the biot-savart law]] : $\vec B \perp I\,d\vec l \implies B_z =0$ 
	- solenoidal condition on cylindrical surface: $B_{R} = 0$
	- magnetic field is azimuthal: $\vec B = B_{\phi}(R)\,\hat\phi$
- **step 2: path**
	- a path, $C$, that is circular and centred on the wire, $d\vec l = dl\,\hat\phi :$
$$
\oint_{C}\vec B\cdot d\vec l = \oint_{C}B_{\phi}(R) \,dl = B_\phi(R)2\pi R
$$
- **step 3: enclosed current**
	- $I_{encl.} = I$
- **step 4: summarize**
	$$\begin{align*}
		B_{\phi}(R)2\pi R = \mu_{0}I \\
		\therefore \vec B = \frac{\mu_{0}I}{2\pi R} \hat\phi
		\end{align*}$$
