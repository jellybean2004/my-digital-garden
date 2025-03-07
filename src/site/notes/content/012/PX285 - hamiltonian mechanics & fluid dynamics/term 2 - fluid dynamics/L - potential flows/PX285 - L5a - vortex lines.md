---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l5a-vortex-lines/","noteIcon":"1","created":"2025-03-07T13:30:52.407+00:00","updated":"2025-03-07T13:40:15.876+00:00"}
---

- the flow around a vortex:
$$\vec u = \frac{K}{2\pi r} \hat \theta$$
	where, $K = \oint \vec y \cdot d\vec l$ is the circulation around any closed loop enclosing the axis, $r = 0$

- if the rotation axis is not attached to a material object, the vortex is called a **free vortex** or **vortex line**

![PX285 - L5 - vortex lines.png|500](/img/user/pics/PX285%20-%20L5%20-%20vortex%20lines.png)

- the closed path above does not enclose the vortex line
- the total circulation is:
$$\begin{align*}
\oint \vec u \cdot d\vec l  &= \int_{\Gamma_{A}} \vec u \cdot d\vec l  + \int_{L_{AB}} \vec u \cdot d\vec l  + \int_{\Gamma_{B}}\vec u \cdot d\vec l  + \int_{L_{BA}} \vec u \cdot d\vec l  \\
&= \int_{\Gamma_{A}} \vec u \cdot d\vec l  + \int_{\Gamma_{B}}\vec u \cdot d\vec l
\end{align*}$$
- this is because the paths $L_{AB}$ and $L_{BA}$ cancel
$$\implies \int_{\Gamma_{A}} \vec u \cdot d\vec l  = - \int_{\Gamma_{B}}\vec u \cdot d\vec l$$
- $\Gamma_{A}$ and $\Gamma_{B}$ are in opposite directions around the vortex line
- if $\Gamma_{B}$ is changed such that both are clockwise, $\oint \vec u \cdot d\vec l$ around the vortex line in a fixed direction is constant along the line
