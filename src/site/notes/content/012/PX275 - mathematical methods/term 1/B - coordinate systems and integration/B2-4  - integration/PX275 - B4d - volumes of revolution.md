---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/b-coordinate-systems-and-integration/b2-4-integration/px-275-b4d-volumes-of-revolution/","noteIcon":"1","created":"2025-08-27T13:14:16.063+01:00","updated":"2024-11-26T10:05:00.000+00:00"}
---

![Pasted image 20241024123648.png](/img/user/pics/Pasted%20image%2020241024123648.png)
- revolving the plane around the $x$-axis to obtain a solid, cylindrical volume
- taking the area element, $dA$, and revolving it by an angle, $d\theta$, around the $x$-axis
- the volume element: 
$$dV = dA \,y\,d\theta = y\,d\theta\,dx\,dy$$
$$ V = \int_{x=x_{1}}^{x_{2}} \int_{\theta=0}^{2\pi} d\theta \int_{y=0}^{f(x)}y\,dy\,dx = 2\pi \int_{x_{1}}^{x_{2}} \frac{(f(x))^{2}}{2}\,dx$$
$$ \therefore V = \pi \int_{x_{1}}^{x_{2}}(f(x))^{2}\,dx$$
## example
- taking the cone again
![Pasted image 20241024124418.png](/img/user/pics/Pasted%20image%2020241024124418.png)
$$\begin{align*}
	V &= \pi \int _{0}^{h}\left(\frac{ax}{h}\right)^{2}\,dx \\
	&= \pi \left(\frac{a}{h}\right)^{2} \left[\frac{x^{3}}{3} \right]_{0}^{h}\\
	\therefore V &= \frac{1}{3}\pi a^{2}h
\end{align*}$$