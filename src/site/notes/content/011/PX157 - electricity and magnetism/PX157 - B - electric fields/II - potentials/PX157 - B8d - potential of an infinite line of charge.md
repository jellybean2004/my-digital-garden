---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/ii-potentials/px-157-b8d-potential-of-an-infinite-line-of-charge/","noteIcon":"1","created":"2025-08-27T13:14:00.333+01:00","updated":"2024-11-26T20:08:33.000+00:00"}
---

![Pasted image 20240125100604.png](/img/user/pics/Pasted%20image%2020240125100604.png)
$$
\vec E = \frac{\lambda}{2\pi\epsilon_{0}R} \hat R
$$
- for path: $\vec r= R\,\hat R \implies d\vec l = d\vec r = dR\,\hat R$
- apply $V_{a}-V_{b} = \int_{a}^{b}\vec E \cdot d\vec l$ :
$$\begin{align*}
	V_{a} &= \int_{R_{a}}^{R_{b}} \frac{\lambda}{2\pi\epsilon_{0}R} \hat R \cdot \hat R\, dR \\
	&= \frac{\lambda}{2\pi\epsilon_{0}} \int_{R_{a}}^{R_{b}} \frac{1}{R}\, dR \\
	&= \frac{\lambda}{2\pi\epsilon_{0}} \ln\left[\frac{R_{b}}{R_{a}}\right] \\
\end{align*}$$
- here, choosing $V(R_{b}\to\infty)=0$ doesn't work
- let, for any finite value $R_{b}=R_{0}, \; V(R_0)=0:$ 
$$
V_{a}= \frac{\lambda}{2\pi\epsilon_{0}} \ln\left[\frac{R_{0}}{R_{a}}\right]
$$
- this is true for any value of $R_{a}$
$$
\therefore V(R)= \frac{\lambda}{2\pi\epsilon_{0}} \ln\left[\frac{R_{0}}{R}\right]
$$
