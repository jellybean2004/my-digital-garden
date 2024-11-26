---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/px-275-formula-sheet/","created":"2024-11-26T21:29:24.782+00:00","updated":"2024-11-26T22:26:40.585+00:00"}
---

## A
### exact differentials
- for a function, $f(x,y)$, such that the total differential is $df = \left(\frac{\partial f}{\partial x}\right)\,dx + \left(\frac{\partial f}{\partial y}\right)\,dy = A\,dx + B$, the function is said to be an exact differential if $\frac{\partial A}{\partial y} = \frac{\partial B}{\partial x}$
- ie: 
$$\frac{\partial^{2}f}{\partial x \partial y} = \frac{\partial^{2}f}{\partial y \partial x}$$
### lagrange multipliers
- for a function, $f(x,y)$, the maxima or minima subject to constraint, $g(x,y)$, can be found using $\vec\nabla f + \lambda \vec\nabla g = 0$, where $\lambda$ is the lagrange multiplier
## B
### centroid
- in 2D:
$$\begin{align*}
	\bar x &= \frac{1}{Area}\iint x\,dA \\
	\bar y &= \frac{1}{Area}\iint y\,dA \\
	\bar z &= \frac{1}{Area}\iint z\,dA
\end{align*}$$
- in 3D:
$$\begin{align*}
	\bar x &= \frac{1}{Vol}\iiint x\,dV \\
	\bar y &= \frac{1}{Vol}\iiint y\,dV \\
	\bar z &= \frac{1}{Vol}\iiint z\,dV
\end{align*}$$
### jacobian
- for a coordinate transformation $(x,y,x) \to (u,v,w)$, the jacobian is defined as:
$$J = \frac{\partial (x,y,z)}{\partial (u,v,w)} = \left| \begin{matrix} \frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} & \frac{\partial x}{\partial w} \\ \frac{\partial y}{\partial u} & \frac{\partial y}{\partial v} & \frac{\partial y}{\partial w} \\ \frac{\partial z}{\partial u} & \frac{\partial z}{\partial v} & \frac{\partial z}{\partial w} \end{matrix} \right|$$
### surface of revolution
- if a function, $y = f(x)$, is rotated about the $x$-axis, the total surface area of the surface of revolution between $s_1$ and $s_2$ is given by:
$$A = \int_{s_{1}}^{s_{2}} 2\pi\,y\,ds$$
	where, $ds = \sqrt{1 + (\frac{dx}{dy})^{2}}\,dy$
### volumes of revolution
- if a function, $y = f(x)$, is rotated about the $x$-axis, the total volume between ${} x_1$ and ${} x_2$ is given by:
$$V = \pi \int_{x_{1}}^{x_{2}} (f(x))^{2}\,dx$$
### pappus' theorem
- pappus' first theorem gives the volume as:
$$V = 2\pi A \bar y$$
	where, $A$ is the surface area, and $\bar y$ is the centroid
- pappus' second theorem gives the surface area as:
$$A = 2\pi \bar yS$$
	where, $S$ is the area 
## D
### conservative fields
- a vector field is said to be conservative if:
	- its path integral is independent of the path taken
	- it can be expressed as the gradient of a scalar field
	- it has no curl
	- if its dot product with the path element is zero $(\vec a \cdot d\vec r = 0)$, or alternatively, its path integral around a closed loop is zero
### green's theorem
- suppose $\vec F$ is a vector field, so its path integral around a closed loop, bounding an area, $R$, is given by:
$$\oint_{C} \vec F \cdot d\vec r = \oint_{C} P\,dx  Q\,dy = \iint_{R} \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right)\,dA = \iint_{R} (\vec\nabla \cdot \vec F)\cdot d\vec A$$
### divergence theorem (2D)
- for a vector field, $\vec F$, its path integral around a closed loop is given by:
$$\oint_{C}\vec F\cdot d\vec n = \iint_{R}\vec\nabla \cdot \vec F\,dA$$
	where, $d\vec n$ is the normal element, given by $dy\, \hat i + dx\, \hat j$
## E
### stokes' theorem
- extending green's theorem into 3D:
$$\oint_{C}\vec F\cdot d\vec r = \iint_{S}(\vec\nabla \times \vec F)\cdot d\vec s$$
### divergence theorem (3D)
$$\iint_{S}\vec F\,d\vec s = \iiint_{V} (\vec\nabla \cdot \vec F)\,dV$$
