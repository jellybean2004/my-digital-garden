---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b1-coordinate-systems/px-275-b1d-time-derivatives/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:33.190+00:00"}
---

- in cartesians: $\vec r = r_{x}\hat i + r_{y}\hat j + r_{z}\hat k$
- the velocity: 
$$\begin{align*}
	\vec v &= \left(\frac{dr_{x}}{dt}\hat i +\frac{d\hat{i}}{dt} r_{x}\right) + \left(\frac{dr_{y}}{dt}\hat j +\frac{d\hat{j}}{dt} r_{y}\right) + \left(\frac{dr_{z}}{dt}\hat k +\frac{d\hat{k}}{dt} r_{z}\right) \\
	&= \frac{dr_{x}}{dt}\hat i + \frac{dr_{y}}{dt}\hat j + \frac{dr_{z}}{dt}\hat k \;[\because \text{the basis vectors do not change in time}]
\end{align*}$$
- in cylindrical polars: $\vec r = \rho \hat e_\rho(\phi) + z \hat e_{z}$
- the velocity: 
$$\vec v = \left(\frac{d\rho}{dt}\hat e_{\rho} + \rho \frac{d\hat{e}_{\rho}}{dt}\right) + \left(\frac{dz}{dt}\hat e_{z} + z \frac{d\hat{e}_{\rho}}{dt} \right)$$
- $\frac{d\hat{e}_{\rho}}{dt}\neq 0$, so using: 
$$\begin{align*}
	\hat e_{\rho}&= \cos\phi \hat i + \sin\phi \hat j \\
	\frac{d\hat{e}_{\rho}}{d\phi} &=  -\sin\theta\hat{i} + \cos\phi\hat{j} \\ 
	&\equiv \hat e_{\phi} \\\\
	\implies \frac{d\hat{e}_{\rho}(\phi)}{dt} &= \frac{d\hat{e}_{\rho}}{d\phi} \frac{d\phi}{dt} \\
	&= \frac{d\phi}{dt}\hat e_{\phi}
\end{align*}$$
$$\therefore\vec v = \frac{d\rho}{dt}\hat e_{\rho} + \rho \frac{d\phi}{dt} \hat{e}_{\phi} + \frac{dz}{dt}\hat e_{z}$$
