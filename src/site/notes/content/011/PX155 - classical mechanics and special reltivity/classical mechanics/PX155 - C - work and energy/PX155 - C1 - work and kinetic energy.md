---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-c-work-and-energy/px-155-c1-work-and-kinetic-energy/","created":"2024-10-01T18:27:09.511+01:00","updated":"2024-11-26T19:55:22.286+00:00"}
---

- from *[[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - B - systems of particles, accelerations/PX155 - B4 - equations of motion#^f972e4\|this equation]]*
$$\int a(x)dx = \int v dv$$
- aside:
$$\int_u^v v.dv = \frac{1}{2}\int_{u^2}^{v^2} d(v^2) = \frac{1}{2}[v^2]_{u^2}^{v^2}$$
	so,
$$\int a(x) dx = \frac{1}{2}\int d(v^2)$$
- if it is a particle of mass $m$:
$$\int F(x) dx= \frac{1}{2}m\int d(v^2)=\int dT=\Delta T$$
		where, $T= \frac{1}{2}mv^2$
- $\int F(x)dx = \Delta T$ is work done $W$
- **if $F$ is constant**, so not a function of position,$$W=\int_{x_A}^{x_{B}}Fdx= F(x_B-x_A)$$ 
$$W=F\Delta x$$
- however, often in infinitesimal step where $F(x)$ can be considered constant
$$dW=F(x)dx=dT$$
## work in 3D
- above generalises to $dW=F_xdx+F_ydy+F_zdz$ 
	- $\vec F=(F_x,F_y,F_z)$
	- $dW=\vec F\cdot d\vec r$
		- $\vec dr = (dx,dy,dz)$
		- in x-direction: $F_xdx = \frac{m}{2}d(v_2^2)$, similar for y and z
		- therefore,
$$T= \frac{1}{2}m(v_x^2+v_y^2+v_z^2)$$
		- so,
$$dW=dT$$
		- so in 3D, $T= \frac{1}{ m}\vec v \cdot \vec v = \frac{1}{2}m|\vec v|^2= \frac{1}{2}mv^2$
			- where,  $v=|\vec v|$
		- and,
$$W=\int\vec F d\vec r = \Delta T$$
		- work done by $\vec F$ along a "slice" of the path $d \vec r$:
$$dW=\vec F d\vec r =F\cos{\theta}dr$$
			- $dW$ is the position of $\vec F$ along the path times an infinitesimal distance moved during that path
