---
dg-publish: true
---
- *what causes the emf in [[content/011/PX157 - electricity and magnetism/PX157 - D - induction/PX157 - D1b - a moving crossbar\|a moving crossbar]]?*
![Pasted image 20240226181250.png](/img/user/pics/Pasted%20image%2020240226181250.png)
- inside the moving crossbar, there are free charges, $q$, moving at a velocity, $\vec v$, across the magnetic field, $\vec B$
- [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C1a - the lorentz force\|the lorentz force]] on the conducting (free) charges, $q:$
$$
\vec F = q\vec v\times \vec B = qvB \,\hat x\times (-\hat z) = + qvB\,\hat y
$$
- positive charges accumulate at point $a$ (top), and negative charges at point $b$ (bottom)
- charge separation leads to an electric field:
$$
\vec E = -E\,\hat y
$$
- electric field creates a force (opposite to the lorentz force):
$$
\vec F = - qE\,\hat y
$$
- in a steady state, the total force is zero:
$$\begin{align*}
	q\vec E + q\vec v\times \vec B &= \vec 0 \\
	\vec E = -\vec v\times\vec B &= -vB\,\hat y
\end{align*}$$
- the voltage between points $a$ and $b:$
$$
V= EL = vLB
$$
- the induced electric field (emf) is due to moving charges, the magnetic lorentz force is called a *motional emf*
- emf, $\epsilon$, is the work done per unit charge moving around a closed loop:
$$\begin{align*}
	\epsilon &= \frac{W}{q} \\
	&= \frac{1}{q}\oint \vec F \cdot d\vec l \\
	&= \oint (\vec E + \vec v\times \vec B)\cdot d\vec l
\end{align*}$$
- the part due to the motion, $\vec v$, is the total motional emf around a closed loop:
$$
\epsilon = \oint_{loop} (\vec v \times \vec B) \cdot d\vec l
$$
