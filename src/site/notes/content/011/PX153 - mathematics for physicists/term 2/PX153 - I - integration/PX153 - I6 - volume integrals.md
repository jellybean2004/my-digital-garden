---
dg-publish: true
---

- so far, cartesian coordinates have been used. a more general 2D integral: 
$$A = \iint_{R}f(\vec r).dA$$
	where, $\vec r = (x,y,z)$

- for volume integrals: 
$$I = \iiint_{V} f(\vec r).dV$$
	where, $dV = dx.dy.dz$ in cartesian coordinates

- eg: what is the mass of a cube, $-L \leq x,y,z \leq L$ , with $\rho(\vec r) = \rho_{0}(1+x)$
$$\begin{align}
	M &= \int_{-L}^{L} \int_{-L}^{L} \int_{-L}^{L} \rho_{0}(1+x).dx.dy.dz \\
	&= \int_{-L}^{L} \int_{-L}^{L} 2L\rho_0 .dy.dz \\
	&= 2L \rho_{0}[y]_{-L}^{L} [z]_{-L}^{L} \\
	&= \rho_{0}(2L)^{3} \\
	\therefore M &= \rho_{0}V
\end{align}$$
