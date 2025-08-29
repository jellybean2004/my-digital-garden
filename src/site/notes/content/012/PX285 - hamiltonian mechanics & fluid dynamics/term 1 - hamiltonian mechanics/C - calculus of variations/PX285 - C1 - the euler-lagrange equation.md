---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/c-calculus-of-variations/px-285-c1-the-euler-lagrange-equation/","noteIcon":"1","created":"2025-08-27T13:14:16.110+01:00","updated":"2024-12-09T10:55:41.000+00:00"}
---

- *calculus of variations* is a technique to find the function that extremizes the integral provided that the end points are fixed
- taking a path, $x(t)$, and varying it as: 
$$\begin{gather}
	x(t) \to x(t) + a(t) \\
	\implies v(t) \to v(t) + \dot a(t)
\end{gather}$$
- $x(t)$ is the extremal path from $x_{0}(t_{0})$ to $x_{1}(t_{1})$, and $a(t)$ is a general, **small** excursion that the path is forced to take, but it must always pass through its fixed end points: $a(t_{0}) = a(t_{1}) = 0$
- considering $L(x,v)$, and taking a small pertubation: $L(x+a,v+\dot a)$ like a taylor expansion, where only the first order variation is of interest: 
$$L(x+a,v+\dot a) \approx L(x,v) + a \frac{\partial L}{\partial x} + \dot a \frac{\partial L}{\partial \dit x} + \dots$$
- by definition, $A = \int_{t_{0}}^{t_{1}} L(x,\dot x)\,dt$, with $x(t)$ as the extremal path, and $A$ as the extremal action: 
$$\begin{gather*}
	A \to A + \delta A \\
	\text{where, } \delta A = \int_{t_{0}}^{t_{1}} \left[a(t) \frac{\partial L}{\partial x} + \dot a(t) \frac{\partial L}{\partial \dot x}\right]\,dt \\
\end{gather*}$$
- using integration by parts on the second term: 
$$\int dt\frac{da}{dt}\frac{\partial L}{\partial \dot x} = \left[a(t) \frac{\partial L}{\partial \dot x}\right]_{t_{0}}^{t_{1}} - \int a(t) \frac{d}{dt}\frac{\partial L}{\partial \dot x} \,dt$$
- $[a(t)]_{t_{0}}^{t_{1}}$ must be equal to zero as the variations vanish at the end points: 
$$\delta A = \int dt\,a(t) \left(\frac{\partial L}{\partial x} - \frac{d}{dt} \frac{\partial L}{\partial v}\right)$$
- the only way $A$ can be stationary, ie: $\delta A =0$, is if the following **euler-lagrange equation** is satisfied: 
$$\frac{\partial L}{\partial x}- \frac{d}{dt}\frac{\partial L}{\partial v} = 0$$
