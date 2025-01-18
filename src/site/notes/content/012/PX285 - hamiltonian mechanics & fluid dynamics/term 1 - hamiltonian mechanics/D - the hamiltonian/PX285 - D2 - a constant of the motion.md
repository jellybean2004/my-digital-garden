---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/d-the-hamiltonian/px-285-d2-a-constant-of-the-motion/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:04.184+00:00"}
---

- taking the time derivative of the hamiltonian: 
$$\frac{dH}{dt} = \frac{d}{dt}\left(\dot x \frac{\partial L}{\partial \dot x} -L\right)$$
- for a function, $f(a,b,t)$, its time derivative is: 
$$\frac{df}{dt} = \frac{\partial f}{\partial a}\frac{\partial a}{\partial t} + \frac{\partial f}{\partial b}\frac{\partial b}{\partial t} + \frac{\partial f}{\partial t}$$
- for $L(x,\dot x,t):$ 
$$\begin{align*}
	\frac{dH}{dt}&= \frac{d}{dt}\left(\dot x \frac{\partial L}{\partial \dot x}\right) - \left(\frac{\partial L}{\partial x}\frac{\partial x}{\partial t} + \frac{\partial L}{\partial \dot x}\frac{\partial \dot x}{\partial t} + \frac{\partial L}{\partial t} \right) \\
	&= \dot x \left(\frac{d}{dt} \frac{\partial L}{\partial \dot x} - \frac{\partial L}{\partial \dot x}\right) - \frac{\partial L}{\partial t} \\
	\therefore \frac{dH}{dt}&= -\frac{\partial L}{\partial t}
\end{align*}$$
	using the euler-lagrange equation, $\frac{\partial L}{\partial x} - \frac{d}{dt}\frac{\partial L}{\partial \dot x}=0$

- if the lagrangian has no *explicit* time dependence, ie: $L(x,\dot x):$ 
$$\frac{dH}{dt} = 0$$
- the hamiltonian is conserved for the case
