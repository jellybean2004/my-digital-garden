---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/a-differentiation/2-advanced-a3-a4-and-a5/px-275-a3a-the-chain-rule/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:01.503+00:00"}
---

- consider the elevation $h(x,y)$ at a point P(x,y)
![Pasted image 20241004170519.png](/img/user/pics/Pasted%20image%2020241004170519.png)
- walk a distance, $s$, to get to the point, $P$
- height changes during the walk
- how does the height vary during the walk?
- movement along $x+y$ is given by $\frac{dx}{ds}$ and $\frac{dy}{ds}$
- change in height is given in terms of $x$ and $y$ by the total differential: 
$$\begin{align*}
	dh &= \frac{\partial h}{\partial x}dx + \frac{\partial h}{\partial y}dy \\
	dh &= \frac{\partial h}{\partial x} \frac{dx}{ds}ds + \frac{\partial h}{\partial y} \frac{dy}{ds} ds \\
	\therefore\frac{dh}{ds} &= \frac{\partial h}{\partial x} \frac{dx}{ds}+ \frac{\partial h}{\partial y} \frac{dy}{ds}
\end{align*}$$
