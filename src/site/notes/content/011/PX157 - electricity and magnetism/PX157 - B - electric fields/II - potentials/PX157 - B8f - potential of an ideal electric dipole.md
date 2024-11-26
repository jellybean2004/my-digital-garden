---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/ii-potentials/px-157-b8f-potential-of-an-ideal-electric-dipole/","created":"2024-10-01T18:27:10.110+01:00","updated":"2024-11-26T23:15:22.912+00:00"}
---

![Pasted image 20240125101634.png](/img/user/pics/Pasted%20image%2020240125101634.png)
- origin is on the midpoint of the two charges, $+q$ and $-q$
$$\begin{align*}
	\vec E &\approx \frac{1}{4\pi\epsilon_{0}r^{3}} \big[3(\vec p \cdot \hat r)\hat r - \vec p\big] \\
	\vec E &\approx \frac{p}{4\pi\epsilon_{0}r^{3}}(2\cos\theta\,\hat r + \sin\theta\,\hat\theta) \\
\end{align*}$$
- $\vec p = q\vec l = ql\,\hat z$
- for the path: ${} \vec r = r\,\hat r \implies d\vec l = d\vec r = dr\,\hat r$
- apply $V_{a}-V_{b} = \int_{a}^{b}\vec E \cdot d\vec l$ :
$$\begin{align*}
	V_{a} &= \int_{r_{p}}^{r_{b}} \frac{p}{4\pi\epsilon_{0}r^{3}}(2\cos\theta\,\hat r + \sin\theta\,\hat\theta)\,\hat r\,dr \\
	&= \frac{p\cos\theta}{2\pi\epsilon_{0}} \int_{r_{p}}^{r_{b}} \frac{1}{r^{3}}dr \\
	&= \frac{p\cos\theta}{2\pi\epsilon_{0}} \left(- \frac{1}{r^{2}}\right)_{r_{p}}^{r_{b}} \\
	&= \frac{p\cos\theta}{2\pi\epsilon_{0}} \left(\frac{1}{r_{p}^{2}} - \frac{1}{r_{b}^{2}}\right)
\end{align*}$$
- define $V(r_{b}\to\infty) = 0:$
$$
V_{a} = \frac{p\cos\theta}{2\pi\epsilon_{0}r_{p}^2}
$$
- true for any value of $r_{p}:$
$$
\therefore V(r) = \frac{p\cos\theta}{2\pi\epsilon_{0}r^{2}}= V_{a} = \frac{\vec p\cdot \hat r}{2\pi\epsilon_{0}r^2}
$$
- eg: electric field that is discontinuous between $R = R_{1}\to R_{2}$
	- can only choose one point where $V=0$
	$$V_{a}-V_{b} = \int_{R_{a}}^{R_{b}} \vec E\cdot d\vec l = \int_{R_{a}}^{R_{2}} \vec E\cdot d\vec l + \int_{R_{2}}^{R_{1}} \vec E\cdot d\vec l + \int_{R_{1}}^{R_{b}} \vec E\cdot d\vec l$$
- **note**: potential is **always** continuous
