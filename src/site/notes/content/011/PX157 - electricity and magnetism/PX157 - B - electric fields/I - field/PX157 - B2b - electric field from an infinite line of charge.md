---
dg-publish: true
---
- charge uniformly spread along the line
- linear charge density, $\lambda$ is constant
![Pasted image 20240116095422.png](/img/user/pics/Pasted%20image%2020240116095422.png)
- cylindrical coordinates $(R, \phi, z)$
- at point, $P: \vec r = R \hat R + z \hat z$
- section at $\vec r' = z' \hat z$
	$dQ = \lambda dz'$
	$\vec r - \vec r' = R \hat R + (z-z')\hat z$
$$distance = |\vec r - \vec r'| = \sqrt{R^{2} + (z-z')^{2}}
$$ 
$$
	d\vec E = \frac{\lambda dz'}{4 \pi \epsilon_{0}} \frac{R \hat R + (z-z')\hat z}{(R^{2} + (z-z')^{2})^\frac{3}{2}}$$
	$$\vec E = \int d\vec E = \int_{-\infty}^{+\infty} \frac{\lambda}{4 \pi \epsilon_{0}} \frac{R \hat R + (z-z')\hat z}{(R^{2} + (z-z')^{2})^{\frac{3}{2}}}dz'$$
- using integrals:
$$\begin{align}
\int_{-\infty}^{+\infty} \frac{a}{(a^{2}+x^{2})^{\frac{3}{2}}}.dx &= \frac{2}{a} \\
\int_{-\infty}^{+\infty} \frac{x}{(a^{2}+x^{2})^{\frac{3}{2}}}.dx &= 0
\end{align}$$
$$
\therefore \vec E = \frac{\lambda}{4\pi\epsilon_{0}} \frac{2}{R} \hat R = \frac{\lambda}{2\pi\epsilon_{0}R}\hat R
$$
