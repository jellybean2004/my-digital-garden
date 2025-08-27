---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-i-integration/px-153-i6-volume-integrals/","noteIcon":"1","created":"2025-08-27T13:14:05.092+01:00","updated":"2024-11-26T19:38:11.000+00:00"}
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
