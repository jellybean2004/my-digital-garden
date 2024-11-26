---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b1-coordinate-systems/px-275-b1e-spherical-polar-coordinates/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:35.341+00:00"}
---

![Pasted image 20241017121142.png](/img/user/pics/Pasted%20image%2020241017121142.png)
- transformations: 
$$\begin{gather*}
	x &= \rho\cos\phi &= r\sin\theta\cos\phi \\
	y &= \rho\sin\phi &=  r\sin\theta\sin\phi \\
	z &= r\cos\theta
\end{gather*}$$
- limits: 
$$\begin{gather*}
	\theta \in [0,\pi] \\
	\phi \in [0,2\pi] \\
	\rho \in [0,\infty)
\end{gather*}$$
## surface and volume elements
![Pasted image 20241017121423.png](/img/user/pics/Pasted%20image%2020241017121423.png)
- the surface element: 
$$dS = d\phi \cdot r d\theta= r^{2}\sin\theta\,d\phi\,d\theta$$
- the volume element: 
$$dV = r^{2}\sin\theta\,d\phi\,d\theta\,dr$$