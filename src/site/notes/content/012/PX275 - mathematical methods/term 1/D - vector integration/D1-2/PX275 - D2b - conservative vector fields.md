---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/d-vector-integration/d1-2/px-275-d2b-conservative-vector-fields/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:39.062+00:00"}
---

## conditions
- consider the integral: 
$$I = \int \vec a \cdot d\vec r$$
- the path dependence of the integral depends on the definition of $\vec a$
- for a *conservative* vector field, the integral is path independent
- a vector field must be continuous (partial derivatives) and simply connected (no holes)

- a vector field is said to be *conservative* if:
	- the path integral, $\int \vec a \cdot d\vec r$, is independent of the path taken ${} ^\dagger$
	- there exists a scalar function, $\phi$, such that the vector field can be expressed as the gradient of the scalar function, ie: $\vec a = \vec\nabla \phi$ 
	- it has no curl, ie: $\vec\nabla \times \vec a = 0$
	- $\vec a \cdot d\vec r$ is an exact differential, ie: $\oint \vec a \cdot d\vec r =0$ 
- **note:** validity of any one of the above four conditions means that the others are also valid

- consider a vector field, $\vec a = \vec\nabla \phi$, if $\vec a$ is conservative: 
$$\int_{A}^{B} \vec a \cdot d\vec r = \phi(B) - \phi(A)$$
## example 1
 - previously considered: ![Pasted image 20241107120733.png](/img/user/pics/Pasted%20image%2020241107120733.png)
 - taking 2 paths in each case:
	 - $OAB$
	 - $OB$
 ![Pasted image 20241107120848.png](/img/user/pics/Pasted%20image%2020241107120848.png)

 - considering $\vec G:$
	 - for path $OAB:$ 
	 $$\int_{OAB} \vec G \cdot d\vec r = \int_{x=0}^{x=1} x\,\hat i \cdot dx\, \hat i + \int_{y=0}^{y=1} x\,\hat i \cdot dy\, \hat j = \frac{1}{2}$$
	 - for path $OB:$ 
	 $$\int_{OB} \vec G \cdot d\vec r = \int_{OB} x\,\hat i \cdot (dx\,\hat i + dy\,\hat j) = \int_{x=0}^{x=1} x\,dx =\frac{1}{2}$$
- considering $\vec H:$
	- for path $OAB:$ 
	$$\int_{OAB} \vec H \cdot d\vec r = \int_{x=0}^{x=1} x\,\hat j \cdot dx\, \hat i + \int_{y=0,x=1}^{y=1} x\,\hat j \cdot dy\, \hat j = 1$$
	 - for path $OB:$ 
	 $$\int_{OB} \vec H \cdot d\vec r = \int_{OB} x\,\hat j \cdot (dx\,\hat i + dy\,\hat j) = \int_{y=0, x=y}^{y=1} x\,dy =\frac{1}{2}$$
- this is sufficient proof to show that $\vec H$ is non-conservative, but not to show that $\vec G$ is conservative as all paths need to be considered

- $\vec G$ does not have curl, therefore it is conservative, and has no path-dependence
- $\vec H$ has curl, therefore the integral has path-dependence

## example 2
past paper [2021 Q1]
$$\vec F = \frac{-y}{x^{2}+y^{2}} \hat i + \frac{x}{x^{2}+y^{2}}\hat j$$
- this looks similar to a $\vec B$-field around a wire
$$\begin{align*}
	\vec\nabla \times \vec F &= \left| \begin{matrix}\hat i & \hat j & \hat k \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ \frac{-y}{x^{2}+y^{2}} & \frac{x}{x^{2}+y^{2}} & 0\end{matrix} \right| \\
	&= \left[ \frac{\partial }{\partial x}\left(\frac{x}{x^{2}+y^{2}}\right) - \frac{\partial }{\partial y} \left(\frac{-y}{x^{2}+y^{2}}\right) \right]\hat k  \\
	&= \left[\frac{1}{x^{2}+y^{2}} \frac{-2x^{2}}{(x^{2}+y^{2})^{2}} - \left(\frac{1}{x^{2}+y^{2}} \frac{-2y^{2}}{(x^{2}+y^{2})^{2}}\right)\right] \hat k \\
	\vec\nabla \times \vec F&= 0
\end{align*}$$
$$\begin{align*}
	\oint_{C} \vec F\cdot d\vec r &= \oint \left(\frac{-y}{x^{2}+y^{2}} \hat i + \frac{x}{x^{2}+y^{2}}\hat j\right) \cdot (-\sin\phi\,dx\, \hat i + \cos\phi \,dy\, \hat j) \\
	&= \oint \left(\frac{y\sin\phi}{x^{2}+y^{2}}dx + \frac{x\cos\phi}{x^{2}+y^{2}}dy\right) \\
	&= \oint 1\\
	&= 2\pi 
\end{align*}$$
