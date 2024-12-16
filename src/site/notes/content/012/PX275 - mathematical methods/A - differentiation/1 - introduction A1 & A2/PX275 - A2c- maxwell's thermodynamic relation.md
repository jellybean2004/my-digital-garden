---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/a-differentiation/1-introduction-a1-and-a2/px-275-a2c-maxwell-s-thermodynamic-relation/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:03:57.821+00:00"}
---

$$\begin{align} 
	dU &= T\,dS-p\,dV \tag{1}\\
	df &= \frac{\partial f}{\partial x}\,dx + \frac{\partial f}{\partial y}\,dy \tag{2} \\
\end{align}$$
- comparing (1) and (2): 
$$\begin{gather}
		T = \frac{\partial U}{\partial S} & \\
		\implies\frac{\partial T}{\partial V} = \frac{\partial^{2} U}{\partial V \partial S}\\\\
		\text{and,}
		-p = \frac{\partial U}{\partial V} \\
		\implies- \frac{\partial p}{\partial S} = \frac{\partial^{2}U}{\partial S \partial V} \\\\
		\boxed{\therefore \frac{\partial T}{\partial V} = -\frac{\partial p}{\partial S}}
\end{gather}$$
- this is one of the four *maxwell's thermodynamic relations*
