---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-i-integration/px-153-i10-conservative-fields/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:38:18.190+00:00"}
---

- what vector fields, $\vec P$, would not show this path dependence? 
$$\vec P = \vec\nabla V$$
	- vector fields which are the gradient of a potential (gradient of a scalar field) have integrals, $\int_{a}^{b} \vec P \cdot d\vec l$, which depend only on the end point, $a$ and $b$
	- such fields are called ***conservative fields***

- eg: is $\vec P = 5y^{2} \hat i +10xy \hat j$ conservative?
$$\nabla V = \left(\frac{\partial V}{\partial x}, \frac{\partial V}{\partial y}\right)$$
$$\begin{align*}
	\frac{\partial V}{\partial x} &= 5y^{2} & \implies V_{1} &= 5xy^{2}+ f_{1}(y) \\
	\frac{\partial V}{\partial y} &= 10xy & \implies V_{2} &= 5xy^{2} + f_{2}(x) \\	
\end{align*}$$
	- since $V_{1}=V_{2}$, $\vec P$ is conservative, where, $V = 5xy^{2}+c$

- it may be useful to parameterize over some variable, $t$
	- eg: 
$$W = \int_{\vec l_{1}}^{\vec l_{2}}\vec F \cdot d\vec l$$
		- the path: $\vec l(t) = x(t) \hat i + y(t) \hat j + z(t) \hat k$
		- as $t$ varies from $t_{1}\to t_{2}$, $\vec l(t)$ traces the path $C$: 
	$$W = \int_{t_{1}}^{t_{2}} \vec F (\vec l (t)) \cdot \frac{d \vec l}{dt} \, dt$$
- if $\vec F = -\vec\nabla U$ (conservative field), and $d\vec l = \frac{dx}{dt} dt \hat i + \frac{dy}{dt} dt \hat j + \frac{dz}{dt} dt \hat k$ : 
$$\begin{align*}
	W &= \int_{t_{1}}^{t_{2}} \left(\frac{\partial U}{\partial x} \frac{dx}{dt} + \frac{\partial U}{\partial y} \frac{dx}{dt} + \frac{\partial U}{\partial z} \frac{dx}{dt}\right)dt \\
	W &= -\int_{t_{1}}^{t_{2}} \frac{dU}{dt}dt = -[U]_{t_{1}}^{t_{2}} = U(t_{2})-U(t_{1})\\
	W &= U(x_{2},y_{2},z_{2}) - U(x_{1},y_{1},z_{1})
\end{align*}$$
- for conservative fields, the line integral depends only on endpoints, and not the path taken
	- eg: electrostatic potential: $\Delta U_{ab} = U_{b}-U_{a} = -\int_{a}^{b} \vec E \cdot d\vec l$
- eg: $\vec F$ is a vector field: $xy^{2}\hat i + 2\hat j + x\hat k$. $L$ is a path parameterized by $x=2t, \; y=\frac{2}{t}, \; z=1$, with ${} 1\leq t\leq 2 {}$. find $\int_{L}\vec F\cdot d\vec r$
	- on path $L$: 
$$\begin{align*}
	\vec F &= \frac{8}{t}\hat i + 2\hat j + 2t\,\hat k \\
	\vec r &= 2t\,\hat i + \frac{2}{t}\hat j + \hat k \\
	d\vec r &= 2dt\,\hat i - \frac{2}{t^{2}}dt\,\hat j + 0\hat k \\
\end{align*}$$
$$\int_{t_{1}}^{t_{2}}\vec F\cdot d\vec r = \int_{1}^{2} \left(\frac{16}{t}-\frac{4}{t^{2}}\right)dt = 16\ln{2}-2$$
	