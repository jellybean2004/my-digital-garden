---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/h-gases/px-284-h1-density-of-states-dos/","noteIcon":"1","created":"2025-01-09T15:13:21.746+00:00","updated":"2025-01-09T15:32:45.000+00:00"}
---

#incomplete [[qm link\|qm link]]

- considering a cloud of particles contained inside a cubic box of side, $L$
- the box is bounded by: $-L/2 \leq x,y,z \le +L/2$

- the wavefunction of a single particle is:
$$\psi_{x} = Ae^{ik_{x}x}$$
	where, $k_{x}$ is the $x$-component of the wavevector, ${} |\vec k| = 2\pi/\lambda {}$
- and similarly for $\psi_y$ and $\psi_z$
- by symmetry, the wavefunction must be the same at either edge of the box, ie:
$$\psi_{x}\left({L}/{2}\right) = \psi_{x}\left(-{L}/{2}\right)\implies e^{ik_{x}L/2} = e^{-ik_{x}L/2}$$
- this is only satisfied if 
$$k_{x} = \cfrac{2\pi}{L} n_{x}$$ 
	where, $n_{x}\in \mathbb{Z}$
- similarly, 
$$\begin{gather}
k_{y} = \cfrac{2\pi}{L} n_{y} \\
k_{z} = \cfrac{2\pi}{L} n_{z}
\end{gather}$$
- thus, the wavevector is quantised into allowed states
- considering that the particles are equally distributed along the cube, with a separation of $2\pi/L$

- in 3D, the volume occupied by one $k$-state is: $2\pi/L \times  2\pi/L \times 2\pi/L$

>[!info] density of states
>$g(k)$ is defined by $g(k)\,dk =$  number of allowed states with wavevector whose magnitudes lie between $k$ and $k+dk$

- in 3D, this must be given by the volume of spherical shell of thickness, $dk$, and radius, $k$, divided by the volume of one $k$-state:
$$g(k)\, dk = 4\pi k^{2}\,\frac{dk}{(2\pi/L)^{3}}$$
$$\boxed{g(k)\,dk = \frac{Vk^{2}}{2\pi}dk}$$
	where, $V$ is the volume of the container

