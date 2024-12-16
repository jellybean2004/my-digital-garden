---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b2-4-integration/px-275-b3-jacobian/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:49.574+00:00"}
---

- the change of variables have been made geometrically, but this can be done in a more generalized way via a method using a construct called a *jacobian*
- to transform from $(x,y,z) \to (u,v,w)$, the jacobian for this transformation is written as:
$$J = \frac{\partial (x,y,z)}{\partial (u,v,w)}$$
$$dV = dx\,dy\,dz = |J|\,du\,dv\,dw$$
	where, $|J|$ is the absolute value of the jacobian
## plane polar 
$$J = \frac{\partial (x,y)}{\partial (p,\phi)} = \left| \begin{matrix} \frac{\partial x}{\partial \rho} & \frac{\partial x}{\partial \phi} \\ \frac{\partial y}{\partial \rho} & \frac{\partial y}{\partial \phi} \end{matrix} \right|$$
- remember: 
		$x = \rho\cos\phi$
		$y = \rho\sin\phi$
$$J = \rho\cos^{2\phi} - (-\rho\sin)^{2}\phi = \rho$$
- area: 
$$dA = dx\,dy = |J|\,d\rho\,d\phi = \rho\,\,d\rho\,d\phi$$
## spherical polar
$$ J = \left| \begin{matrix} \frac{\partial x}{\partial r} & \frac{\partial x}{\partial \theta} & \frac{\partial x}{\partial \phi} \\ \frac{\partial y}{\partial r} & \frac{\partial y}{\partial \theta} & \frac{\partial y}{\partial \phi} \\ \frac{\partial z}{\partial r} & \frac{\partial z}{\partial \theta} & \frac{\partial z}{\partial \phi} \end{matrix} \right|$$
- remember:
		$x = r\sin\theta\cos\phi$
		$y = r\sin\theta\sin\phi$
		$z = r\cos\theta$
$$\begin{gather}
	J  = r^{2}\sin\theta \\
	dV = r^{2}\sin\theta \,dr\,d\theta\,d\phi
\end{gather}$$

