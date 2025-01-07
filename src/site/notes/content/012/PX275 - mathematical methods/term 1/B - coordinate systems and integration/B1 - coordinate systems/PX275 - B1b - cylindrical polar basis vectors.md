---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/b-coordinate-systems-and-integration/b1-coordinate-systems/px-275-b1b-cylindrical-polar-basis-vectors/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:28.656+00:00"}
---

![Pasted image 20241015150304.png](/img/user/pics/Pasted%20image%2020241015150304.png)
- **note:** only $\vec e_{z}$ is always in the same direction, $\vec e_\rho$ and $\vec e_\phi$ change directions wrt the axes
- it is only in cartesian coordinates that the basis vectors hold their positions for all points in space
- the position vectors, eg: $\vec r$, should only be defined in the cartesian space
	- eg: at a point, $P_{1}: \vec r = x\hat{i} + y\hat{j} + x\hat{k} = \rho\cos\phi\hat{i} + \rho\sin\phi\hat{j} + z\hat{k}$
- the new basis vectors are related to $\hat i$, $\hat j$, $\hat k$ by taking the derivative of $\vec r$ wrt $\rho, \phi,z:$ 
$$\begin{align*}
	\frac{\partial \vec r}{\partial z} = \vec e_{z} &= \hat k \\
	\frac{\partial \vec r}{\partial x} = \vec e_{\rho} &= \cos\phi \hat i + \sin\phi\hat j \\
	\frac{\partial \vec r}{\partial y} = \vec e_{\phi} &= -\rho\sin\phi \hat i + \rho\cos\phi\hat j
\end{align*}$$
- $|\vec e_{z|}= |\vec e_\rho| =1\implies$ they are unit vectors, ie: $\hat e_{z}= \vec e_{z}$ and ${} \hat e_{\rho} = \vec e_{\rho} {}$
- but, $|\vec e_\phi|=\rho$, so, $\hat{e}_{\phi} = \frac{\vec e_{\phi}}{\rho}$

- **note:**
	- $\vec r \neq \rho \hat e_{\rho} + \phi \hat e_{\phi} + z \hat e_{z}$, as $\rho,\phi$ are not fixed wrt the axes
	- it can be written as: $\vec r = \rho \hat e_\rho(\phi) + z\hat e_{z}$
	- a vector field at $P$ will typically have components along the three directions: $\vec F = F_{x}\hat i + F_{y}\hat j + F_{z}\hat k = F_{\rho} \hat e_{\rho} + F_{\phi} \hat e_{\phi} + F_{z}\hat e_{z}$
