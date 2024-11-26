---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/a-introduction/px-285-a2b-angular-momentum/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:46.661+00:00"}
---

- eg:

	- $\vec\omega = \omega\,\hat n$, $\vec r$ at an angle $\theta$
	$$\begin{align*}
	\vec v &= \vec\omega\times\vec r \\
	&= \vec\omega \times (r\cos\theta\,\hat{n}+ r\sin\theta\,\hat{x})\\
	&= \vec\omega \times \hat{x} r\sin\theta \\
	&= \hat{v}\,r\sin\theta\,\omega
	\end{align*}$$
	 $\vec\omega\times\vec x = \omega\,\hat{v}$ 
- using the fact that all mass elements, $m_{i}$ (atoms), in a solid body rotate about the same axis if the body is rotated: 
$$\vec v_{i} = \vec\omega\times \vec r_{i}$$
$$\begin{align*}
	\vec L &= \sum\limits_{i}m_{i}\vec r_{i} \times (\vec\omega\times\vec r_{i}) \\
	 &= \sum\limits_{i}m_{i}\,[\vec\omega(\vec r_{i}\cdot\vec r_{i})-\vec r_{i}(\vec r_{i}\cdot\vec\omega)]
\end{align*}$$
$$\begin{align*}
	\implies L_{x}&= \sum\limits_{i} m_{i}[\omega_{x}(\vec r_{i}\cdot \vec r_{i}) - x_{i}(x_{i}\omega_{x}+y_{i}\omega_{y}+ z_{i}\omega_{z})] \\
	&= \omega_{x}\sum\limits_{i}m_{i}(\vec r_{i}\cdot \vec r_{i} -x_{i}^{2})+ \omega_{y} \sum\limits_{i}m_{i}(-x_{i}\,y_{i})+ \omega_{z} \sum\limits_{i}m_{i}(-x_{i}\,z_{i}) \\
\end{align*}$$
- let: 
$$\begin{align*}
	I_{xx}&= \sum\limits_{i}m_{i}(\vec r_{i}\cdot \vec r_{i}), \\
	I_{xy}&= \sum\limits_{i}m_{i}(-x_{i}\,y_{i}), \\
	I_{xz}&= \sum\limits_{i}m_{i}(-x_{i}\,z_{i}). \\\\
	\therefore L_{x} &= I_{xx}\omega_{x} -x_{i}^{2} + I_{xy}\omega_{y} + I_{xz}\omega_{z} \\
\end{align*}$$
- it can be asserted that: 
$$\begin{align*}
	L_{y} &= I_{yx}\omega_{x} -x_{i}^{2}+ I_{yy}\omega_{y} + I_{yz}\omega_{z} \text{ ;}\\
	L_{z} &= I_{zx}\omega_{x} -x_{i}^{2}+ I_{zy}\omega_{y} + I_{zz}\omega_{z}
\end{align*}$$
- define a matrix: 
$$I = \begin{bmatrix}I_{xx} & I_{xy} & I_{xz} \\ I_{yx} & I_{yy} & I_{yz} \\ I_{zx} & I_{zy} & I_{zz}\end{bmatrix}$$
- then: 
$$\vec L = I\,\vec\omega$$
- eg: calculate the kinetic energy of rotation
$$\begin{align}
	T_{rot} &= \frac{1}{2}\sum\limits m_{i}\vec v_{i}\cdot \vec v_{i} \sim \frac{1}{2}mv^{2} \\
	&= \frac{1}{2}\sum\limits m_{i}\vec v_{i}\cdot(\vec \omega\times\vec r_{i}) \\
	&= \frac{1}{2}\sum\limits m_{i}\vec\omega\cdot(\vec r_{i}\times \vec v_{i}) \\
	&= \frac{1}{2} \vec\omega\cdot\sum\limits m_{i}(\vec r_{i}\times \vec v_{i}) \\
	&= \frac{1}{2}\vec\omega\cdot \vec L \\
	&= \frac{1}{2}\vec\omega\cdot I\cdot \vec\omega \\
	&= \frac{1}{2}\omega^{2}[\hat{n}\cdot I\hat{n}] \\
	\therefore T_{rot}&= \frac{1}{2}I\omega^{2} \tag{1}
	\end{align}$$
- comparing $(1)$ with $T=\frac{1}{2}mv^{2}$, $I$ must have dimensions of $[ML^{2}]:$ 
$$T = \frac{1}{2}I\omega^{2}= \frac{1}{2}I\,\dot\theta^{2}$$
$$\begin{align*} 
I &= \hat{n} \cdot \frac{1}{2} \vec{L} \\\\
\frac{1}{2}I\omega^{2} &= \frac{1}{2}\omega\,\hat{n}\cdot L \\
&= \frac{1}{2}\vec\omega\cdot\vec L \\\\
I &= \hat{n}\cdot \sum\limits_{i}m_{i}(\hat{n} (\vec{r}_{i}\cdot\vec{r}_{i})- \vec r_{i}(\vec r_{i}\cdot \hat{n})) \\
&= \sum\limits_{i} m_{i} \left[ \vec r_{i}\cdot \vec r_{i}-(\vec r_{i} \cdot\hat n)^{2} \right]
\end{align*}$$
- continuum limit exists: 
$$\sum\limits_{i}m_{i}\to \sum\limits_{i} \rho_{i}\,\Delta V_{i} \to \int \rho(\vec r) \,dV$$

- consider a cylinder having a length, $l$, a radius, $r$, and a constant density, ${} \rho$
$$\begin{align*}
I &= \int \rho(r)\,dV[\vec r\cdot\vec r- (\vec r\cdot\hat z)^{2}] \\
&= \sum\limits_{i}m_{i}[(x^{2}+y^{2}+z^{2}) -z^{2}] \\
\therefore I &= \sum\limits_{i}m_{i}\, \tilde{r}^{2}
\end{align*}$$
	where, $\tilde r=x^{2}+y^{2}$

- considering cylindrical coordinates: $dV = dx\,dy\,dz = \tilde r\,d\tilde r\,d\theta\, dz$
$$\begin{align*}
	I &= \int_{0}^{2} \rho\,\tilde r\,d\tilde r \int_{0}^{2\pi} d\theta\int_{0}^{l}dz\,\tilde r^{2} \\
	\therefore I &= \frac{\pi\,l\,\rho\,R^{4}}{2} \\\\
	\implies T_{rot} &= \frac{1}{2}\left(\frac{\pi\,l\,\rho\,R^{4}}{2}\right)\, \omega^2
\end{align*}$$
- for a cylinder rotating through the centre of mass: 
$$T_{tot} = T_{rot}+T_{trans}$$
