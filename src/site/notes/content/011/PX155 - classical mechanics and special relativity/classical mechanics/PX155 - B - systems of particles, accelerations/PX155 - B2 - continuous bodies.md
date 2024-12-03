---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-b-systems-of-particles-accelerations/px-155-b2-continuous-bodies/","created":"2024-10-01T18:27:09.493+01:00","updated":"2024-11-26T19:55:12.100+00:00"}
---

- more common to treat bodies as continuous, not a collection of distinct points
	- eg: $N\to \infty$ and $m_i\to0$ infinite number of points(elements) of mass $dm$$$\vec r_{cm}=\frac{\int \vec r dm}{\int dm}$$
		- ***NB***: $\int \vec r dm = (\int x dm, \int y dm, \int z dm)$
		- x-component of $\vec r_{cm}= \frac{\int xdm}{\int dm}$
- eg: a bar of length $l$ has mass per unit length $\rho = \alpha x$, where $x$ is the distance from one end
	- to find: the position of its centre of mass
	
$$M=\int dm=\int_0^L \rho.dx =\int_o^L\alpha x .dx = \alpha[\frac{x^2}{2}]_0^L= \frac{\alpha L^2}{2}$$
	- similarly,$$\int x.dm=\int_0^L x\rho.dx =\int_o^L\alpha x^2 .dx = \alpha[\frac{x^3}{3}]_0^L= \frac{\alpha L^3}{3}$$
	- hence,
$$x_{cm}=\frac{\int x.dm}{\int dm}=\frac{2}{3}L$$
- eg: find the centre of mass of a uniform semicircle of radius $R$ ![Pasted image 20231011090437.png](/img/user/pics/Pasted%20image%2020231011090437.png)
	- let
$$\sigma = \frac{M}{A}\implies M = \frac{\pi R^2}{2}\sigma(=\int dm)$$
	- slicing the semicircle vertically:
$$\int x.dm=\int_0^R x.2.(R^2-x^2)^{\frac{1}{2}}.\sigma.dx=...=\frac{2}{3}\sigma R^3$$
	$$\therefore x_{cm}=\frac{\int x.dm}{\int dm}=\frac{4}{3\pi} R\approx 0.424R$$