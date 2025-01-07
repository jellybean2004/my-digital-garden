---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/a-differentiation/1-introduction-a1-and-a2/px-275-a1-partial-differentiation/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:03:46.292+00:00"}
---

- for a function, $f(x,y)$, partial differentials can be defined as $\left(\frac{\partial f}{\partial x}\right)_{y}$; $\left(\frac{\partial f}{\partial y}\right)_{x}$
$$\begin{align*} 
	\frac{\partial }{\partial x} \left(\frac{\partial f}{\partial x}\right) &= \frac{\partial ^{2}f}{\partial x^{2}} \\
	\frac{\partial }{\partial y} \left(\frac{\partial f}{\partial y}\right) &= \frac{\partial ^{2}f}{\partial y^{2}}
\end{align*}$$ $$\frac{\partial ^{2}f}{\partial x\partial y} = \frac{\partial ^{2}f}{\partial y\partial x}$$

$$\frac{\partial ^{2}f}{\partial x\partial y} = \frac{\partial ^{2}f}{\partial y\partial x}$$
- the above property is always true for "well-behaved functions" routinely encountered in physics

- **note:** $\frac{\partial }{\partial x}$ and ${} \frac{\partial }{\partial y}$ are *operators* acting on a function
- if $f(x) = \sin(x)$, $\frac{\partial }{\partial x} {\sin{x}}$ is not the same as $\sin{x}\frac{\partial }{\partial x}$
- for $\frac{\partial ^{2}f}{\partial x\partial y} = \frac{\partial ^{2}f}{\partial y\partial x}$ to be true, (implies that the order of the operators can be swapped), $\frac{\partial }{\partial x} \left(\frac{\partial f}{\partial y}\right) = \frac{\partial }{\partial y} \left(\frac{\partial f}{\partial x}\right)$

- in general, with operators, the order of operation is important
