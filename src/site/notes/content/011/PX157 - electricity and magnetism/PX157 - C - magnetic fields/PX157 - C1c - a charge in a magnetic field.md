---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-c-magnetic-fields/px-157-c1c-a-charge-in-a-magnetic-field/","noteIcon":"1","created":"2024-10-01T18:27:10.177+01:00","updated":"2024-11-26T20:09:17.502+00:00"}
---

## the motion of a charge in a magnetic field
- a charge, $q$, in a uniform magnetic field, $\vec B$
- splitting the velocity vector of the charge, $\vec v$, into two components:
$$
\vec v (t) = \vec v_{\parallel} + \vec v_{\perp}
$$
- $\vec v_{\parallel} \times \vec B = 0$ and $\vec v_{\perp}\cdot \vec B =0$
$$\begin{align*}
	\vec F &= q\vec v \times \vec B \\ 
	&= q\vec v_{\perp}\times \vec B \\
	\therefore |\vec F| &= |q|\,v_{\perp}\,B
\end{align*}$$
- balancing this force against the centripetal acceleration:
$$\begin{align*}
		|q|v_{\perp}B &= \frac{mv_{\perp}^{2}}{R_{L}}\\
		\therefore R_{L}&= \frac{mv_{\perp}}{|q|B}
		\end{align*}$$
	where, $R_{L}=$ *larmer radius*
- parallel motion has no force as $\vec v_{\parallel}\times \vec B = \vec 0$, $\therefore \vec v_{\parallel}$ is constant

![Pasted image 20240213093445.png](/img/user/pics/Pasted%20image%2020240213093445.png)
- the motion is a helix

- **note:** to figure the direction of force, use left hand thumb rule for positive charge and right hand thumb rule for negative charge

## work done by  moving charge
- equation of motion:
$$\begin{align*}
		m \frac{d\vec v}{dt} &= q\vec v \times \vec B \\
		m \frac{d\vec v}{dt}\cdot\vec v &= q(\vec v \times \vec B)\cdot \vec v \\
		\frac{1}{2}m \frac{d}{dt}(\vec v\cdot \vec v) &= 0 \\
		\frac{1}{2}m \frac{d}{dt}v^{2} &= 0 \\
		\frac{d}{dt} \left(\frac{1}{2}mv^{2}\right) &= 0 \\
	\end{align*}$$
- $KE$ is constant $\implies$ no work done
- therefore, a magnetic field (constant in time and space) does no work

- alternatively,
$$
W = \int q(\vec v \times \vec B) \cdot d\vec l
$$
- $d\vec l$ is along the path, but ${} \vec v$ is also along the path:
$$
\vec v = \frac{d \vec l}{dt} \implies \vec v \parallel d\vec l \implies W=0
$$
