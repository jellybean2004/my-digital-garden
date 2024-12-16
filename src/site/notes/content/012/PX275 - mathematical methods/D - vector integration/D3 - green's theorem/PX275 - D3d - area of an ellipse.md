---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/d-vector-integration/d3-green-s-theorem/px-275-d3d-area-of-an-ellipse/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:47.954+00:00"}
---

![Pasted image 20241114121218.png](/img/user/pics/Pasted%20image%2020241114121218.png)
- an ellipse is defined by: 
$$\begin{align*}
	x &= a\cos\phi \\
	y &= b\sin\phi \\
	&0 \leq \phi\leq 2
\end{align*}$$
taking the differentials of $x$ and $y:$ 
$$\begin{align*}
	dx &= - a\sin\phi\,d\phi \\
	dy &= b\cos\phi\,d\phi
\end{align*}$$
- writing: $Q=x$ and $P=-y:$ 
$$\begin{align*}
	2A &= \oint_{C} x\,dy - y\,dx = \iint_R \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \,dA \\
	2A &= \oint_{C }(a\cos\phi) (b\cos\phi\,d\phi) - (b\sin\phi)( - a\sin\phi\,d\phi) \\ 
	A &= \frac{ab}{2}\oint_{C} \cos^{2}\phi + \sin^{2}\phi \,d\phi \\ 
	&= \frac{ab}{2}\oint_{C}d\phi \\
	\therefore A &= \pi ab
\end{align*}$$
