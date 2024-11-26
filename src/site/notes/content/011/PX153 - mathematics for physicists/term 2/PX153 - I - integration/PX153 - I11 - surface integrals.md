---
dg-publish: true
---

$$\iint_{S} \phi\,dS \; or \; \iint_{S} \vec a \cdot d\vec S \; or \; \iint_{S} \vec a \times d\vec S \; or \; \iint_{S} a\, d\vec S$$
- $d\vec S$ is a surface element that represents $dS\,\hat n$, where $dS$ is an infinitesimal area, and $\hat n$ is the normal to the surface element (3D vector with a magnitude of 1)

- formally, dividing $S$ into $N$ elements, each with an area, $\Delta S_{p}$, where $p=1,...N$, and each surface element is assigned its normal, $\hat n_{p}$: 
$$\iint_{S} \vec a \cdot d\vec S = \lim_{N\to\infty} \sum\limits_{p=1}^{N} \vec a (\bar x_{p}, \bar y_{p}, \bar z_{p}) \cdot \Delta S_{p}\hat n_{p}$$ 
$$d\vec S = r^{2}\sin\theta \, d\theta \, d\phi$$
- eg: what is the vector area of the hemisphere?
	$$I = \int_{S} 1\,d\vec S$$
		$x^{2}+y^{2}+z^{2}=a^{2}$
		$d\vec S = a^{2}\sin\theta \, d\theta\, d\phi\, \hat r$
$$\begin{align*}
	I &= \int_{0}^{2\pi} \int_{0}^{\frac{\pi}{2}} (\sin\theta \cos\phi\, \hat i + \sin\theta \sin\phi\, \hat j + \cos\theta\, \hat k) a^{2}\sin\theta\, d\theta\, d\phi \\
	&= \int_{0}^{2\pi} \int_{0}^{\frac{\pi}{2}} \cos\theta\, \hat k \, a^{2}\sin\theta \, d\theta\, d\phi \\
	&= a^{2} \hat k \int_{0}^{2\pi} \frac{1}{2} \left[- \frac{\cos(2\theta)}{2}\right]_{0}^\frac{\pi}{2}d\phi \\
	&= a^{2} \hat k \int_{0}^{2\pi} \frac{1}{2}\, d\phi \\
	&= a^{2}\pi\,d\phi
\end{align*}$$
## flat surface
- eg: $S$ is area $0\leq x\leq1,\; 0\leq x\leq1$. compute: $I = \iint \vec\nabla\phi\cdot d\vec S$ , where, $\phi=xyz$	
	- **convention**: the sense of the normal is defined by the orientation at the boundary: follows the right hand thumb rule
		$\vec\nabla\phi = (yz,\, xz,\, xy)$ 
		$d\vec S = (0,0,dx\,dy)$ (integrating over an infinitesimal area, $dx\,dy$)
	$$I = \int_{0}^{1}\int_{0}^{1} xy\,dx\,dy =...= \frac{1}{4}$$
