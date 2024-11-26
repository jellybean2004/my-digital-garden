---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-e-circular-motion-rotation-of-bodies/px-155-e12-example-of-moments-of-intertia/","created":"2024-10-01T18:27:09.687+01:00","updated":"2024-11-26T19:57:15.934+00:00"}
---

![Pasted image 20231108063054.png](/img/user/pics/Pasted%20image%2020231108063054.png)
- eg: find $I$ for a thin ring with radius,$R$, and mass ,$M$, about an axis through the centre of the ring, and perpendicular to the ring
	- all mass is at a distance, $R$, from the axis
	- let mass per unit length of circumference $=\sigma$, then, a small section, $d\theta$, will have mass, $dm = R\sigma d\theta$:
$$I = \int r^{2}.dm = R^{2} \int_{0}^{2\pi} R\sigma.d\theta = 2\pi R^{3}\sigma$$
	- ***but*** $2\pi R\sigma = M$,
$$\therefore I=MR^{2}$$
- eg: find $I$ for a uniform disc with radius, $R$, and mass, $M$, about an axis through its centre, and perpendicular to the disc 
	- integrate all rings at radius, $r$, and thickness ,$dr$
	- mass of each ring = $2\pi rdr\sigma$, $\sigma =$ mass per unit area
	- $dm = (2\pi rdr)\sigma$
	- $I=\int r^{2}.dm = 2\pi \sigma \int_{0}^{R} r^{3}.dr = 2\pi \sigma \frac{R^{4}}{4}$
	- ***but*** $\pi R^{2}\sigma = M$,
$$\therefore I = \frac{1}{2}MR^{2}$$
- other moments of inertia
	- $I$ for a hollow sphere about an axis through its centre $=\frac{2}{3}MR^{2}$
	- $I$ for a solid sphere about an axis through its centre $= \frac{2}{5}MR^{2}$
	- $I$ for a thin uniform rod, with length, ${} L$, about a perpendicular axis through its centre $= \frac{1}{12}ML^{2}$
	- $I$ for a thin uniform rod, with length, ${} L$, about a perpendicular axis through one end $= \frac{1}{3}ML^{2}$
- for exam: $I$ is either given or needs to be derived