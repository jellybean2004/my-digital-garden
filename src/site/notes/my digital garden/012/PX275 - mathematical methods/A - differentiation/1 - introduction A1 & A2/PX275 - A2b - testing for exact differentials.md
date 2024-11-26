---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/a-differentiation/1-introduction-a1-and-a2/px-275-a2b-testing-for-exact-differentials/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:03:54.853+00:00"}
---

- for a function, $f(x,y)$, the total differential is: 
	$$df = \left(\frac{\partial f}{\partial x}\right)dx + \left(\frac{\partial f}{\partial y}\right)dy$$
- writing $\frac{\partial f}{\partial x}$ as $A$, and $\frac{\partial f}{\partial y}$ as $B:$ 
  $$df = A\,dx + B\,dy$$
- now, differentiating $A$ and $B$ wrt ${} y$ and ${} x$ respectively: 
$$\begin{gather*}
		\frac{\partial A}{\partial y} = \frac{\partial }{\partial y}\left(\frac{\partial f}{\partial x}\right) = \frac{\partial ^{2}f}{\partial y \partial x}\\
		\frac{\partial B}{\partial x} = \frac{\partial }{\partial x}\left(\frac{\partial f}{\partial y}\right) = \frac{\partial ^{2}f}{\partial x \partial y}\\\\
		\therefore \frac{\partial A}{\partial y}= \frac{\partial B}{\partial x}
\end{gather*}$$
- if $\frac{\partial A}{\partial y} \neq \frac{\partial B}{\partial x}$, it is an inexact differential, ie: $f(x,y)$ does not exist