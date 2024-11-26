---
dg-publish: true
---

- **top-hat distribution**: 
$$a(k) =\begin{cases}
    A &for& k_{0}-\frac{w}{2}<k<k_{0}+\frac{w}{2} \\
    0 && otherwise
\end{cases}$$
$$\begin{align*}
	f(s) &= A\int_{-\frac{w}{2}}^{\frac{w}{2}} dk' \,\exp(ik's) \\
	&= A\left[\frac{\exp(ik's)}{is}\right]_{-\frac{w}{2}}^{\frac{w}{2}} \\
	&= \frac{2A}{s} \sin\left(\frac{ws}{2}\right) \\\\
	\therefore |f(s)|^{2} &= \frac{4A^{2}}{s^{2}} \sin^{2}\left(\frac{ws}{2}\right)
\end{align*}$$
![Pasted image 20240305094130.png](/img/user/pics/Pasted%20image%2020240305094130.png)
- the width in $k$ is $w$
- the width in $s$ is inversely proportional to $w$

- **important result**: a wave packet with width, $w$, can represent a particle localised in a region of width of order $\frac{1}{w}$
	