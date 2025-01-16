---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/h-introduction-to-fluids/px-285-h6b-example-of-a-flow/","noteIcon":"1","created":"2025-01-16T14:52:04.743+00:00","updated":"2025-01-16T14:52:42.825+00:00"}
---

- considering a flow between two parallel plates at $a$ and $-a$

![PX285 - H6 - stream line-1.png|500](/img/user/pics/PX285%20-%20H6%20-%20stream%20line-1.png)

- the assumptions:
	- laminar (1D, $\parallel \hat x$, no vortices)
	- steady (time independent)
	- viscous ($\mu$ is important)
$$\vec u = u_{x}(y)\hat x$$
- the boundary conditions:
	$\vec u(y = -a, a) = 0$
- the steady motion requires a force which counteracts the viscous force
- let it be the pressure difference, ${} P_{1} > P_{2} {}$

![PX285 - H6 - stream line-2.png|500](/img/user/pics/PX285%20-%20H6%20-%20stream%20line-2.png)

- the viscous force:
$$F_{v} = \mu A \frac{\partial u}{\partial y}$$
	where, $A = \Delta x \, \Delta z$

- the net force applied at the fluid element:
$$\begin{align*}
A \mu \bigg\{ \frac{\partial u_{x}}{\partial y}\bigg|_{y+\Delta y} - \frac{\partial u_{x}}{\partial y} \bigg|_{y}\bigg\} &= A \mu \frac{\Delta\left(\partial u_{x}/\partial y\right)}{\Delta y} \Delta y \\
&=( P(x) - P(x+\Delta x))\Delta y \Delta z \\
&\approx -\frac{\partial P}{\partial x} \Delta x \Delta y \Delta z 
\end{align*}$$
- as the flow is stedy, there is no acceleration:
$$\begin{gather}
\frac{\partial P}{\partial x} \Delta x \Delta y \Delta z = \mu \frac{\partial^{2} {u_{x}}}{\partial {y}^{2}} \Delta x \Delta y \Delta z \\
\implies \frac{\partial P}{\partial x}  = \mu \frac{\partial^{2} {u_{x}}}{\partial {y}^{2}} = -Q
\end{gather}$$
- **note:** the negative sign vanishes as pressure is decreasing with $x$
- from the RHS:
$$u_{x} (y) = - \frac{Q}{2\mu}  y^{2} + Ay + B$$
- using the boundary conditions 
$$\begin{gather}
u_{x}(y=-a) = 0 = -\cfrac{Qa^{2}}{2\mu} -Aa + B \\
u_{x}(y=+a) = 0 = -\cfrac{Qa^{2}}{2\mu} + Aa + B \\
\implies A = 0 \;\text{and}\; B = \frac{Qa^{2}}{2\mu}
\end{gather}$$
$$\therefore u_{x}(y) = \frac{Q}{2\mu}(a^{2}- y^{2})$$
- constant $Q$ comes from the pressure difference
- using the LHS:
$$Q = -\frac{\partial P}{\partial x} \approx \frac{P_{1}-P_{2}}{L}$$
$$\therefore u_{x}(y) = \frac{P_{1}- P_{2}}{2L\mu}(a^{2}- y^{2})$$
- therefore, the form of the flow is parabolic

![[Pasted image 20250116145232.png\|500]]