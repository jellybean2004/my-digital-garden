---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/a-differentiation/2-advanced-a3-a4-and-a5/px-275-a3c-change-of-variables-and-coordinate-system/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:07.044+00:00"}
---

## cylindrical coordinates
![Pasted image 20241004170604.png](/img/user/pics/Pasted%20image%2020241004170604.png)
$$P(x,y) \to P(\rho,\theta)$$
	$x=\rho\cos\theta$ 
	$y=\rho\sin\theta$ 
	$\rho^{2}=x^{2}+y^{2}$ 
	$\tan\theta=y/x$

- $x$ and $y$ are functions of $\rho$ and $\theta$

- at any point, $P$, the function has a particular value, independent of the co-ordinate system used: $f(x,y)=g(\rho,\theta)$
- for a small step: $\rho\to\rho+d\rho$, $\theta\to\theta+d\theta$ 
- using the chain rule: $f(x,y)=g(\rho,\theta):$ 
$$\begin{gather}
	\frac{\partial g}{\partial \rho} &= \frac{\partial f}{\partial x} \frac{\partial x}{\partial \rho} + \frac{\partial f}{\partial y} \frac{\partial y}{\partial \rho} &= \cos\theta \frac{\partial f}{\partial x} + \sin\theta \frac{\partial f}{\partial y} \\
	\frac{\partial g}{\partial \theta} &= \frac{\partial f}{\partial x} \frac{\partial x}{\partial \theta} + \frac{\partial f}{\partial y} \frac{\partial y}{\partial \theta} &= -\rho\sin\theta \frac{\partial f}{\partial x} + \rho\cos\theta \frac{\partial f}{\partial y}
\end{gather}$$
- considering these expressions as operators, 
$$\begin{align*}
	\frac{\partial }{\partial \rho} &= \cos\theta \frac{\partial }{\partial x} + \sin\theta \frac{\partial }{\partial y} \\
	\frac{\partial }{\partial x} &= \cos\theta \frac{\partial }{\partial \rho}  - \frac{1}{\rho} \sin\theta \frac{\partial }{\partial \theta} \\
	\frac{\partial }{\partial y} &= \sin\theta \frac{\partial }{\partial \rho}  + \frac{1}{\rho} \cos\theta \frac{\partial }{\partial \theta}
\end{align*}$$
