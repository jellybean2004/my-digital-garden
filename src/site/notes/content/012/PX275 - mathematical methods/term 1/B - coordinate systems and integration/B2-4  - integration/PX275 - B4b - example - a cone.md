---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/b-coordinate-systems-and-integration/b2-4-integration/px-275-b4b-example-a-cone/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:57.028+00:00"}
---

![Pasted image 20241024121733.png](/img/user/pics/Pasted%20image%2020241024121733.png)
- taking a cone of radius, $1m$, and height, $3m$, by revolving the line, $y=\frac{x}{3}$, around the $x$-axis 
$$\begin{align*}
	A &= \int_{s_{1}}^{s_{2}} 2\pi \,y\,ds \\
	ds &= dx\sqrt{1 + \left(\frac{dy}{dx}\right)^{2}} \\\\
	A &= \int_{x=0}^{3}2\pi\,y \sqrt{1+\left(\frac{dy}{dx}\right)^{2}}\,dx \\
	&= \int_{x=0}^{3}2\pi\,\frac{x}{3} \sqrt{1+\left(\frac{1}{3}\right)^{2}}\,dx \\
	&= \int_{x=0}^{3}2\pi\,\frac{x}{3} \sqrt{\frac{10}{9}}\,dx \\
	&= \frac{\pi}{3}\sqrt{\frac{10}{9}} [x^{2}]_{0}^{3} \\
	\therefore A &= \pi\sqrt{10}
\end{align*}$$
### returning to centroids
- centroid in y of the function/curve that is being revolved: 
$$2\pi\,\bar y = \frac{2\pi\int y\,ds}{\int ds}$$
$$2\pi\,\bar y = \frac{A}{S}$$
	where, $A$ is surface area of the rotation, and $S$ is the length of the original curve
- pappus's second theorem: 
$$A = 2\pi\,\bar y\,S$$
