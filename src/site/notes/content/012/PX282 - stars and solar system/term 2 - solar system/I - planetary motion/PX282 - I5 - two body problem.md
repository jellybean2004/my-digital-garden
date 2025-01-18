---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/i-planetary-motion/px-282-i5-two-body-problem/","noteIcon":"1","created":"2025-01-17T16:24:15.624+00:00","updated":"2025-01-17T16:28:03.764+00:00"}
---

- for the **one body problem** (where mass of one object dominates), considering the sun in the origin, and planet at a position given by $\vec r$
- the equation of motion, ie. the acceleration due to gravity:
$$\frac{d^{2}\vec r}{dt^{2}} = - \frac{GM}{r^{2}} \hat r$$


- now, for the **two body problem** (where both masses matter), placing the centre of mass at the origin:
$$\frac{m_{1}\vec{r_{1}}+m_{2}\vec{r_{2}}}{m_{1}+m_{2}} = 0$$
- also:
$$\vec r = \vec r_{2}- \vec r_{1}$$
$$\begin{align*}
\implies \vec r_{1} &= - \frac{m_{2}}{m_{1}+m_{2}} \vec r \\
\vec r_{2} &= \frac{m_{1}}{m_{1}+m_{2}} \vec r
\end{align*}$$
- the two bodies have orbits with the same shape, both proportional to $\vec r$, but of different amplitudes

$$\begin{align*}
\frac{d^{2}\vec{r}}{dt^{2}}&= \frac{d^{2}\vec{r_{2}}}{dt^{2}} - \frac{d^{2}\vec{r_{1}}}{dt^{2}} \\
&= - \frac{Gm_{1}}{r^{2}} \hat r - \frac{Gm_{2}}{r^{2}}\hat r \\
&= \frac{G(m_{1}+ m_{2})}{r^{2}}
\end{align*}$$
- this is mathematically identical to the one-body problem

- [[content/012/PX282 - stars and solar system/term 2 - solar system/I - planetary motion/PX282 - I2 - kepler's laws\|kepler's laws]] apply and both objects follow elliptical orbits with the centre of mass at a focus of the ellipse

>[!note] generalized kepler's third law
> $$P^{2} = \frac{4\pi^{2}}{G(m_{1}+m_{2})} (a_{1}+a_{2})^{2}$$

